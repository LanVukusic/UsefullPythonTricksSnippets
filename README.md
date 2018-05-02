
# UsefullPythonTricksSnippets
A list od trikcs and snippets i find usefull
my cheatsheet: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
***

#### 1. Returns a binary from an int
```python
	'{0:b}'.format(2)
```
Returns 10  
*It strips leading zeros so be carefull*
***

#### 2. Reverses a string
```python
	"hello"[::-1]
```
Returns "olleh".  
*[x:y:z] selects subset where **x** is starting point(inclusive), **y** is ending point (exclusive) and **z** is a step.
if step is negative, the traversial is inverted.*

***

#### 3. Special functions -MAGIC-
*we are in a file named python.py*
```python
	print(__file__)
	print(__name__)
```
Returns:  
"C:/PythonProjects/python.py"  
"\_\_main__" if we are running the script directly, and not calling it as an import for example.  

***

#### 4. Appending to a list
*we have a list called **myList** and a variable **a**, that we wuld like to add to a list*
```python
	myList = [1, 2, 3, 4, 5]
	a = 6

	myList.append(a) # If we would like to add it to the end, we would do it like that*	
	myList.insert(0, a) # If we would like to insert it to the spacific index, we would do it like that*

	myList.remove(2)
	del myList[4]
	print(myList.pop(-1))
```  
 * **.append(x)** adds element **x** to the end of the list. In that case **[1, 2, 3, 4, 5, 6]**.
 * **.insert(x,y)** adds element **x** to the **y** index of the list. In that case **[6, 1, 2, 3, 4, 5]**.

* **.remove(x)** removes the first **x** in list. In that case, it would return **[1, 3, 1, 2, 3]**.   

* **del** removes the element at spacific index. in that case, it would return **[1, 2, 3, 1, 3]** 

* **.pop(x)** is basically same as remove, but it returns the poped element.   
Returns: 3
***

#### 5. Reverse iteration
*it actually iterates reversely and is not changing the iterative item itself*
```python
	myList = [1, 2, 3, 4, 5]
	for i in range(len(myList)-1, -1, -1):
		print(myList[i])
``` 
Prints: 5 4 3 2 1
***  
#### 6. Christmas tree with format
```python
	for i in range (1, 10, 2):
    		print("{:-^20}".format("X"*i))
``` 
Prints:  
---------X----------  
--------XXX---------  
-------XXXXX--------  
------XXXXXXX-------  
-----XXXXXXXXX------  

#### 7. Library version
```python
	import lalala as a
	print(a.__version__)
``` 
Prints:
1.0.0


