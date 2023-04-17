# Readings: Ten Thousand 2

1. Variable scope in Python refers to the accessibility and visibility of a variable within a program. A variable's scope determines where it can be accessed and modified within a program. Local scope refers to a variable that is defined within a function and is only accessible within that function. Global scope refers to a variable that is defined outside of any function and can be accessed and modified from anywhere in the program.
 Here is an example illustrating the usage of both local and global scopes:
```
# global variable
x = 10

def my_func():
    # local variable
    y = 5
    print("local variable y:", y)

    # accessing global variable
    global x
    x = x + 1
    print("global variable x:", x)

# calling function
my_func()
print("global variable x after function call:", x)

```
In this example, x is a global variable that can be accessed and modified from anywhere in the program, while y is a local variable that can only be accessed within the my_func function.

2. The global keyword in Python is used to modify a variable that is defined outside of a function, making it accessible and modifiable from within the function. The nonlocal keyword is used to modify a variable that is defined in the enclosing function, making it accessible and modifiable from within a nested function. You would use these keywords when you need to modify a variable that is outside the current scope of a function.
For example, consider the following code:
```
x = 0

def outer():
    x = 1

    def inner():
        nonlocal x
        x = 2

    inner()
    print("x in outer:", x)

outer()
print("x outside outer:", x)

```

In this example, x is a variable defined outside the outer function. Inside outer, a local variable with the same name is defined and assigned a value of 1. inner is a nested function that modifies the x variable using the nonlocal keyword. After inner is called, x is now equal to 2 inside outer. Outside outer, the value of x remains unchanged at 0.

3. Big O notation is a way of describing the performance or efficiency of an algorithm by measuring how it scales with respect to the size of the input. The purpose of Big O notation is to give us a way to compare different algorithms and determine which ones are more efficient for large inputs. It is important in the context of algorithm analysis because it allows us to predict how an algorithm will perform as the input size grows, which is important for understanding the scalability and practicality of the algorithm.

4. To simulate a dice roll in Python, we can use the random module, which provides functions for generating random numbers. Here is an example:
```
import random

# simulate a dice roll
roll = random.randint(1, 6)
print("You rolled a", roll)

# calculate probability of rolling a specific number
num_trials = 1000000
count = 0
for i in range(num_trials):
    roll = random.randint(1, 6)
    if roll == 6:
        count += 1

probability = count / num_trials
print("Probability of rolling a 6:", probability)

```
In this example, we use the randint function from the random module to simulate a dice roll. We generate a random integer between 1 and 6, inclusive. To calculate the probability of rolling a specific number (in this case, 6), we use a loop to simulate a large number of
