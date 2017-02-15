
a)Write a Java code with the class name, “acad,” and a method called “main.”
Hard code the program with two integers and print the sum of those two
integers.

import java.util.Scanner;

public class acad {
	public static void main(String args[])
	{
		Scanner sc = new Scanner(System.in);
		int a = 123;
		int b  = 321;
		a= a+b;
		System.out.println(a);
		
	}

}

b)Rewrite the above code, wherein the inputs are provided by the user at
runtime and the output is printed.

import java.util.Scanner;

public class acad {
	public static void main(String args[])
	{
		Scanner sc = new Scanner(System.in);
		int a = sc.nextInt();
		int b  = sc.nextInt();
		a= a+b;
		System.out.println(a);
		
	}

}



c)Write a program with the method name, “sum()” that accepts two
parameters from the user and print the sum of those two numbers. The
output format should be:
First number is:
Second number is:
Sum is:





import java.util.Scanner;

public class acad {
	public static int sum(int a,int b)
	{
		int d = a+b;
		return d;
	}
	public static void main(String args[])
	{
		
	Scanner sc =new Scanner(System.in);
	int a = sc.nextInt();
	int b =sc.nextInt();
		
	System.out.println( "First number is:"+a);
		System.out.println("Second number is:"+b);
		System.out.println("Sum is:"+sum(a,b));
		
	}

}


d)Write a program to accept two numbers from “stdin” and find all the odd
as well as even numbers present in between them.


import java.util.Scanner;

public class acad {
	
public static void main(String args[])
{
	StringBuffer sb = new StringBuffer();
		StringBuffer sb1 = new StringBuffer();
		Scanner sc =new Scanner(System.in);
		int a = sc.nextInt();
		int b =sc.nextInt();
		for (int i = a; i <=b; i++) {
			if(i%2==0)
			{
				sb.append(i);
				sb.append(" ");
			}
			else
			{
				sb1.append(i);
				sb1.append(" ");
			}
		}
		System.out.println("The even number are");
		System.out.println(sb.toString());
		System.out.println("The odd number are");
		System.out.println(sb1.toString());
	}

}

e)Joe is scared to go to school. When her dad asked for the reason, Joe said
that she was unable to complete the task given to her by her teacher. The
task was to find the “first 10 multiples” of the number entered from
“stdin”. 




import java.util.Scanner;

public class acad {
	
public static void main(String args[])
	{
		Scanner sc= new Scanner(System.in);
		System.out.println("Input");
		int a = sc.nextInt();
		System.out.println("Output");
		for (int i = 1; i <=10; i++) {
			System.out.println(a+"x"+i+"="+i*a);
			
		}
	}

}


f)Write a program consisting the method “sum()” and demonstrate the
concept of method overloading using this method.


import java.util.Scanner;

public class acad {
	public static void sum(int a , int b)
    {
         System.out.println(a+b);
         
    }
    public static void  sum(String s ,String s1)  
    {
    	String s4 = s+s1;
         System.out.println(s4);
    }
	
	public static void main(String args[])
	{
		Scanner sc= new Scanner(System.in);
		
		int a = sc.nextInt();
		int b = sc.nextInt();
		String s = sc.next();
		String s4 = sc.next();
		sum(a,b);//sum with integer type as input
		sum(s,s4);//	sum with String type as input
		}
	}
  
  g)Can you overload a method with the same return type? Explain your
answer with proper logic.
  
  Yes we can overload method with same return type but the argument list should be diffrent. If it is the case that arguments are same as that of the other then aleast the sequence of the arguments should be changed.
  Method Overloading means to have two or more methods with same name in the same class with different arguments. The benefit of method overloading is that it allows you to implement methods that support the same semantic operation but differ by argument number or type.

Important Points

Overloaded methods MUST change the argument list
Overloaded methods CAN change the return type
Overloaded methods CAN change the access modifier
Overloaded methods CAN declare new or broader checked exceptions
A method can be overloaded in the same class or in a subclass
import java.util.Scanner;

public class acad {
	public static int sum(int a , int b)
    {
		return a+b; 
    }
    public static int  sum(char c)  
    {
    	int n =(int)c;
         return n;
    }
	
	public static void main(String args[])
	{
		Scanner sc= new Scanner(System.in);
		
		int a = sc.nextInt();
		int b = sc.nextInt();
		System.out.println("output");
		System.out.println(sum(a,b));//sum with integer type as input
		System.out.println(sum('a'));//	sum with char type as input
		}
	}
  Here we can see that the method sum has the same return type but argument list is different one gives actual sum and the other gives the ascii value of the character.
  
  
  h)Write a program in Java using Arrays, that sorts the element in a
descending order.
import java.util.Arrays;
import java.util.Collections;
import java.util.Scanner;

public class acad {
		public static void main(String args[])
	{
		Scanner sc= new Scanner(System.in);
		
		Integer[] intArray = new Integer[5];
	for (int i = 0; i < 5; i++) {
		intArray[i]=sc.nextInt();
	}
	Arrays.sort(intArray, Collections.reverseOrder());
	System.out.println("Output");
	for (int i = 0; i < intArray.length; i++) 
		
	
	{
		System.out.println(intArray[i]);
	}
	
	}
		
	}






