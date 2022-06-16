# ComparatorJava
Comparators are used to compare two objects. In this challenge, you'll create a comparator and use it to sort an array.

The Player class is provided for you in your editor. It has  fields: a  String and a  integer.

Given an array of  Player objects, write a comparator that sorts them in order of decreasing score; if  or more players have the same score, sort those players alphabetically by name. To do this, you must create a Checker class that implements the Comparator interface, then write an int compare(Player a, Player b) method implementing the Comparator.compare(T o1, T o2) method.

Input Format

Input from stdin is handled by the locked stub code in the Solution class.

The first line contains an integer, , denoting the number of players.
Each of the  subsequent lines contains a player's  and , respectively.

Constraints

 players can have the same name.
Player names consist of lowercase English letters.
Output Format

You are not responsible for printing any output to stdout. The locked stub code in Solution will create a Checker object, use it to sort the Player array, and print each sorted element.

Sample Input

5
amy 100
david 100
heraldo 50
aakansha 75
aleksa 150
Sample Output

aleksa 150
amy 100
david 100
aakansha 75
heraldo 50
Language
Java 7

More
131415161718192021222324252627282930345678910111212
import java.util.*;

class Checker implements Comparator<Player>
{
    public int compare(Player a,Player b)
    {
        return b.score-a.score;
    }
}

…    }
}
Line: 42 Col: 2

Submit Code

Run Code

Upload Code as File

Test against custom input
Congratulations!

You have passed the sample test cases. Click the submit button to run your code against all the test cases.


Sample Test case 0
Input (stdin)

Download
5
amy 100
david 100
heraldo 50
aakansha 75
aleksa 150
Your Output (stdout)
aleksa 150
amy 100
david 100
aakansha 75
heraldo 50
Expected Output

Download
aleksa 150
amy 100
david 100
aakansha 75
heraldo 50
Contest Calendar
