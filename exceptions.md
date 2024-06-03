## Syntax Error ##
Syntax error has to be fixed manually.
There's no other way to omit this.
Example:
```python
print("Hello World)
```
## Try / Except / Else / Finally ##
```python
try:
    x = int(input("What's x? "))
    print(f"x is {x}")
except ValueError:
    print("x is not an integer")
```
The below code is incorrect:
```python
try:
    x = int(input("What's x? "))
except ValueError:
    print("x is not an integer")
print(f"x is {x}")
```
Instead use 'else' statement:
```python
try:
    x = int(input("What's x? "))
except ValueError:
    print("x is not an integer")
else:
    print(f"x is {x}")
```
We can reprompt the user until a correct answer received:
```python
while True:
    try:
        x = int(input("What's x? "))
    except ValueError:
        print("x is not an integer")
    else:
        break
print(f"x is {x}")
```
Let's add some functions:
```python
def main():
    x = get_int()
    print(f"x is {x}")


def get_int():
    while True:
        try:
            x = int(input("What's x? "))
        except ValueError:
            print("x is not an integer")
        else:
            break


main()
```
Now let's shorten the get_int() func and remove the explicit exception print:
```python
def main():
    x = get_int()
    print(f"x is {x}")


def get_int():
    while True:
        try:
            return int(input("What's x? "))
        except ValueError:
            pass


main()
```
## Debugging ##
In VSC just choose breakpoints and press Run and Debug ( Ctrl + Shift + D )

Step over to move to the next executed line of code.
Step into to search the line being executed in detail.
