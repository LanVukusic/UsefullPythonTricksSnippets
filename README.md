
# UsefullPythonTricksSnippets
A list od trikcs and snippets i find usefull
my cheatsheet: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
***

#### 1. Returns a binary from an int
```python
	'{0:b}'.format(2)
```
returns 10  
*It strips leading zeros so be carefull*
***

#### 2. Reverses a string
```python
	"hello"[::-1]
```
returns "olleh".  
*[x:y:z] selects subset where **x** is starting point(inclusive), **y** is ending point (exclusive) and **z** is a step.
if step is negative, the traversial is inverted.*

***

#### 3. Special functions -MAGIC-
*we are in a file named python.py*
```python
	print(__file__)
	print(__name__)
```
returns:  
"C:/PythonProjects/python.py"  
"\_\_main__" if we are running the script directly, and not calling it as an import for example.  

***
