# Ex04-Constructor
## Aim:
 To write a C# program to calculate the salary of an employee by passing the name, designation, noofexperience, basic salary and insurance amount through constructor.
 
 ## Algorithm:
 ### Step1:
 Start the C# program in visual studio 2022.


 ### Step2:
 Create a class and a constructor.


  ### Step3:
  Get employee name, Designation, No of experience, basic salary and insurance amount from the User.



 ### Step4:
Call salary method in constructor to calculate salary.


 ### Step5:
 Call display method to display the output.



 ### Step6:
 Run the prgram.





 
 
 
 ## Program:
 ~~~
 using System;
namespace employee
{
   class employee {
       public string name, designation;
       public int no_exp, salary,insurance;
       public double hra,ta,basic_pay;
       

       public employee(string name, string designation, int no_exp, int salary,int insurance)
       {
           this.name = name;
           this.designation = designation;
           this.no_exp = no_exp;
           this.salary = salary;
           this.insurance = insurance;
           
       }
       public void Salary()
       {
           hra = this.salary * 0.2;
           ta = this.salary * 0.1;
           basic_pay = this.salary + hra + ta - this.insurance;
       }
       public void display()
       {
           Console.WriteLine("Name of the employee is {0} having {1} of experience, working as {2}",this.name,this.no_exp,this.designation);
           Console.WriteLine("Receives {0} of salary",basic_pay);
       }
   }
   class employeeDeatils
   {
       public static void Main(string[] args)
       {
           employee emp1 = new employee("Hari","Tester",10,30000,1000);
           emp1.Salary();
           employee emp2 = new employee("Latha", "Developer", 5, 25000, 1000);
           emp2.Salary();

           emp1.display();
           emp2.display();
       }
   }

}

 ~~~
 ## Output:
 ![Exp4](https://user-images.githubusercontent.com/94381788/230870667-712bef17-d45a-4b6a-8869-514c29a81c2a.png)

 
 ## Result:
 Thus C# program to calculate the salary of an employee by passing the name, designation, noofexperience, basic salary and insurance amount through constructor is executed successfully.


