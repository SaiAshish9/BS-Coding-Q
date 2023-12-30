# BS-Coding-Q 

```
Practice Q

Problem
Your friend and you made a list of topics and both of them voted if they like or dislike the topic. They wrote 0 to denote dislike and 1 to denote like. They asked you to count the number of topics that both like or both dislike.

Input format

The first line contains a string, , denoting Bob's likes and dislikes.
The second line contains a string, , denoting Alice's likes and dislikes.
Output format

Print the number of topics both, Bob and Alice, like or dislike.

Constraints

Both A and P contains only 0 and 1. 0 denotes dislike and 1 denotes like.
```

```
Sample Input
010101
101101
Sample Output
3

Score 20
```

```
import java.io.BufferedReader;
import java.io.InputStreamReader;
import java.util.*;

 class TestClass {
 public static void main(String args[] ) throws Exception {
   Scanner sc=new Scanner(System.in);         String s1=sc.nextLine();     
   String s2=sc.nextLine();         int count=0;         for(int i=0;i<s1.length()&& i<s2.length();i++)
    {             char c1=s1.charAt(i);             char c2=s2.charAt(i);
           if(c1=='0' &&c2=='0')
      {                 count++;             }
     else if(c1=='1'&&c2=='1')
   {                 count++;             }         }
    System.out.print(count);       } }
```
