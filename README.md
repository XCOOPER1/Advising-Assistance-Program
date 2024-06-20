Advising Assistance Program

Description
The Advising Assistance Program is a command-line application designed to help students and advisors manage course information. It allows users to load course data from a file, print a list of all courses, and display detailed information about a specific course, including its prerequisites.

 Algorithm
The program primarily uses standard C++ data structures and algorithms. Here's an overview of the key components and algorithms used:

1. Data Structure:
    Course Structure: A `struct` named `Course` holds course information, including the course number, name, and a list of prerequisites.
    Course Map: A `std::map` is used to store courses with the course number as the key and the `Course` struct as the value.

2. Functions:
    loadCourses(const std::string& filename)`: Reads course information from a file and populates the `std::map` of courses.
    printCourseList(const std::map<std::string, Course>& courses)`: Prints a sorted list of all course numbers and their names.
    printCourseInfo(const std::map<std::string, Course>& courses, const std::string& courseNumber)`: Prints detailed information about a specific course, including its prerequisites.

3. Main Program:
    The main loop presents a menu to the user with options to load data, print the course list, print course information, or exit the program.
    Based on the user's choice, the corresponding function is called to perform the desired action.


3. Menu Options:
    1. Load Data Structure**: Enter the filename of the course data file to load the course information.
    2. Print Course List**: Display a sorted list of all courses and their names.
    3. Print Course**: Enter a course number to display detailed information about that course, including its prerequisites.
    9. Exit**: Exit the program.

Example
Here is an example of how the program works:

1. Start the program:
      
2. Choose option 1 to load course data:
    
    Enter the file name: courses.txt
    
3. Choose option 2 to print the course list:
    
    101, Introduction to Programming
    102, Data Structures
    
4. Choose option 3 to print information about a specific course:
    
    What course do you want to know about? 102
    102, Data Structures
    Prerequisites: 101
    
5. Choose option 9 to exit:
    
    Thank you for using the course planner!

I hope this README provides a clear understanding of the Advising Assistance Program, how it works, and how to use it. If you have any questions or need further assistance, please feel free to ask!
