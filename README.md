
# EX-01-Datatypes-Operators
## NAME: VASANTH N 
## REG.NO: 212224110060
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
	#include <stdio.h>
	int main()
	{
	    char ch,ch1,ch2;
	    scanf("%c%c%c",&ch,&ch1,&ch2);
	    printf("The reverse of %c%c%c is %c%c%c",ch,ch1,ch2,ch2,ch1,ch);
	    return 0;
	    
	}

## OUTPUT:


![image](https://github.com/user-attachments/assets/f05141a7-8c03-433f-a8a2-14aeb750fd4f)


## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:

	#include <stdio.h>
	int main()
	{
	    int a;
	    scanf("%d",&a);
	    if (a>=0)
	    {
	        printf("Number is positive.");
	    }
	    else
	    {
	        printf("Number is negative.");
	    }
	    return 0;
	}

# OUTPUT:



![image](https://github.com/user-attachments/assets/bfdb37cb-a6f7-4abb-9826-56957ca82e0a)





# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
#include <stdio.h>
		
		int main() {
		    int n1,d1,n2,d2;
		    float fra1,fra2,min;
	
		    scanf("%d %d", &n1,&d1);
		
		    scanf("%d %d", &n2,&d2);
		
		    fra1 = (float)n1/d1;
		    fra2 = (float)n2/d2;
		
		    min = (fra1 < fra2) ? fra1 : fra2;
		
		    printf("The smaller fraction in decimal form is: %.2f\n", min);
		
		    return 0;
		}


## OUTPUT:




![image](https://github.com/user-attachments/assets/b97c9e1d-26d0-4da7-aab6-fb064e17c8eb)





## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:

	#include <stdio.h>
	int main()
	{
	    int a;
	    scanf("%d",&a);
	    if(a==1)
	       printf("TRUE");
	       
	   
	}
## OUTPUT:






![image](https://github.com/user-attachments/assets/b71ab6e8-d568-4b00-b7bb-c880e1d8a66e)



	

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
	#include <stdio.h>
	#include <string.h>
	
	int main()
	{
	    int phy,che,ca,total;
	    float per;
	    char div[10];
	
	   
	    scanf("%d%d%d",&phy,&che,&ca);
	    total = phy+che+ca;
	    per = total/3.0;
	    if (per>=60)
		 strcpy(div,"First");
	    else if (per<60&&per>=48)
		    strcpy(div,"Second");
		else
		    if (per<48&&per>=36)
			strcpy(div,"Pass");
		     else
			strcpy(div,"Fail");
	
	      
	       printf("Total Marks = %d\nPercentage = %5.2f\nDivision = %s\n",total,per,div);
	       return 0;
	}
## OUTPUT:
![image](https://github.com/user-attachments/assets/2563c7cc-03ad-4bb0-8969-5e638c015e39)


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

