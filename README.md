# testMavericksSolutions
testMavericksSolutions
1. What is the major difference between an abstract class and an interface ?


Abstract class							

1) Abstract class can have abstract and non-abstract methods.	
2) Abstract class doesn't support multiple inheritance.	
3) Abstract class can have final, non-final, static and non-static variables.	
4) Abstract class can have static methods, main method and constructor.
5) Abstract class can provide the implementation of interface.	
6) The abstract keyword is used to declare abstract class.	
7) Example:
	public abstract class Shape{
	public abstract void draw();
	}	


Interface
1) The interface keyword is used to declare interface.
2) Interface can't provide the implementation of abstract class.
3) Interface can't have static methods, main method or constructor.
4) Interface has only static and final variables.
5) Interface supports multiple inheritance.
6) Interface can have only abstract methods.
7) Example:
	public interface Drawable{
	void draw();
	}



2. Why is Java 7’s class inheritance flawed?


Ans2)  to avoid the diamond problem .Suppose we have two classes B and C inheriting from A. Assume that B and C are overriding an inherited method and they provide their own implementation. Now D inherits from both B and C doing multiple inheritance. D should inherit that overridden method, which overridden method will be used? Will it be from B or C? Here we have an ambiguity.


3. What are the major differences between Activities and Fragments ?


Ans3)  Activity has single view and fragment supports multiple views .


4. When using Fragments , how do you communicate back to their hosting Activity ?

Ans4)  we can then use getBaseActivity() as our root context.

5. Can you make an entire app without ever using Fragments ? Why or why not?Are there any special cases when you absolutely have to use or should use
Fragments?

Ans 5)  Yes ,I have to make an app that is only run on android devices not tablet fragements have een introduced in 3.0 for tablets only but after wards android sdk provide complete lifecycle for device and tablet as well .There is a case when we are working on scnarios where mater ,detail functionality is required then in that case fragments were very usefull.


6. What makes an AsyncTask such an annoyance to Android developers? Detail
some of the issues with AsyncTask , and how to potentially solve them


Ans6)    Android Async task is become tricky when we have to perform web synchronization and update our UI acordingly but async task will not breake in middle of operation now adays retrofit and volley is very usefull libraries to avoid async ambiguities
