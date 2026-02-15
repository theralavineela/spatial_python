# **Python Basics**
**Values**

*   A value is the fundamental thing that a program manipulates
*   Values can be ‘Hello Python’, 1 , True
Values have types.

# **Variable**
1.   One of the most basic and powerful concepts is
that of a variable.
2.   A variable assigns a name to a value.
Variables are nothing more than reserved memory locations that store values.
3. Python variables does not need explicit declaration to reserve memory.
4.Unlike C/C++ and Java, variables can change types



```python
message = 'Hello Python!'
```


```python
type(message)
```




    str



# **Data Types**


### 1.   Numeric Types


*   Integer Types: 92, 12, 0, 1
*   Floats (Floating point numbers): 3.1415
*   Complex Numbers: a + b*i (composed of real and imaginary component, both of which are floats a + b*i)
*   Booleans: True/False are a subtype of integers (0 is false, 1 is true)

2.   Strings
*   ‘Hello Python’
*  'India'

3.  Sequence types:


*   Lists : [1,2,3,4,5]
*   Tuples: (1, 2)
*   Ranges:


```python
x = 1         # assign variable x the value 1
y = x + 5     # assign variable y the value of x plus 5
z = y         # assign variable z the value of y
a = 10.5      # assign variable a the value of 10.5 float
b = True      # assign variable b the value True boolean
x = 10.5

print(type(x))
```

    <class 'float'>
    


```python

x = 'Hello'
print(type(x))
```

    <class 'str'>
    


```python
name = 'Python'

name_1 = 'Python1'
```


```python
1Name = 'Python'
```


      Cell In[6], line 1
        1Name = 'Python'
        ^
    SyntaxError: invalid decimal literal
    



```python
def  = 10

```


      Cell In[7], line 1
        def  = 10
             ^
    SyntaxError: invalid syntax
    



```python
x = 1       # integer
x = 1.0     # decimal (floating point)
x = 10
print(type(x)) # outputs: <class 'int'>


```

    <class 'int'>
    


```python
x = 10.0
print(type(x)) # outputs: <class 'float'>
x = True

print(type(x))

y = False

print(type(y))

```

    <class 'float'>
    <class 'bool'>
    <class 'bool'>
    


```python
x = 'This is a string'
print(x) # outputs: This is a string
print(type(x)) # outputs: <class 'str'>
y = "This is also a string"
x = 'Hello' + ' ' + 'World!'
print(x) # outputs: Hello World!

```

    This is a string
    <class 'str'>
    Hello World!
    


```python
planets_in_solar_system = 8 # int, pluto used to be the 9th planet, but is too small
distance_to_alpha_centauri = 4.367 # float, lightyears
can_liftoff = True
shuttle_landed_on_the_moon = "Apollo 11" #string
```

# **Modules**


1.   module is a file containing Python definitions and statements
2.   not all functionality available comes automatically when starting Python
1.   extra functionality can be added by importing modules
1.   objects in the module can be accessed  by prefixing them with the module name



```python
import math
```


```python
math.pow(2, 5)
```




    32.0




```python
import random
```


```python
random.randint(1, 70)
```




    65




```python
from pathlib import Path
```

Comments Start with a `#`


```python
# This is a comment
```

**Putting All things together**

---


Now we will write a program to calculate Simple Intrest


```python
rate = 10
```


```python
principle = 1000
```


```python
time = 3
```


```python
intrest = (rate * principle * time)/100
```


```python
print('Intrest is ', intrest)
```

    Intrest is  300.0
    

## Operations


```python
answer = 30 + 12
print(answer)

# Output: 42
```

    42
    


```python
difference = 30 - 12
print(difference)
```

    18
    


```python
product = 30 * 12
print(product)
```

    360
    


```python
quotient = 30 / 12
print(quotient)
```

    2.5
    


```python
seconds = 1042
display_minutes = 1042 // 60
print(display_minutes)

```

    17
    


