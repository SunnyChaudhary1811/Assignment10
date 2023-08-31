# Assignment10

Q1:-

The try and except blocks in Python are used for managing exceptions or errors in code. The try block contains potentially problematic code, and the except block handles errors that might occur in the try block, preventing crashes and allowing for graceful error handling.

Q2:-


```python
try:
    num = int(input("Enter a number: "))
    result = 10 / num
    print("Result:", result)
except ZeroDivisionError:
    print("Cannot divide by zero.")
except ValueError:
    print("Invalid input. Please enter a number.")

```

    Enter a number: 9
    Result: 1.1111111111111112
    

Q3:-

If an exception occurs inside a try block and there's no matching except block, the exception will propagate up the call stack. If no matching except block is found, the program will terminate, displaying an error message indicating the unhandled exception. It's important to handle exceptions to prevent unexpected program termination.

Q4:-

Using a bare except block catches any exception, making debugging harder and potentially masking errors. Specifying a specific exception type in an except block allows you to handle only intended exceptions, improving error diagnostics and code predictability.

Q5:-


```python
try:
    numerator = int(input("Enter the numerator: "))
    denominator = int(input("Enter the denominator: "))
    
    try:
        result = numerator / denominator
        print("Result:", result)
    except ZeroDivisionError:
        print("Cannot divide by zero.")
except ValueError:
    print("Invalid input. Please enter valid integers.")

```

    Enter the numerator: 45
    Enter the denominator: 34
    Result: 1.3235294117647058
    

Q6:-


```python
try:
    num = int(input("Enter a number: "))
    result = 10 / num
    print("Result:", result)
except ZeroDivisionError:
    print("Cannot divide by zero.")
except ValueError:
    print("Invalid input. Please enter a number.")
except Exception as e:
    print("An error occurred:", e)

```

    Enter a number: 56
    Result: 0.17857142857142858
    

Q7:-

a. EOFError: Raised when there's an unexpected end of file or input while trying to read data.

b. FloatingPointError: Raised when a floating-point operation (like division by zero or invalid result) cannot be performed.

c. IndexError: Raised when trying to access an index that doesn't exist in a sequence, like a list or a string.

d. MemoryError: Raised when an operation cannot be completed due to lack of memory.

e. OverflowError: Raised when an arithmetic operation exceeds the maximum limit of a numeric type.

f. TabError: Raised when inconsistent use of tabs and spaces for indentation is detected in the code.

g. ValueError: Raised when an operation receives an argument of the correct type but with an inappropriate value.









Q8:-


```python
try:
    numerator = int(input("Enter the numerator: "))
    denominator = int(input("Enter the denominator: "))
    result = numerator / denominator
    print("Result:", result)
except ZeroDivisionError:
    print("Cannot divide by zero.")
except ValueError:
    print("Invalid input. Please enter valid integers.")

```

    Enter the numerator: 56
    Enter the denominator: 65
    Result: 0.8615384615384616
    


```python
try:
    string_num = input("Enter a number: ")
    num = int(string_num)
    print("Number:", num)
except ValueError:
    print("Invalid input. Please enter a valid integer.")

    
```

    Enter a number: 56
    Number: 56
    


```python
my_list = [10, 20, 30]
try:
    index = int(input("Enter an index: "))
    element = my_list[index]
    print("Element at index", index, ":", element)
except IndexError:
    print("Index out of range.")
except ValueError:
    print("Invalid input. Please enter a valid integer.")

```

    Enter an index: 6
    Index out of range.
    


```python
try:
    value = int(input("Enter a positive number: "))
    if value < 0:
        raise ValueError("Negative number not allowed.")
    print("Value:", value)
except ValueError as e:
    print("Error:", e)

```

    Enter a positive number: 6
    Value: 6
    


```python
try:
    num = int(input("Enter a number: "))
    result = 10 / num
    print("Result:", result)
except Exception as e:
    print("An error occurred:", e)

```

    Enter a number: 6
    Result: 1.6666666666666667
    


```python

```
