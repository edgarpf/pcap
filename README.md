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
* Special attributes of the classes:
  * `__name__` - the class name
  * `__module__` - the name of the module in which the class was defined
  * `__dict__` - the dictionary containing the class’s namespace
  * `__bases__` - a  tuple containing the base classes, in the order of their occurrence in the base class list
  * `__dict__` - the dictionary containing the class’s namespace
  * `__annotations__` - a dictionary containing variable annotations collected during class body execution.
* `[*list1, *list2]` - combine two lists.
* The `__init__.py` files are required to make Python treat directories containing the file as packages.
* Both are correct:
    ```python
    import os
    import sys
    ```
    ```python
    import os, sys
    ```
* Both are incorrect:
    ```python
    from python import os
    from python import sys
    ```
    ```python
    from python import os, sys
    ```
* `isinstance(object, classinfo)` - return True if the object argument is an instance of the classinfo argument.
* Note the `increment_age` method.
    ```python
    class Pet:
        def __init__(self, name, age):
            self.name = name
            self.age = age
        def increment_age(self):
            self.age += 1
    ```
* `hasattr(object, name)` - the arguments are an object and a string. The result is True if the string is the name of one of the object’s attributes, False if not.
* `pip show` - Show information about one or more installed packages. The output is in RFC-compliant mail header format.
* `str.splitlines(keepends=False)` - returns a list of the lines in the string, breaking at line boundaries.
* Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language and first released it in 1991 as Python 0.9.0.
* List than contains None value can not be sorted.
* Using the code:
    ```python
    from machine_learning import classification_report
    ```
    you can use:
    ```python
    classification_report()
    ```
* Python 3.6 introduced underscores in numeric literals, which allows you to place single underscores between numbers and after base specifiers to improve readability. This feature is not available in older Python versions.
* Yield expressions and statements are only used when defining a generator function, and are only used in the body of the generator function. 
* `NameError` is raised when a local or global name is not found. 
* PSF - Python Software Foundation.
* Python’s default arguments are evaluated once when the function is defined, not each time the function is called.
* The following declarations are valid:
    ```python
    a, b = 'a', 'b'
    a = 'a'; b = 'b'
    ```
* `repr(object)` - return a string containing a printable representation of an object.
* The following code is valid:
    ```python
    try:
        import my_package
    except ModuleNotFoundError as err:
        print(err)
    ```
* Break ouside loop will raise a SyntaxError exception.
* All the declarations are valid:
    ```python
    stocks1 = ('AAPL',)
    stocks2 = tuple(['AAPL'])
    stocks3 = 'AAPL',
    ```
* In Python, all exceptions must be instances of a class that derives from `BaseException`.
* `str.strip([chars])` - returns a copy of the string with the leading and trailing characters removed.
* `str.rstrip([chars])` - returns a copy of the string with trailing characters removed. 
* `str.lstrip([chars])` - returns a copy of the string with leading characters removed.
* How to delete the code:
    ```python
    course_name = 'python interview'
    ```
    ```python
    del course_name
    del globals()['course_name']
    del(course_name)
    ```
* The `pass` statement does nothing. It can be used when a statement is required syntactically but the program requires no action.
* `hasattr(object, name)` - the arguments are an object and a string. The result is True if the string is the name of one of the object’s attributes, False if not.
* Multiline strings, which occupy more than one line of source code are delimited by trigraphs:
  * '''
  * """
* List comprehensions provide a concise way to create lists.
* `pip uninstall` - Uninstall packages. pip is able to uninstall most installed packages.
* Dictionaries keep the insertion order since Python 3.7 or higher.
* The right argument of the % operator can not be zero.
* `issubclass(class, classinfo)` - return True if class is a subclass (direct, indirect, or virtual) of classinfo.
* An except clause may name multiple exceptions as a parenthesized tuple, for example: 
    ```python
    except (RuntimeError, TypeError, NameError):
        pass
    ```
* When iterating over a dictionary, we iterate over its keys by default.
* `id(object)` - return the “identity” of an object.
* `numbers[:]` is a copy of `numbers = [1, 2,3]`
* `True + True + 2 * True - False` = 4
* There is no `switch` statement in Python.
* `object.__new__(cls[, ...])` - called to create a new instance of class cls.
* `filter(function, iterable)` - constructs an iterator from those elements of iterable for which function returns true. 
* **ZeroDivisionError** is raised when the second argument of a division or modulo operation is zero. 
* List slicing: list[start:stop:step]
* `pip freeze` - outputs installed packages in requirements format. Packages are listed in a case-insensitive sorted order.
* 

