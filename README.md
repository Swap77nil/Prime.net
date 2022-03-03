16 PRIME NUMBER<br>
using System;<br>
public class PrimeNumber<br>
{<br>
    public static void Main(string[] args)<br>
    {<br>
        int n, i, m = 0, flag=0;<br>
        Console.Write("Enter the Number to check Prime");<br>
            n=int.Parse(Console.ReadLine());<br>
        m=n/2;<br>
        for (i=2; i<=m; i++)<br>
        {<br>
            if (n%i==0)<br>
            {<br>
                Console.Write("Number is not prime");<br>
                flag=1;<br>
                break;<br>
            } <br>
        }<br>
        if (flag==0)<br>
            Console.Write("Number is Prime");<br>
    }<br>
}<br>

OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145365/155660263-381f8ea6-1b35-4ed9-8643-345b0d5def39.png)<br>
![image](https://user-images.githubusercontent.com/98145365/155660400-995429b6-f7d4-4942-acb6-a2cbdd6fcd09.png)<br>

17:PALNDROME<br>
using System;<br>
public class Palindrome<br>
{<br>
    public static void Main(string[] args)<br>
    {<br>
        int n, r, sum = 0, temp;<br>
        Console.Write("Enter the number");<br>
        n=int.Parse(Console.ReadLine());<br>
        temp=n;<br>
        while (n>0)<br>
        {<br>
            r=n%10;<br>
            sum=(sum*10)+r;<br>
            n=n/10;<br>
        }<br>
        if (temp==sum)<br>
            Console.Write("Number is Palindrome");<br>
        else<br>
            Console.Write("Number is not Palindrome");<br>
    }<br>
}<br>

OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145365/155662205-08262ff8-e93e-4f67-ab49-87a902e1e978.png)<br>
![image](https://user-images.githubusercontent.com/98145365/155662303-0a68c3e0-b01c-4e57-b9d9-facab849da17.png)<br>

18.FACTORIAL<br>
using System;<br>
public class Factorial<br>
{<br>
    public static void Main(string[] args)<br>
    {<br>
        int i, fact = 1, number;<br>
        Console.Write("Enter any number");<br>
        number=int.Parse(Console.ReadLine());<br>
            for (i=1; i<=number; i++)<br>
        {<br>
            fact=fact*i;<br>
        }<br>
        Console.WriteLine("Factorial of "+number+ "is "+fact);<br>
    }<br>
}<br>

OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145365/155663931-84a4f76d-c2df-4055-a34d-61ef404f5df2.png)<br>

19.AMSTRONG<br>
using System;<br>
public class Amstrong<br>
{<br>
    public static void Main(string[] args)<br>
    {<br>
        int n, r, sum = 0, temp;<br>
        Console.Write("Enter the Number=");<br>
        n=int.Parse(Console.ReadLine());<br>
        temp=n;<br>
        while (n>0)<br>
        {<br>
            r=n%10;<br>
            sum=sum+(r*r*r);<br>
            n=n/10;<br>
        }<br>
        if (temp==sum)<br>
            Console.Write("Armstrong Number");<br>
        else<br>
            Console.Write("Not Armstrong Number");<br>
    }<br>
}<br>

OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145365/155666477-0d929e93-15a8-4f20-8232-afa7912c98fe.png)<br>
![image](https://user-images.githubusercontent.com/98145365/155667664-28f55c90-dd48-4eeb-9717-3a8fd707c39b.png)<br>

21)Sum of digit<br>
using System;<br>
public class Sum<br>
{<br>
    public static void Main(string[] args)<br>
    {<br>
        int n, sum = 0, m;<br>
        Console.WriteLine("Enter a Number");<br>
        n=int.Parse(Console.ReadLine());<br>
        while (n>0)<br>
        {<br>
            m=n%10;<br>
            sum=sum+m;<br>
            n=n/10;<br>
        }<br>
            Console.WriteLine("Sum is= "+sum);<br>
        }<br>
    }<br>
    
    OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145365/155669009-93e4d0fd-7f15-4649-a6ab-94ccbb00454a.png)<br>


22.REVERSE<br>
using System;<br>
public class Reverse<br>
{<br>
    public static void Main(string[] args)<br>
    {<br>
        int n,reverse=0,rem;<br>
        Console.Write("Enter a number");<br>
        n=int.Parse(Console.ReadLine());<br>
        while (n!=0)<br>
        {<br>
            rem=n%10;<br>
            reverse=reverse*10+rem;<br>
            n/=10;<br>
}<br>
        Console.WriteLine("Reversed Number"+reverse);<br>
    }<br>
}<br>

OUTPUT:<br>
