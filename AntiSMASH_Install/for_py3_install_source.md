For python 3, several utility library are reconfigured and thus python 2 users need to be aware of syntax and import issues.
In the folder, a download_database.py for python 3 users are included. 
For your information, here's the major changes from python 2, in case of future modifications, please refer to the following 
syntax. 

#Python 2

```python
print 'Python', python_version()
print 'Hello, World!'
print('Hello, World!')
print "text", ; print 'print more text on the same line'
```

```
Python 2.7.6
Hello, World!
Hello, World!
text print more text on the same line
```
#Python 3


```python
print('Python', python_version())
print('Hello, World!')
print("some text,", end="")
print(' print more text on the same line')
```
```
Python 3.4.1
Hello, World!
some text, print more text on the same line
```
```python
print 'Hello, World!'
```
Note that when trying Python2 syntax, a SyntaxError would be reported

```
  File "<ipython-input-3-139a7c5835bd>", line 1
    print 'Hello, World!'
                        ^
SyntaxError: invalid syntax
```


