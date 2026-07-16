3.Write The Program For The Followings:
a. Create methods add(). multiply(),substract(),divide() with suitable parameters and call these methods using concept of C# delegate.
CODE:-
using System;
delegate void Operation(int a, int b);
class Calculator{
 public void Add(int a, int b)
 {
 Console.WriteLine("Addition:"+(a+b));
 }
 public void Subtract(int a, int b)
 {
 Console.WriteLine("Subtraction:"+(a-b));
 }
 public void Multiply(int a, int b)
 {
 Console.WriteLine("Multiplication:"+(a*b));
 }
 public void Divide(int a, int b)
 {
 Console.WriteLine("Division:"+(a/b));
 }}
public class Program
{
 public static void Main(string[] args)
 {
 Calculator c= new Calculator();
 Operation obj;
 obj = c.Add(20, 10);
 obj=c.Subtract(20,10);
 obj=c.Multiply(20, 10);
 obj = c.Divide(20, 10);
 Console.WriteLine("Priti Yadav T054");
 }}



b.Write a program using multicast delegate.
CODE:-
using System;
delegate void Message();
class Demo{
 public void ShowMessage(){
 Console.WriteLine("Hello,Students");
 }
 public void Learn() {
 Console.WriteLine("Learning C# Delegates");
 }}
public class Program{
 public static void Main(string[] args){
 Demo d = new Demo();
 Message obj;
 obj = d.ShowMessage;
 obj();
 obj = d.Learn;
 obj();
 Console.WriteLine("Priti Yadav T054");
 }}



 
c.Create a class BankAccount with AccountNumber and Balance.Implement property for Balance with validation (Balance cannot be negative)
CODE:-
using System;
class BankAccount
{
 public int AccountNumber { get; set; }
 private double balance;
 public double Balance
 {
 get
 {
 return balance;
 }
 set 
 { 
 if (value >= 0)
 balance = value;
 else
 Console.WriteLine("Balance cannot be negative.");
 } }}
class Program
{
 static void Main(string[] args)
 {
 BankAccount b=new BankAccount();
 b.AccountNumber= 12345;
 b.Balance = 1000;
 Console.WriteLine("Account Number: " + b.AccountNumber);
 Console.WriteLine("Balance: " + b.Balance); 
 b.Balance = -500;
 Console.WriteLine("Priti Yadav T054");
 }}

------------------------------------------------------------------------------------------------------------------------------------------------------------------------
4. Create an ASP.NET Web Forms application using simple server controls.
a. Design a Student Registration Form using the following ASP.NET controls:
i. Label and TextBox to accept Student Name
ii. RadioButton to select Gender (Male/Female)
iii. DropDownList to select Course (BSc IT, BSc CS, BCA)
iv. CheckBox for accepting Terms & Conditions
v. Calendar control to select Date
vi. Button control to submit the form
vii. Label control to display the output
CODE:-






b. Create a Registration form to demonstrate use of various Validation controls.
CODE:-



c. Create Web Form to demonstrate use of Adrotator Control.
CODE:-



 
