# ConditonalStatements

# Conditional Statements

 Conditions help us make decisions! It checks if the condition is true or false / boolean.

There are 4 types of conditional statements.

1- If condition

2- If-else condition

3- Else-if condition(if-else if ….else)

4- Switch
  

You use these conditions to perform different tasks. 


## If Condition:

If condition only takes one option. The option is going to be the true option. If the option is true then it will be executed. If the condition is false, the condition won’t get executed.

if(condition){

	logics
  
}

Ex:

int num = 6;

if(num == 6){

	System.outprintln(“Correct!”);
  
}


## If Else:

If - else takes two options. When the if condition is false, else block is executed.

if(condition){

	logics
  
}

else{

	logics
  
}

Ex:

int number = 10;

if(number == 10){

	System.outprintln(“Correct!”);
  
}
else{

	System.outprintln(“Wrong!”);
  
}


## Else-If condition:

Else if takes more than two options. You can use as many else if blocks as you want!  “Else - if “condition is going to be in-between if condition and else condition.

if (condition)

	{	logics 
  
	}
  
	else if (condition)
  
	{	logics 
  
	}
  
	else if (condition)
  
	{	logics 
  
	}
  
	else
  
	{	logics 
  
	}


Ex:

import java.util.Scanner;

class Day{

	public static void main(String[] args){
  
	Scanner s = new Scanner(System.in);
  
	String day = s.next();

	if(day.equals("Monday") ||day.equals("Tuesday")  || day.equals("Wednesday")){
  
		System.out.println("Discount 5%");
    
	}
  
	else if(day.equals("Thursday")  || day.equals("Friday")) {
  
		System.out.println("Discount 4%");
    
	}
  
	else if(day.equals("Saturday")  || day.equals("Sunday")) {
  
		System.out.println("Discount 3%");
    
	}
  
	else{
  
		System.out.println("You typed in the wrong thing. Try again");
    
	}

   }

}

### Ternary Operator:

Ternary Operator is a short hand of the if - else condition. It uses a ? ( Question mark symbol). 

Ex:

String res = (10 < 20 ? “Correct!” : “False”); 

If 20 is greater than 10:

Option 1:

It will print “Correct”

Option 2:

Else it will print “False”



# Switch:



Else if is condition based but switch is used for argument based. “Based on the value of the expression” different parts will be executed. Switches are used to take more than two options but it is argument based.

In a switch we have cases, defaults, and breaks.  Cases are used for options. But if none of the cases match then we use default. Breaks are used to stop the case.


### Note:
We don’t have to use breaks in a case. There will be no error if we don’t use the breaks. If we don’t use the break then it will execute all the cases one by one until one case uses break. It is recommended to use break.


import java.util.Scanner;
class Test 

{	public static void main(String[] args)

	{	Scanner s = new Scanner(System.in);
  
		System.out.println("Enter your number....");
    
		int num = s.nextInt();
    
	
		switch (num)
    
		{	case 8:  System.out.println("Good morning");
    
					 break; 
           
			case 12: System.out.println("Good afternoon");
      
					 break; 			
           
			case 17 :  System.out.println("Good evening...");
      
						break; 			
            
			case 20 : System.out.println("Good night");
      
						break; 
            
			default : System.out.println("This is work time focus on your work..");
      
						break;
            
		}
    
	}
  
  
}


In switch, float, double and long are not allowed because they have large values.


