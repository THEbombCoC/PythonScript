## Operation on Tuple

### 1.Concatenating 2 tuples

Example:
```python
tupl1=(1, 3) 
tupl2=("red","green") 

tupl3=tupl1+tupl2
print(tupl3) 
```
Output:
```
(1, 3,"red", "green") 
```

### 2.Nested tuple 

Example:
```python
tupl1=(1, 3) 
tupl2=["red","green"]

tupl3=(tupl1,tupl2) 
print(tupl3) 
```
Output:
```
((1, 3),["red", "green"]) 
```

### 3. Change Tuple value 

- unlike a list, a tuple is immutable objects. This means that the element of a tuple can not be changed once it has been assigned. 
- but if a tuple contains any mutable object such as a list then this object can be changeable. 

For Example:
```python
mytple=(1,2,3,4,5,["red", "green"]) 
# change 2 element with 9
mytple[1]=9
print(mytple)
````
Output:
```
Error tuple object does not support item assignments
```

But in the same example, you want to replace **"red"** With **"black"**

Example:
```python
mytple=(1,2,3,4,5,["red", "green"])

# change "red"  element with "black"
mytple[5][1]="black"

print(mytple) 
```
Output:
```
(1,2,3,4,5,["black", "green"]) 
```

### 4. Deleting Tuple
- A tuple is an immutable object so we can delete the individual item from the tuple. 
- The entire tuple will be deleted or removed using a del keyword. 

Syntax:
```python
del tuplename
```
Example:
```python
mytple=(1,2,3,4,5,["red", "green"]) 
# delete tuple

del mytple
print(mytple)
```
Output
```
NameError: name 'mytple' is not defined
```


### 5. Counting Frequency of Element
Get the frequency of particular element appears in the tuple.

Synatx:
```python
tuplename.count(element) 
```
Example:
```python
tpl=(3,4,68,3,5,3) 
res=tpl.count(3)
print(res) 
```
Output:
```
3
```

### 6. Find Position index of element.

Get the first index of the specified value. 

Syntax:
```python
tuplename.index(value) 
```
Example:
```python
tpl=(3,4,68,3,5,3,4) 
res=tpl.index(4)
print(res) 
```
Output:
```
1
```

### 7.Check element is present in tuple or not

- **'in'** keyword is used to check whether the element is present in tuple or not
- if the element is present this will return boolean value True otherwise False

Syntax:
```python
Element in tuplename
```
Example:
```python
tpl=(3,4,68)
# check 4 is present or not
if 4 in tpl:
    print("present") 
else:
    print("Not present")
```
Output:
```
present
```
