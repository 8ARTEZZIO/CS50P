While loop:
```python
i = 0
while i < 3:
    print("meow")
    i += 1
```
For loop:
```python
for _ in range(3):
    print("meow")
```
Or alternatively:
```python
print("meow\n" * 3, end="")
```
```python
def main():
    number = get_number()
    meow(3)

def get_number():
    while True:
        n = int(input("What's n? "))
        if n > 0:
            return n

def meow(n):
    for _ in range(n):
        print("meow")

main()
```