```python
seconds = 1042
display_minutes = 1042 // 60
display_seconds = 1042 % 60

print(display_minutes)
print(display_seconds)


```

    17
    22
    


```python
endVelocity = 60
startVelocity = 0
acceleration = 9.8

time = (endVelocity - startVelocity) / acceleration
print("Time to reach desired velocity = ", time)
```

    Time to reach desired velocity =  6.122448979591836
    

# **Indentation**
1.  In Python, blocks of code are defined using indentation
1.  The indentation within the block needs to be consistent
1.  The first line with less indentation is outside of the block
1.  The first line with more indentation starts a nested block
1.  Often a colon appears at the start of a new block

## Conditionals


```python
x = 12
if x<10:
    print('x is less than 10')
    print('H## Conditional Statements

```


      Cell In[30], line 4
        print('H## Conditional Statements
              ^
    SyntaxError: unterminated string literal (detected at line 4)
    



```python
a = 97
b = 55

# test expression
if a < b:
    # statement to be run
    print(b)

```


```python
a = 24
b = 44

if a <= 0:
    print(a)
print(b)

```

    44
    


```python
a = 93
b = 27
if a >= b:
    print(a)
else:
    print(b)

```

    93
    


```python
a = 93
b = 27
if a >= b:
    print("a is greater than or equal to b")
elif a == b:
    print("a is equal to b")

```

    a is greater than or equal to b
    


```python
a = 93
b = 27
if a > b:
    print("a is greater than b")
elif a < b:
    print("a is less than b")
else:
    print ("a is equal to b")

```

    a is greater than b
    


```python
a = 16
b = 25
c = 27
if a > b:
    if b > c:
        print ("a is greater than b and b is greater than c")
    else:
        print ("a is greater than b and less than c")
elif a == b:
    print ("a is equal to b")
else:
    print ("a is less than b")

```

    a is less than b
    

## `and` and `or` operators


```python
a = 23
b = 34
if a == 34 or b == 34:
    print(a + b)

```

    57
    


```python
a = 23
b = 34
if a == 34 and b == 34:
    print (a + b)
```

# **Strings**

*   Strings are text values like ‘Hello Anaconda’
*   Strings can be enclosed in single quote ‘ ..’ or double quotes “…”




```python
moon_radius = "The Moon has a radius of 1,080 miles"
```


```python
print(moon_radius)
```

    The Moon has a radius of 1,080 miles
    


```python
fact = 'The "near side" is the part of the Moon that faces the Earth'
```


```python
print(fact)
```

    The "near side" is the part of the Moon that faces the Earth
    


```python
 multiline = """Facts about the Moon:
             There is no atmosphere.
             There is no sound."""
```


```python
print(multiline)
```

    Facts about the Moon:
                There is no atmosphere.
                There is no sound.
    


```python
"Moon" in "This text will describe facts and challenges with space travel"
```




    False




```python
"Moon" in "This text will describe facts about the Moon"
```




    True




```python
temperatures = """Saturn has a daytime temperature of -170 degrees Celsius,
                  while Mars has -28 Celsius."""
```


```python
temperatures.find("Moon")
```




    -1




```python
temperatures.find("Mars")
```




    82




```python
temperatures.count("Mars")
```




    1




```python
temperatures.count("Moon")
```




    0




```python
"The Moon And The Earth".lower()
```




    'the moon and the earth'



Strings can be *indexed* (subscripted), with the first character having index 0.


```python
 word = 'Python'
```


```python
word[0]
```




    'P'




```python
word[5]
```




    'n'



indices may also be negative numbers, to start counting from the right.


```python
word[-1]  # last character
```




    'n'




```python
word[-2]  # second-last character
```




    'o'



In addition to indexing, slicing is also supported. While indexing is used to obtain individual characters, slicing allows you to obtain substring:


```python
 word[0:2]  # characters from position 0 (included) to 2 (excluded)
```




    'Py'




```python
word[2:5]  # characters from position 2 (included) to 5 (excluded)
```




    'tho'




```python
text = 'Put several strings within parentheses '+\
        'to have them joined together.'
```


```python
text
```




    'Put several strings within parentheses to have them joined together.'



# **Lists**
1.  ordered sequence of information, accessible by index
1.  a list is denoted by square brackets, [ ]
1.  a list contains usually homogenous elements
1.  list elements can be changed so a list is mutable



```python
planets = ["Mercury", "Venus", "Earth", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune"]
```


```python
print("The first planet is", planets[0])
print("The second planet is", planets[1])
print("The third planet is", planets[2])

```

    The first planet is Mercury
    The second planet is Venus
    The third planet is Earth
    


```python
planets[3] = "Red Planet"
print("Mars is also known as", planets[3])
```

    Mars is also known as Red Planet
    


```python
number_of_planets = len(planets)
print("There are", number_of_planets, "planets in the solar system.")
```

    There are 8 planets in the solar system.
    


```python
planets.append("Pluto")
number_of_planets = len(planets)
print("There are actually", number_of_planets, "planets in the solar system.")
```

    There are actually 9 planets in the solar system.
    


```python
planets.pop()  # Goodbye, Pluto
number_of_planets = len(planets)
print("No, there are definitely", number_of_planets, "planets in the solar system.")
```

    No, there are definitely 8 planets in the solar system.
    


```python
planets = ["Mercury", "Venus", "Earth", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune"]
```


```python
print("The first planet is", planets[0])
```

    The first planet is Mercury
    


```python
print("The last planet is", planets[-1])
print("The penultimate planet is", planets[-2])

```

    The last planet is Neptune
    The penultimate planet is Uranus
    


```python
jupiter_index = planets.index("Jupiter")
print("Jupiter is the", jupiter_index + 1, "planet from the sun")
```

    Jupiter is the 5 planet from the sun
    


```python
#The following code creates a list that shows the gravitational forces of all eight planets in the solar system, in G:
gravity_on_planets = [0.378, 0.907, 1, 0.377, 2.36, 0.916, 0.889, 1.12]

#In this list, gravity_on_planets[0] is the gravity on Mercury (0.378 G), gravity_on_planets[1] is the gravity on Venus (0.907 G), and so on
```


```python
bus_weight = 12650 # in kilograms, on Earth

print("On Earth, a double-decker bus weighs", bus_weight, "kg")
print("On Mercury, a double-decker bus weighs", bus_weight * gravity_on_planets[0], "kg")

```

    On Earth, a double-decker bus weighs 12650 kg
    On Mercury, a double-decker bus weighs 4781.7 kg
    


```python
bus_weight = 12650 # in kilograms, on Earth

print("On Earth, a double-decker bus weighs", bus_weight, "kg")
print("The lightest a bus would be in the solar system is", bus_weight * min(gravity_on_planets), "kg")
print("The heaviest a bus would be in the solar system is", bus_weight * max(gravity_on_planets), "kg")

```

    On Earth, a double-decker bus weighs 12650 kg
    The lightest a bus would be in the solar system is 4769.05 kg
    The heaviest a bus would be in the solar system is 29854.0 kg
    


```python
planets = ["Mercury", "Venus", "Earth", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune"]
planets_before_earth = planets[0:2]
print(planets_before_earth)
```

    ['Mercury', 'Venus']
    


```python
planets_after_earth = planets[3:8]
print(planets_after_earth)
```

    ['Mars', 'Jupiter', 'Saturn', 'Uranus', 'Neptune']
    


```python
planets_after_earth = planets[3:]
print(planets_after_earth)
```

    ['Mars', 'Jupiter', 'Saturn', 'Uranus', 'Neptune']
    


```python
amalthea_group = ["Metis", "Adrastea", "Amalthea", "Thebe"]
galilean_moons = ["Io", "Europa", "Ganymede", "Callisto"]

regular_satellite_moons = amalthea_group + galilean_moons
print("The regular satellite moons of Jupiter are", regular_satellite_moons)
```

    The regular satellite moons of Jupiter are ['Metis', 'Adrastea', 'Amalthea', 'Thebe', 'Io', 'Europa', 'Ganymede', 'Callisto']
    


```python
regular_satellite_moons.sort()
print("The regular satellite moons of Jupiter are", regular_satellite_moons)
```

    The regular satellite moons of Jupiter are ['Adrastea', 'Amalthea', 'Callisto', 'Europa', 'Ganymede', 'Io', 'Metis', 'Thebe']
    


```python
regular_satellite_moons.sort(reverse=True)
print("The regular satellite moons of Jupiter are", regular_satellite_moons)
```

    The regular satellite moons of Jupiter are ['Thebe', 'Metis', 'Io', 'Ganymede', 'Europa', 'Callisto', 'Amalthea', 'Adrastea']
    

# **Tuple**
1.  tuple consists of a number of values separated by commas
1.  cannot change element values, immutable
1.  tuples always enclosed in parenthesis  
1.  used to return more than one value from a function



```python
t = 12345, 54321, 'hello!'
```


```python
t
```




    (12345, 54321, 'hello!')




```python
t[0]
```




    12345




```python
u = t, (1, 2, 3, 4, 5) # Tuples may be nested:
```


```python
u
```




    ((12345, 54321, 'hello!'), (1, 2, 3, 4, 5))




```python
t[0] = 88888 # Tuples are immutable:
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[90], line 1
    ----> 1 t[0] = 88888
    

    TypeError: 'tuple' object does not support item assignment



```python
x, y, z = t
print(x)
print(y)
print(z)
```

    12345
    54321
    hello!
    

# **Sets**
1.  A set is an unordered collection with no duplicate elements
1.  set objects also support mathematical operations like union, intersection, difference, and symmetric difference



```python
basket = {'apple', 'orange', 'apple', 'pear', 'orange', 'banana'}
```


```python
basket_l = ['apple', 'orange', 'apple', 'pear', 'orange', 'banana']
```


```python
print(basket)# show that duplicates have been removed
```

    {'apple', 'banana', 'pear', 'orange'}
    


```python
'orange' in basket                 # fast membership testing
```




    True




```python
'crabgrass' in basket
```




    False




```python
a = set('abracadabra')
b = set('alacazam')
```


```python
a - b
```




    {'b', 'd', 'r'}



# **Dictionary**
1.  dictionary is a set of key:value pairs
1.  dictionaries are indexed by keys, which can be any immutable type
1.  dictionary stores a value with some key and extracts the value given the key


```python
telephone = {'jack': 4098, 'sape': 4139,'alpha':1099,'beta':1000}
telephone
```




    {'jack': 4098, 'sape': 4139, 'alpha': 1099, 'beta': 1000}




```python
telephone['jack']
```




    4098




```python
telephone['king'] = 4127
telephone
```




    {'jack': 4098, 'sape': 4139, 'alpha': 1099, 'beta': 1000, 'king': 4127}




```python
del telephone['sape']
```


```python
telephone
```




    {'jack': 4098, 'alpha': 1099, 'beta': 1000, 'king': 4127}




```python
'queen' in telephone
```




    False



## While and For Loops


```python
user_input = ''

while user_input.lower() != 'done':
    user_input = input('Enter a new value, or done when done')
```

    Enter a new value, or done when done hi
    Enter a new value, or done when done hello
    Enter a new value, or done when done done
    


```python
# Create the variable for user input
user_input = ''
# Create the list to store the values
inputs = []

# The while loop
while user_input.lower() != 'done':
    # Check if there's a value in user_input
    if user_input:
        # Store the value in the list
        inputs.append(user_input)
    # Prompt for a new value
    user_input = input('Enter a new value, or done when done')
```

    Enter a new value, or done when done 1
    Enter a new value, or done when done 2
    Enter a new value, or done when done 3
    Enter a new value, or done when done done
    


```python
countdown = [4, 3, 2, 1, 0]
for number in countdown:
    print(number)
print("Blast off!! 🚀")
```

    4
    3
    2
    1
    0
    Blast off!! 🚀
    


```python
from time import sleep

countdown = [4, 3, 2, 1, 0]

for number in countdown:
    print(number)
    sleep(1)  # Wait 1 second
print("Blast off!! 🚀")
```

    4
    3
    2
    1
    0
    Blast off!! 🚀
    

### To iterate over a sequence of numbers, the built-in function range() comes in handy.


```python
for i in range(5):
    print(i,end=',')
```

    0,1,2,3,4,


```python
for i in range(5,10):
    print(i,end=',')
```

    5,6,7,8,9,


```python
for i in range(5,10,2):
    print(i,end=',')
```

    5,7,9,

# **break  and continue Statements**
1.  break statement breaks out of innermost enclosing for or while loop.
1.  continue statement continues with the next iteration of the loop skipping remaining statements.



```python
for i in range(50):
    if i==4:
        break
    print(i)
```

    0
    1
    2
    3
    


```python
for i in range(5):
    if i==2:
        continue
    print(i)
```

    0
    1
    3
    4
    

# **Write and call/invoke a function**
If its find that  the same bits of code is reused over and over, you can create your own function and call that instead of         repeating the same code.


```python
def rocket_parts():
    print("payload, propellant, structure")
```


```python
output = rocket_parts()
output is None

```

    payload, propellant, structure
    




    True




```python
def distance_from_earth(destination):
    if destination == "Moon":
        return "238,855"
    else:
        return "Unable to compute to that destination"
```


```python
distance_from_earth()
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[122], line 1
    ----> 1 distance_from_earth()
    

    TypeError: distance_from_earth() missing 1 required positional argument: 'destination'



```python
distance_from_earth("Moon")
```




    '238,855'




```python
def days_to_complete(distance, speed):
    hours = distance/speed
    return hours/24
```


```python
days_to_complete(238855, 90)
```




    110.58101851851852



# **Default Value Argument**


```python
def calc_intrest(principal,rates=5,duration=5):
    intrest=(principal*rates*duration)/100
    amount=intrest+principal
    print('Principal Amount=',principal)
    print('Rate=',rates)
    print('Duration=',duration)
    print('Total Amount=',amount)
```


```python
calc_intrest(10)
```

    Principal Amount= 10
    Rate= 5
    Duration= 5
    Total Amount= 12.5
    


```python
calc_intrest(10,rates=10)
```

    Principal Amount= 10
    Rate= 10
    Duration= 5
    Total Amount= 15.0
    


```python
calc_intrest(10,rates=10,duration=20)
```

    Principal Amount= 10
    Rate= 10
    Duration= 20
    Total Amount= 30.0
    

# Reading File


```python
f = open(r'work.txt','r')

lines = f.read() # Entire file is read
print(lines)
f.close()
```


    ---------------------------------------------------------------------------

    FileNotFoundError                         Traceback (most recent call last)

    Cell In[131], line 1
    ----> 1 f = open(r'work.txt','r')
          3 lines = f.read() # Entire file is read
          4 print(lines)
    

    File ~\anaconda3\Lib\site-packages\IPython\core\interactiveshell.py:324, in _modified_open(file, *args, **kwargs)
        317 if file in {0, 1, 2}:
        318     raise ValueError(
        319         f"IPython won't let you open fd={file} by default "
        320         "as it is likely to crash IPython. If you know what you are doing, "
        321         "you can use builtins' open."
        322     )
    --> 324 return io_open(file, *args, **kwargs)
    

    FileNotFoundError: [Errno 2] No such file or directory: 'work.txt'



```python
f = open(r'd:\work.txt','r')
for line in f:
    print(line)
f.close()
```


```python
with open(r'd:\work.txt','r')as f:
    for line in f:
        print(line,end='')
```

# Writing to file


```python
value = ('the answer is ', 42)
with open(r'd:\workfile2.txt','w') as f:
    s=str(value)
    f.write(s)
```

## Thank You


