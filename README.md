# 608-mod6

**Chapter 9 Notes:**

Introduction:
- Files provide long term retention of typically large amounts of data.
- Data maintained in files is persistent. 
- Store files on secondary storage devices. 
- Exception Handling
  - An exception indicates an execution-time problem. 

Files:
- Text file - Sequence of characters
- Binary file - sequence of bytes
- end-of-file-marker
  - Denotes the end of a file
- Standard file objects:
  - sys.stdin - standard input file object 
  - sys.stdout - standard output file object 
  - sys.stderr - standard error file object 

Text-File Processing: 
- Python's with statement
  - Acquires a resource and assigns its corresponding object to a variable
  - Allows the application to use the resource via that variable
  - Calls the resource objects close method to release the resource when program control reaches end. 
  - Built-in open function opens the file contents.
  - Mode argument specifies the file-open mode.  
  - .txt indicates plain text file. 
  - As clause assigns the variable the name
- Reading data from a text file:
  - *SEE JUPYTER LAB FILE* 
  - Argument 'r' is used to read the file.
  - File objects readlines method also can be used to read an entire text file. 
  - Use function seek in order to locate a specific file position. 

Updating Text Files:
- Steps to update: *See Jupyter Lab examples* 
- os module provides functions for interacting with operating system. 

Sterilization with JSON:
- JSON objects contain a comma-separated list. 
- JSON supports arrays 
- json module enables you to convert objects to JSON --> This is known as steralizing data. 
- The dump function steralizes a file to json. 
- Can also desteralize json 
  - load function reads the entire JSON contents of its file object argument and converts the JSON into a python object. 
  - Can also use [] to locate a specific index in a JSON file. 

Focus on Security: pickle Serialization and Deserialization 
- Python's pickle module can serialize objects in a python specific data format. 
- Pickle files can be hacked. 
- legacy code - old code that's often no longer supported. 

Additional Notes Regarding Files: 
- Page 331 contains a chart for the different file modes. 
- read method returns a string containing the number of characters specified by the method's integer argument. 
- readline method returns one line of text as a string. 
- writelines method recieves a list of strings and writes its contents to a file. 
- The classes that python uses to create file objects are defined in the python standard library's io module. 

Handling Exceptions:
- A FileNotFoundError occurs if you attempt to open a non-existent file for reading. 
- A PermissionsError occurs if you attempt an operation for which you do not have permission. 
- Division by zero
  - Invalid input resulting in a ZeroDivisionError
  - This ZeroDivisionError exception is raised an displayed. 
  - A ValueError occurs if you attempt to convert to to an integer a string. 
- Try statements
  - enables exception handeling 
  - A try clause may be followed by an except clause to handle exceptions. 
  - the else clause only executes if no exceptions occur. 
- Point in program where exception occurs is the raise point.
- Catching Multiple Exceptions in One except clause
  - Put all your except statements in a tuple. 

Finally Clause:
- Closing a file helps prevent a resource leak in which the file resource is not available to other programs. 
- finally clause is guaranteed to execute, regardless of whether its try suite executes successfully. 

Explicitly Raising an Exception:
- The raise statement explicitly raises an exception. 

(Optional) Stack Unwinding and Tracebacks:
- Includes the lines of code that lead to the exception. 
- Traceback shows the type of exception that occured followed by the complete function call stack. 
- When an exception is not caught in a given function, stack unwinding occurs. 

Intro to Data Science: Working with CSV Files: 
- CSV (Comma-separated values)
- The csv module provides functions for working with CSV files. 
- writerows can replace all writerow values.
- csv's reader function returns an object that reads a CSV-format dat from the specified file object. 
- Be careful with commas in a CSV file. 
- Reading CSV Files into Pandas DataFrames
  - The popular Rdatasets repository provides links over 1100 free datasets in comma-separated values format. 
- Data method 'head' returns the first five rows.
- data method 'tail' returns final five rows.



**Chapter 17 Notes: Big data - Hadoop, Spark, NoSQL, and IoT **

SQL:
- Structured Query Language 
















