# project-3
Project: Project 2 – Student Management System – Version 2

Total Points Possible: 100 pts


Exercise Overview
Implement a Java program that creates a ‘Student Management System’
The user is presented with a menu and should be able to add students, delete students, display full list of students in order and lastly find a student by ID. 

Version 2 additional requirement: You will add another module called ‘Course Management System’. When the program starts users will see 3 main options 1. Student Management System 2. Course Management System 3. Exit. When users click 1, options from project 2 Version 1 will display. Exit SMS option should take the users back to the new top-level menu. When users click 2, the following new options for Course Management System will appear. Exit CMS from this menu should take the users back to the top-level menu.

Functional Requirements (how the code will work from the user perspective)
•	Program displays a description of the system
•	Possible options for the user to select:
o	Student Management System(SMS)
	Add a new student
	Activate or Inactivate a student
	Display all students in ascending order by first name and also write to a file called “StudentReport.txt”
	Search for a student
	Assign on-campus job(Ask for an ID, assign a job)
•	Possible jobs are – TA(Teaching Assistant or Research Assistant)
	Display students with on-campus job(you will need a method in your Student_Employee subclass). The subclass method should be able to print Student ID, Name, Employment type and Job 
	Exit SMS
o	Course Management System(CMS)
	Add a new course
	Assign student a new course
•	Ask for a Student ID and Course ID
•	Write to a file as soon as assignment is made. Filename = “CourseAssignment.txt”. If the file doesn’t exist, then create it
	Display students with assigned courses. You will have to read from the file
	Exit CMS
o	Exit


Technical Requirements (how you must code it)
The system should include the following Java components:
•	You must have two interfaces. One will be implemented by Student class and the other will be implemented by Course class. These two interfaces will declare all of your necessary getters, setter and/or displays
•	You must have these classes
1.	Driver class or main class
2.	Student class
	Student_Employee subclass
3.	Course class
•	You must implement an object array of students
1.	The object will have 
	Student ID(Randomly assigned ID between 0 and 99)
	Student First Name
	Student Last Name
	Student level
•	Freshman
•	Sophomore
•	Junior
•	Senior
	Active
•	true – this is the default
•	false
•	Student_Employee must inherit from Student class. You will need an object array for Student_Employee
1.	Fields are
	Employment type- Full time or Part time
	Job  - TA or RA 
•	Your course class will have
	Course ID(Example – 3311, 3312 etc.)
	Course name(Java 101, History 101  etc.)
•	You need to ask the user for the number of students they will have in the system 
o	Create the object array based on the number
•	Name of your source code main class as follows:  YourName_Section000_Project2.java
•	Variables (other than local vars) should be declared at the beginning of the main method.

Exception handling requirement:
•	You need to show at least 3 exception handling implementation within your program


Hints and suggestions.
•	Use comments to label the different sections (and subsections) of your code.
•	While writing code, print variable values to console frequently.
•	Use simple input values to test the menu and functions.

Students to complete the following sections:

Student Name: 	 Prof. Khan
Class and Section:  ITSS 3312, Section 501 or 002

Example output (copy and paste from the Eclipse console)

                Welcome to Student and Course Management System!

This system will allow you to manage students and courses. Let’s start with the number of students this system will have: 5

***Welcome to Student and Course Management System***

Press ‘1’ for Student Management System (SMS)
Press ‘2’ for Course Management System (CMS)
Press ‘0’ to exit

1
***Welcome to SMS***

Press ‘1’ to add a student
Press ‘2’ to deactivate a student
Press ‘3’ to display all students
Press ‘4’ to search for a student by ID
Press ‘5’ to assign on-campus job
Press ‘6’ to display all students with on-campus jobs
Press ‘0’ to exit SMS

1
Enter first name: Joe
Enter last name: Smith
Enter level of the student: Freshman

Joe Smith has been added as a Freshman with ID 7

***Welcome to SMS***

Press ‘1’ to add a student
Press ‘2’ to deactivate a student
Press ‘3’ to display all students
Press ‘4’ to search for a student by ID
Press ‘5’ to assign on-campus job
Press ‘6’ to display all students with on-campus jobs
Press ‘0’ to exit SMS

1
Enter first name: Mary
Enter last name: Cane
Enter level of the student: Junior

Mary Cane has been added as a Junior with ID 6

***Welcome to SMS***

Press ‘1’ to add a student
Press ‘2’ to deactivate a student
Press ‘3’ to display all students
Press ‘4’ to search for a student by ID
Press ‘5’ to assign on-campus job
Press ‘6’ to display all students with on-campus jobs
Press ‘0’ to exit SMS


***Welcome to SMS***

Press ‘1’ to add a student
Press ‘2’ to deactivate a student
Press ‘3’ to display all students
Press ‘4’ to search for a student by ID
Press ‘5’ to assign on-campus job
Press ‘6’ to display all students with on-campus jobs
Press ‘0’ to exit SMS

3

Joe Smith
ID: 7
Level: Freshman
Status: Active

