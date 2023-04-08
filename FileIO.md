# FileIO & Exceptions

## Why This Topic Matters
File Input/Output (IO) is an essential part of programming as programs often need to store data in a file and retrieve it later. Python provides various functions and modules to read and write files. On the other hand, exceptions are a common occurrence in programming, and properly handling them is crucial to ensure that the program executes without errors. Exception handling is a powerful technique that allows the program to gracefully recover from an error and continue execution.

## Reading Questions
1. What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?

The 'with' statement is used when working with unmanaged resources like file IO. The purpose of 'with' is to make sure that the file is closed correctly after the block inside the 'with' statement is executed. The 'with' statement handles opening and closing the file, so there is no need to use file.close() explicitly. It also provides better error handling by automatically closing the file in case of an exception.

Example:
```
with open('file.txt', 'r') as f:
    data = f.read()
    print(data)
# file automatically closed after block is executed

```
2. Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method.

The 'read()' method reads the entire content of the file as a single string. It takes an optional argument that specifies the number of bytes to read from the file.

Example:
```
with open('file.txt', 'r') as f:
    data = f.read()
    print(data)

```
The 'readline()' method reads a single line from the file. If called again, it reads the next line and so on until the end of the file is reached. It returns an empty string when there is no more line to read.

Example:

```
with open('file.txt', 'r') as f:
    line = f.readline()
    while line:
        print(line)
        line = f.readline()

```

3. Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example.

Exception handling is the process of catching and handling errors that occur during the execution of a program. In Python, exceptions are objects that represent errors that occur during the execution of a program.

The 'try' block is used to enclose the code that might raise an exception. The 'except' block is used to catch the exception and handle it. The 'finally' block is used to execute code that must be run regardless of whether an exception was raised or not.

Example:

```
try:
    x = int(input("Enter a number: "))
    y = 1/x
except ZeroDivisionError:
    print("Cannot divide by zero")
else:
    print("Result is", y)
finally:
    print("Done")


```
In this example, if the user enters 0, a ZeroDivisionError is raised, and the code inside the except block is executed. If the user enters a non-zero number, the code inside the else block is executed. Finally, the code inside the finally block is executed regardless of whether an exception was raised or not.

### Things I want to know more about
1. Advanced exception handling techniques in Python
2. FileIO with binary files


