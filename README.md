# PCAP

* Use of ***imports***
    ```python
    import pandas as pd
    from pandas import DataFrame as Frame
    ```
* Importing a module is done by an instruction named ***import***.
* A module is identified by its name.
* Each module consistis of entities (functions, variables, constants, classes and objects).
* Given the function:
    ```python
    def add(a, b):
        result = a + b
        return 
    ```
    The call ***add(3, 5)*** will result in ***None***.
* LEGB is the rule by which Python resolves names. The letters in LEGB stand for Local, Enclosing, Global and Built-in scope.
* The code:
    ```python
    from builtins import sum
    
    
    print(sum([4, 6]))
    
    
    def sum(iterable):
        result = 0
        for item in iterable:
            result += item * 2
        return result
    
    
    print(sum([4, 6]))
    ```
    will result in: <br>
    10 <br>
    20
* ***KeyError*** is raised when a mapping (dictionary) key is not found in the set of existing keys.
* `','.join(list_name)` returns a string which is the concatenation of the strings of list_name.
* ***Method Resolution Order (MRO)*** is the order in which base classes are searched for a member during lookup.
* ***list.index(x[, start[, end]])*** - return zero-based index in the list of the first item whose value is equal to x. Raises a ValueError if there is no such item. 
* The following dictionaries are given:
    ```python
    stocks_1 = {'MSFT': 280.0, 'AAPL': 146.39, 'TSLA': 644.22}
    stocks_2 = {'AMZN': 3573.0, 'NVDA': 726.44}
    ```
    You can combine them with:
    ```
    stocks_1 | stocks2 
    stocks_1.update(stocks2) 
    {**stocks_1, **stocks2}
    ```
* ***help([object])*** - invokes the built-in help system.
* Convert a list to a set and back to a list again to remove duplicates from the list.
* The try/except statement specifies exception handlers and/or cleanup code for a group of statements.
* A docstring is a string literal that occurs as the first statement in a module, function, class, or method definition. Such a docstring becomes the `__doc__` special attribute of that object.
* The following reverse list:
    ```
    [IN]: numbers = list(range(10, 100, 10))
    [IN]: numbers[::-1]
    [OUT]: [90, 80, 70, 60, 50, 40, 30, 20, 10]
    ```
* The following reverse list and return every second element:
    ```
    [IN]: numbers = list(range(10, 100, 10)) <br>
    [IN]: numbers[::-2] <br>
    [OUT]: [90, 70, 50, 30, 10] 
    ```
* Variable name cannot start with a digit.
* Space character is not allowed in a variable name
* The following code will result in **data not received**
    ```python
    data_stream = ''
    while data_stream:
        print('data received')
    else:
        print('data not received')
    ```
* Python is a high level programming language.
* Protected members of a class are accessible from within the class and are also available to its sub-classes. No other environment is permitted access to it. This enables specific resources of the parent class to be inherited by the child class. Python's convention to make an instance variable protected is to add a prefix `_` (single underscore) to it.
* The meaning of the **keyword argument** is determined by its name specified along with its value.
* **Guido van Rossum** is the creator of Python.
* The following answers will create an empty class
    ```python
    class Company(object):
        pass
    ```
    ```python
    class Company: pass
    ```
    ```python
    class Company:
        pass
    ```
* `pip list` - Lists installed packages, including editables. Packages are listed in a case-insensitive sorted order.
* `pip freeze` - outputs installed packages in requirements format. Packages are listed in a case-insensitive sorted order.
* `bin(x)` - convert an integer number to a binary string prefixed with “0b”.
* Considering `p = Person()` you get class name using `type(p).__name__` and `p.__class__.__name__`.
* `from math import *` is usnafe. You will import all entities from math module.
* `__file__` - the pathname of the file from which the module was loaded, if it was loaded from a file.
* The following code: 
    ```python
        a = [1, 2, 3, 4, 5]
        b = a
        b[:] = [3, 6]
    ```
  will result in:
  ```python
  b = [3, 6]
  a = [3, 6]
  ```
* You only need to add a double underscore __ before the attribute name to make it private.
* Assert statements are a convenient way to insert debugging assertions into a program.
* Function definition must be placed before the first invocation.
* list() is list() is false because there two different lists.
* `str.title()` - return a titlecased version of the string where words start with an uppercase character and the remaining characters are lowercase.
* `from math import sin, exp` - It's correct, but not recommended due to stylistic reasons. It's better and prettier to express the same intention in more a verbose and explicit form using two lines.
* `issubset(other)` or `set <= other` - test whether every element in the set is in other.
* `True` and `and` are reserved words in Python.
* A docstring is a string literal that occurs as the first statement in a module, function, class, or method definition. Such a docstring becomes the `__doc__` special attribute of that object.
* The following commands will check the pip version:
    ```
    pip --version
    python -m pip --version
    py -m pip --version
    ```