Mary Cane
ID: 6
Level: Junior
Status: Active

***Welcome to SMS***

Press ‘1’ to add a student
Press ‘2’ to deactivate a student
Press ‘3’ to display all students
Press ‘4’ to search for a student by ID
Press ‘5’ to assign on-campus job
Press ‘6’ to display all students with on-campus jobs
Press ‘0’ to exit SMS

2
Enter the ID for the student you want to deactivate: 6

Mary Cane has been deactivated

***Welcome to SMS***

Press ‘1’ to add a student
Press ‘2’ to deactivate a student
Press ‘3’ to display all students
Press ‘4’ to search for a student by ID
Press ‘5’ to assign on-campus job
Press ‘6’ to display all students with on-campus jobs
Press ‘0’ to exit SMS

4
Enter the student ID: 7

Joe Smith
ID: 7
Level: Freshman
Status: Active

***Welcome to SMS***

Press ‘1’ to add a student
Press ‘2’ to deactivate a student
Press ‘3’ to display all students
Press ‘4’ to search for a student by ID
Press ‘5’ to assign on-campus job
Press ‘6’ to display all students with on-campus jobs
Press ‘0’ to exit SMS

5
Enter student ID: 7
Enter job: TA
Enter job type: part-time
Joe Smith has been assigned part-time TA job

***Welcome to SMS***

Press ‘1’ to add a student
Press ‘2’ to deactivate a student
Press ‘3’ to display all students
Press ‘4’ to search for a student by ID
Press ‘5’ to assign on-campus job
Press ‘6’ to display all students with on-campus jobs
Press ‘0’ to exit SMS

6
Joe Smith 
ID - 7
Part-time TA

***Welcome to SMS***

Press ‘1’ to add a student
Press ‘2’ to deactivate a student
Press ‘3’ to display all students
Press ‘4’ to search for a student by ID
Press ‘5’ to assign on-campus job
Press ‘6’ to display all students with on-campus jobs
Press ‘0’ to exit SMS

0

***Welcome to Student and Course Management System***

Press ‘1’ for Student Management System (SMS)
Press ‘2’ for Course Management System (CMS)
Press ‘0’ to exit

2

***Welcome to CMS***

Press ‘1’ to add a new course
Press ‘2’ to assign student a new course
Press ‘3’ to display student with assigned courses
Press ‘0’ to exit CMS

1
Enter course ID: 3311
Enter course name: Java 101
Confirmation: New course 3311 has been added

Press ‘1’ to add a new course
Press ‘2’ to assign student a new course
Press ‘3’ to display student with assigned courses
Press ‘0’ to exit CMS

2
Enter student ID: 7
Enter course ID: 3311
Confirmation: Joe Smith has been assigned course 3311

Press ‘1’ to add a new course
Press ‘2’ to assign student a new course
Press ‘3’ to display student with assigned courses
Press ‘0’ to exit CMS

3
Joe Smith
ID – 7
Courses: 3311

Press ‘1’ to add a new course
Press ‘2’ to assign student a new course
Press ‘3’ to display student with assigned courses
Press ‘0’ to exit CMS

0

***Welcome to Student and Course Management System***

Press ‘1’ for Student Management System (SMS)
Press ‘2’ for Course Management System (CMS)
Press ‘0’ to exit

0

Good Bye!!!






Research and Analysis.  Describe the system including input, processing, arrays, classes and output in your own words (10 pts).  Type response here.


Design.  Describe the major steps for solving the problem (10 pts).  Type response here.

I divided my program into few sections with subsections and denoted these using comments as follows:
•	Classes
•	Arrays
•	File creation, reading and writing
•	Search
•	Menu Options
o	What happens upon pressing each options
•	Variables declaration 
•	Gathering of inputs

Coding.  Source code and output (25 pts).  Submit your source code, your .java file, as a second file when you submit your project.

Testing.  Describe how you tested this program (5 pts).  Include descriptions of testing for specific calculations and/or algorithms, methods, and logic.

Create 2 members of your arrays to keep it simple as you build your program. Test everything.
//

What I have done so far

import java.util.Arrays;
import java.util.Scanner;
import java.util.Random; 
import java.util.*;
import java.io.File; 
import java.io.IOException;
import java.io.PrintWriter;

