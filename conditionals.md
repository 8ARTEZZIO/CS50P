```python
x = int(input("What's x? "))
y = int(input("What's y? "))

if x < y:
  print("x is less than y")
elif x > y:
  print("x is more than y")
else:
  print("x is equal to y")
```

![alt text](https://www.trytoprogram.com/images/python_ifelseif.jpg "Flowchart")

```python
def main():
  x = int(input("What's x? "))
    if is_even(x):
      print("Even")
    else:
      print("Odd")

def is_even(n):
  return n % 2 == 0

main()
```
```python
name = input("What's your name? ")

match name:
  case "Harry" | "Hermione" | "Ron":
    print("Gryffindor")
  case "Draco":
    print("Slytherin")
  case _:
    print("Who?")
```
