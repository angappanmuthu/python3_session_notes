# Python3
## What is Python ?

* Python is a popular programming language. It was created by Guido van Rossum, and released in 1991.

## Applications
- Web Development
- Software Development
- Mathematics
- System Scriping
- Mobile Application 
- AI/ML/DL
- Computer Vision 
- Data Science
- Internet of Things (IoT)

## Why Python ?

- Python not platform dependent (Windows, Linux, Mac)
- Simple Syntax.
- It is the interpreter system which means easy to execute and debug the code.
- This is the Object Oriented Programming Language (Solve the problem with real life scenario)

## Python3 Installation
- To install Python3 in Windows [Download](https://www.python.org/downloads/)
![python3](https://sites.pitt.edu/~naraehan/python3/img/win-install-2.png)
- For linux and mac (It has python3 pre-installed)

## Verifiy Installation

```bash
python3 --version
```
- if error raises in mac or linux you should install : -
- For Linux :
```bash
sudo apt-get install python3.8
```
- For Mac : [brew](https://brew.shx) required to install python3
```bash
brew install python@3.8
```

## Open Python3 shell

```bash
python3 
```
(or)
```bash
python
```
(or) 
```bash
py
```
![python3 shell](https://media.geeksforgeeks.org/wp-content/uploads/20191211195520/Run-a-Python-Script-in-interactive-mode-GfG.png)

## Creating Project Workspace

```bash
mkdir python_project/
cd python_project/
touch main.py
```

## Variable

-  A variable is a value that can change, depending on conditions or on information passed to the program.

## Defining Variable and rules

1) It should not start with number.
2) It might be alphanumeric.
3) Special characters is not allow except underscore.
4) Variable name with space in not allowed.

```python
# Syntax
# [variable_name] = [value]
var1 = 10
```

## Datatypes

1. Text Type:	str
2. Numeric Types:	int, float, complex
3. Sequence Types:	list, tuple, range
4. Mapping Type:	dict
5. Set Types:	set, frozenset
6. Boolean Type:	bool
7. Binary Types:	bytes, bytearray, memoryview
8. None Type:	NoneType

### **Numeric Types**

Example:

```python
x = 1    # int
y = 2.8  # float
z = 1j   # complex
```


### **Text Type or String**

Example:

```python
print("Hello")
print('Hello')
```


### **Boolean Type or Binary**

Example:

```python
a = True
print(a)
print(10 > 9)
```

### List in Python

- A list in a sequence datatype in python that enable heterogeneous elements rather than other programming language. It is mutable datatype.

```python
arr = [1,2.5,'h',True]
arr2 = [2.2,3.5,5.6,7.8]
```

### Tuple in Python

- Tuples have indexes and Immutable datatype, which is used to defining static array values.

```python
size = (50,50)
image_size = (50,50,1)
```

### Set in Python

- Sets are unchangable, unindexed datatype and never allow any dublicate values.

```python
thisset = {"apple", "banana", "cherry", "apple"}

print(thisset)
```

### Dict in Python

- Dictionaries are used to store data values in key:value pairs.

- A dictionary is a collection which is ordered*, changeable and do not allow duplicates.

```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict)
```










