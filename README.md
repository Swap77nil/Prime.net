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
![Screenshot 2022-03-03 113032](https://user-images.githubusercontent.com/98145032/156505670-e58df890-a97d-46f5-b77d-0c51ce4c8496.png)
# Image-Processing<br>

Program 1:<br>
import cv2<br>
img=cv2.imread('blue.jpg',0)<br>
cv2.imshow('image',img)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

<br>
Program 2:<br>
import matplotlib.image as mping<br>
import matplotlib.pyplot as plt<br>
img=mping.imread('leaf1.jpg')<br>
plt.imshow(img)<br>
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/97939356/173813368-136d4654-07a2-40c2-8f6f-d616996be0e9.png)
![Screenshot 2022-06-15 161934](https://user-images.githubusercontent.com/98145032/173815255-f95445d5-72e1-4318-a569-303caa92e8d1.png)<br>
<br>
3:
from PIL import Image<br>
img=Image.open('butterfly1.jpg')<br>
img=img.rotate(180)<br>
img.show()<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
<br>
4:
from PIL import Image<br>
img=Image.new('RGB',(200,400),(255,255,0))<br>
img.show()<br><br>
<br>
5:
import cv2<br>
import matplotlib.pyplot as plt<br>
import numpy as np<br>
img=mping.imread('plant1.jpg')<br>
img=cv2.cvtColor(img,cv2.COLOR_BGR2RGB)<br>
plt.imshow(img)<br>
plt.show()<br>
OUTPUT:<br>
![Screenshot 2022-06-15 162257](https://user-images.githubusercontent.com/98145032/173815385-69c271f2-9c88-4a29-b227-82b8c19e6f77.png)<br>
<br>
6:
from PIL import Image<br>
img=Image.open('plant1.jpg')<br>
print('Filename:',img.filename)<br>
print('Format:',img.format)<br>
print('Mode:',img.mode)<br>
print('Size:',img.size)<br>
print('Width:',img.width)<br>
print('Height:',img.height)<br>
img.close()<br>
OUTPUT:<br>
![Screenshot 2022-06-15 162538](https://user-images.githubusercontent.com/98145032/173815512-6ecc0eb6-03aa-4f73-8771-e178125146a8.png)
<br>
<br>
7:
from PIL import ImageColor<br>
img1=ImageColor.getrgb("yellow")<br>
print(img1)<br>
img2=ImageColor.getrgb("red")<br>
print(img2)<br>
OUTPUT:<br>
![Screenshot 2022-06-15 162807](https://user-images.githubusercontent.com/98145032/173815622-3e93c08c-63fe-47c1-b2cb-2ed4297301d2.png)
<br>
8:
import cv2
img=cv2.imread('blue.jpg')
print('original image length width',img.shape)
cv2.imshow('original image',img)
cv2.waitKey(0)
#to show resized image
imgresize=cv2.resize(img,(150,160))
cv2.imshow('Resized image',imgresize)
print('Resized image length width',imgresize.shape)
cv2.waitKey(0)
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98145032/174045246-7e960d12-d8ab-4519-94f1-48c823315080.png)

