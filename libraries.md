## Random ##
[Random Module](docs.python.org/3/library/random.html)

import - allows you to import from some module in python

e.g.
random.choice(seq)

```python
import random

coin = random.choice(["heads", "tails"])
print(coin)
```

OR

```python
from random import choice 

coin = choice(["heads", "tails"])
print(coin)
```

### Randint ###

```python
from random import randint

number = randint(1, 10)
print(number)
```

# Shuffle

```python
import random

deck = ["jack", "queen", "king"]
random.shuffle(deck)

for card in deck:
    print(card)
```

## Statistics ##
[Statistics Module](docs.python.org/3/library/statistics.html)

```python
import statistics

print(statistics.mean([100, 90]))
```

## Command-line arguments ##

```python
import sys

try:
    print("hello, my name is", sys.argv[1])
except IndexError:
    print("Too few argument")
```

To Provide More REFINED response

```python
import sys

if (len.argv) < 2:
    print("Too few arguments")
elif len(sys.argv) >2:
    print("Too many arguments")
else:
    print("hello, my name is", sys.argv[1])
```

Too have a slice of sys.argv:

```python
import sys

if (len.argv) < 2:
    sys.exit("Too few arguments")

for arg in sys.argv[1:]:
    print("hello, my name is", arg)
```

## Packages ##

### PyPi ##

[pypi.org](pypi.org)

### cowsay ###

[for curious](pypi.org/project/cowsay)

### pip ###

Allows you to install all the packages from a command line in terminal.

e.g.

```python
pip install cowsay
```
```python
import cowsay
import sys

if len(sys.argv) == 2:
    cowsay.cow("hello, " + sys.argv[1])
```

## APIs ##

### requests ###

[Python Requests](docs.python-requests.org)

```python
pip install requests
```

## JSON - Javascript Object Notation ##

How to read JSON file in python

```python
import sys
import requests
import json

if len(sys.argv) != 2:
    sys.exit()

response = requests.get("https://itunes.apple.com/search?entity=song&limit=1&term=" + sys.argv[1])
print(json.dumps(response.json(), indent=2))
```