public class JosephChoi_Section002_Project3 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner allInputs = new Scanner(System.in);//scanner for all of the inputs the user will put in
		
		Random r = new Random();
		int randomInt = r.nextInt(100);//creating randoms to be used in the code later
		int selection;//different variables for if statement or deciding making within the code
		int option;
		int choice;
		
		System.out.println("***Welcome to Student and Course Management System***");//first option giver
		System.out.println("Press ‘1’ for Student Management System (SMS)");
		System.out.println("Press ‘2’ for Course Management System (CMS)");
		System.out.println("Press ‘0’ to exit");
		choice = allInputs.nextInt();//depending on what the user put will go to sms or cms
		
		if(choice == 1) { // student 
			System.out.println("\nStudent Managment System Main Menu");//message that will first be seen by user for sms
			System.out.println("Press 1 to add a new student");
			System.out.println("press 2 to Activate or inactivate a student");
			System.out.println("Press 3 Display all students in ascending order by first name");
			System.out.println("Press 4 to Search for a student");
			System.out.println("Press 5 to assign on campus job");
			System.out.println("Press 6 to display all students with on campus jobs");
			
			selection = allInputs.nextInt();
			option = allInputs.nextInt();
			Student[] StudentArray;
			StudentArray = new Student[5];
			
			Course[] CourseArray;
			CourseArray = new Course[5];
			String studentJob;
			switch(selection) {
			case 1://add new student
				System.out.println("please enter first name, lastn name, and level in order:");
				StudentArray[0] = new Student(randomInt, allInputs.next(), allInputs.next(), allInputs.next(), true);
				break;
				
			case 2: //activate student
				System.out.println("Type the id of the student: ");
				int studentSearchC2 = allInputs.nextInt();
				int searchedStudent = Arrays.binarySearch(StudentArray, studentSearchC2);
				
				if (selection == 1) {
					StudentArray[5].active = false;
				}else if (selection == 2) {
					StudentArray[5].active = true;
				}else {
				};
				Arrays.sort(StudentArray);
				break;
				
			case 3://order by first name and write to file StudentReport.txt
				Arrays.sort(StudentArray);
				System.out.println("Allstudents sorted: " + Arrays.toString(StudentArray));
				
				File file = new File("StudentReport.txt");
				if (!file.exists()) {
					try {
						file.createNewFile();
					}catch(IOExeption e) {
						e.printStackTrace();
					}
				}
				break;
				
			case 4: //search for a student
				System.out.println("Type the id of the Student: ");
				int studentSearchC4 = allInputs.nextInt();
				int searchedStudentC4 = Arrays.binarySearch(StudentArray, studentSearchC4);
				System.out.println("Student is: " + StudentArray[searchedStudentC4]);
				break;
				
			case 5://assign a job
				System.out.println("Enter your ID: ");
				int id = allInputs.nextInt();
				System.out.println("Enter job 1 for TA 2 for RA: ");
				int i = allInputs.nextInt();
				boolean employment;
				if(i < 1) {
					employment = false;
				}else if(i > 0) {
					employment = true;
				}
				if(i == 1) {
					studentJob = "TA";
				}else if(i == 2) {
					studentJob = "RA";
				}
				System.out.println("Student id is: " + id + " Job is: " + studentJob);
				
			case 6:
				// display for students with on campus job
				if(employment = true){
					//display
					super.display();
					
				}else {
					//dont display
				}
				
			case 7://exit the program
				System.out.println("Exiting prgram...");
				System.exit(0);
				break;
				
			default:
				System.out.println("This is not a valid menu option! please select another");
				break;
				}
			}//where while loop ends
		
		else if(choice == 2) {//course management system
			switch(selection) {
			System.out.println("Welcome to course management system");
			System.out.println("Enter 1 to Assign new course");
			System.out.println("Press ‘2’ to assign student a new course");
			System.out.println("Press ‘3’ to display student with assigned courses");
			
			case 1:
				//add a new course
				//1st add to file
				File file = new File("Courses.txt");
				if (!file.exists()) {
					try {
						file.createNewFile();
					}catch(IOExeption e) {
						e.printStackTrace();
					}
				}
				break;
				
			case 2:
				//assign student a new course
				System.out.println("Enter course ID: ");
				int cID = allInputs.nextInt();
				System.out.println("Enter Student ID: ");
				int studentID = allInputs.nextInt();
				File file = new File("CourseAssignment.txt");//write to file and create if not there
				if (!file.exists()) {
					try {
						file.createNewFile();
					}catch(IOExeption e) {
						e.printStackTrace();
					}
				}
				break;
			case 3:
				//display students with assigned courses
				break;
			case 4:
				//exit the program
				System.out.println("Exiting prgram...");
				System.exit(0);
				break;
			default:
				System.out.println("This is not a valid menu option! please select another");
				break;
			}
		}//while ends
		}//end of main class
	
	

	public class Student{//student class
		public int id;
		public String fName;
		public String lName;
		public String level;
		public boolean active;
		
		public Student(int id, String fName, String lName, String level, boolean active)
		{
			this.id = id;
			this.fName = fName;
			this.lName = lName;
			this.level = level;
			this.active = active;
		}
		
		public void display()//display message
		{
			System.out.println("Student id is " + id + " and student name is: " + fName + " " + lName + " student level is " + level + " student active: " + active);
		}
	}
	
	public class Course{//course class
		public int courseID;
		public String courseName;
		
		public Course(int courseID, String courseName) {
			this.courseID = courseID;
			this.courseName = courseName;
		}
		public void display2() {//display message
			System.out.println("Course id is " + courseID + "Course name is " + courseName);
		}
	}
	
	
	
	
	}
