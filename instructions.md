# Instructions

<details>
  <summary>
    💡 REPL Guide
  </summary>

  - To toggle commenting, highlight the line(s) and press Ctrl + /
  - To move a statement or block of statements one indent to the right, highlight the statement(s)  press Tab
  - To move a statement or block of statements one indent to the left, highlight the statement(s)  press Shift+Tab
  - Avoid using backspaces or spaces to remove or place indents
  - To ask the instructor a code question, highlight the line(s) of code and press Alt + / and type in your question/issue/comment and click on collapse
  - To view comments placed by the instructor click on the comment icon at the end of any highlighted code
  - If your issue is resolved, click on Resolve to remove the comment
</details>

<details>
  <summary>
    Assignment Instructions
  </summary>
 
  - All class definitions will be in classes.py (It will not be inside any folder)
  - Refer to the [inheritance diagram](https://github.com/suchialex/CINS3002-HW10/blob/main/Employee%20inherited%20from%20Person.pdf) for relationships between classes
</details>

# Start Working

<details>
  <summary>
    ✅ Create Pycharm Project
  </summary>

  - Create new file main.py
  - Create folder hw10
  - Inside the folder create a Python file called `classes.py` two folders `employees` and `students`
  - Inside the folder `employees` create files class_functions.py and validations.py
  - Copy the contents of class_functions.py and validations.py from the previous assignment
  - Inside the folder `students` create files class_functions.py and validations.py

</details>

## In classes.py

<details>
  <summary>
    ✅ 1. Define class <code>Person</code>
  </summary>

  - Create the class and define initializer accepting attributes name, phone, email and initialize as __protected attributes__ (⏩ Refer to 10-3a)
  - Define accessor methods `get_name`, `get_phone`, `get_email` (⏩ Refer to 10-5a)
  - Define two mutator methods `set_name` and `set_phone` accepting new_name and new_phone respectively (⏩ Refer to 10-6a)
</details>


<details>
  <summary>
    ✅ 2. Define class <code>Employee</code> as a child of <code>Person</code>
  </summary>

  - Create the class and define initializer
    - accepting attributes emp_id, name, phone, email, department, salary
    - Call the parent init to initialize name, phone, email (⏩ Refer to 11-5 Try this)
    - initialize emp_id, department and salary as __protected attributes__ 
  - Define mutators `set_salary`, `set_department` accepting new_salary and new_department (⏩ Refer to 10-6a)
  - Define accessors `get_empid`, `get_department`, `get_salary` (⏩ Refer to 10-5a)
  - Define str method to return employee data fields formatted as shown below:
    - emp_id centered over 6 characters
    - name left aligned over 15 characters
    - phone center aligned over 12 characters
    - department center aligned over 6 characters
    - salary right aligned over 8 characters
    - email left aligned over 15 characters   
    (⏩ Refer to 10-4)
</details>


<details>
  <summary>
    ✅ 3. Define class <code>Student</code> as a child of <code>Person</code>
  </summary>

  - Create the class and define initializer
    - accepting attributes stu_id, name, phone, email, major, classification
    - Call the parent init to initialize name, phone, email (⏩ Refer to 11-5 Try this)
    - initialize stu_id, major and classification as __protected attributes__ 
  - Define mutators `set_major`, `set_classification` accepting parameters new_major and new_classification (⏩ Refer to 10-6a)
  - Define accessors `get_stuid`, `get_major`, `get_classification` (⏩ Refer to 10-5a)
  - Define str method to return all the instance data in the format given below 
    - stu_id centered over 8 characters
    - name left aligned over 15 characters
    - phone center aligned over 12 characters
    - major center aligned over 6 characters
    - classification center aligned over 4 characters
    - email left aligned over 15 characters  
    (⏩ Refer to 10-4)

</details>

## In employees/class_functions.py

<details>
<summary>
  ✅ Import the Employee class from classes.py
</summary>

  - Write an import statement to import the Employee class from classes.py
</details>

## In main.py

<details>
<summary>
  ✅ Test code
</summary>

  - Inside main()
    - Import and call the employee_operations() located in class_functions.py
  - In class_functions.py, in display_employees function, replace the print statment with formatted values and simply print the object (this will call the str method)
  - Execute code
  - All the employee operations should work without having to make any changes
</details>

## Create New Folder Students

## Create new file class_functions.py in students folder

## In students/class_functions.py

<details>
<summary>
  ✅ Write code for functions
</summary>

Using the Student class, create student objects to write code for the following functions. (Refer to employee/class_functions.py if needed). You must import the class from classes2.py

  - student_operations
  - file_to_dictionary (unpickle students.class and store in a dictionary, if file not found or empty return empty dictionary)
  - generate_next_student_id (you may set the default ID at 30010)
  - add_student (call the init by creating a student object)
  - lookup_student (get attributes using get methods)
  - update_student_name (use the mutator method)
  - update_student_phone (use the mutator method)
  - update_student_major (use the mutator method)
  - update_student_classification (use the mutator method)
  - delete_student
  - display_students (in a for loop, print each student object)

    Instructions:
    - All these operations are in a while loop until user presses x or X
    - You must create a dictionary of student objects
    - Serialize the dictionary and save in the file students.class (⏩ Refer to 9-10)
    - Call this function in main.py after the function call to employee_operations functions()
    - Bonus 2pts: If you write validation functions in validations.py
</details>
