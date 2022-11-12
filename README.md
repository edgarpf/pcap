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
* The code:
    ```python
    input_str = '3.14'
    converted_int_number = int(input_str)
    ```
    will raise **ValueError** exception.
* 0., .0 and 1e6 are float types.
* `iterator` - an object representing a stream of data. Repeated calls to the iterator’s `__next__()` method (or passing it to the built-in function next()) return successive items in the stream. Iterators are required to have an `__iter__()` method that returns the iterator object itself
* `ord(c)` - given a string representing one Unicode character, return an integer representing the Unicode code point of that character.
* Use the **global** to create a global variable from local scope.
* The compiled Python bytecode is stored in files which have their names ending with **pyc**.
* PEP stands for Python Enhancement Proposal. The PEP is a design document that provides information to the Python community or describes a new Python function, its processes, or its environment. It is also a set of rules that determine how Python code is formatted for maximum readability.
* `zip(*iterables, strict=False)` - iterate over several iterables in parallel, producing tuples with an item from each one.
* `sys.version` - a  string containing the version number of the Python interpreter plus additional information on the build number and compiler used.
* `any(iterable)` - return True if any element of the iterable is true. If the iterable is empty, return False.
* `builtins` module provides direct access to all ‘built-in’ identifiers of Python; for example, builtins.open is the full name for the built-in function open().
* Python strings are immutable. 
* A special method (magic method) is a method that is implicitly called by Python to perform a specific operation. For example, such as addition, subtraction, extended assignment, etc. Special methods have names that begin and end with double underscores.
* PEP8 is a document that provides coding conventions and style guide for Python code.
* `importlib.reload(module)` - reloads a previously imported module.
* PyPI is shor for Python Package Index.
* When a Python source file is imported for the first time, a `__pycache__` directory will be created in the package directory, if one does not already exist. 
* You cannot append elements to tuples.
* var = 36e-4 -> 0.0036
* 'python' * False = ''
* var1 is var2 = true if they have the same value.
* When a dictionary is converted to a set using `set()` the result is a set of dictionary keys.
* The `datetime` module supplies classes for manipulating dates and times.
* An infinite recursive function will raise RecursionError exception.
* `class type(name, bases, dict, **kwds)` - with one argument, return the type of an object.
* Conda and Pip are package managers.
* CPython is the default implementation of the Python programming language.
* **Python While Else** - With the else statement we can run a block of code once when the condition no longer is true:
* Python supports functional programming.
* `object.__repr__(self)` - called by the `repr()` built-in function to compute the “official” string representation of an object.
* **SyntaxError** is raised when the parser encounters a syntax error.
* `keyword.kwlist` - sequence containing all the keywords defined for the interpreter.
* **do while** is not available in Python.
* Lambda function has a : as example:
    ```python
    lambda (a,b): True
    ```
* **true** does not exist. **True** is correct.
* `re` module in Python supports regular expressions.
* `10 != '1' + '0'` results in `True`. No exception is raised. 
* The `platform.system()` function returns a string with your OS name, the `platform.version()` function returns a string with your OS version. The `platform.processor()` function returns a string with the name of your processor.
* `os.mkdir("a/b/c/d")` will raise **FileExistsError** if d exists.
* The integer value of `True` is 1.
* If the index is given, `pop()` removes and returns
the element at the given index.
* When there is no `__str__()` method present and you print an object, Python shows the object id in that way.
* `insert(0, 1)` inserts 1 before index 0 (at the front of the list).
* `break` can not be used outside of a loop,
and the default `except` must be last.
* The values that become False in Python are the following:
    ```python
    print(bool(''))        # False
    print(bool(0))         # False
    print(bool(0.0))       # False
    print(bool(0j))        # False
    print(bool(None))      # False
    print(bool([]))        # False
    print(bool(()))        # False
    print(bool({}))        # False
    print(bool(set()))     # False
    print(bool(range(0)))  # False
    ```
* The **Exception** class contains a property named **args** and it is a tuple.
* First use `pip list --outdated` to list your outdated packages. Then use `pip install -U package_name` to update one of the packages.
* The `read()` method reads the whole content of a file and returns it as a string. The `readline()` method only reads one line. The `readlines()` method also reads the whole content but returns it as a list of lines.
* If a variable name shadows into a function you can use it in an expression or you can assign a new value to it BUT you can not do both at the same time.
* The division operator ALWAYS returns a float.
* An imported module is executed only once.
* `range(-1, -2)` has no element.
* If you have instance variables with two leading underscores,
you can not just access them from outside of the class. The code will raise **AttributeError** exception.
* The digraph written as **#!** is used to tell a Unix or Unix-like OS how to execute the contents of a Python file.
* List slicing: [start(inclusive):end(exclusive):step]
* **ZeroDivisionError** is a subclass of **ArithmeticError**.
* **Python Package Index** is also known as the Cheese Shop
* stdin, stdout, stderr are names of pre-opened streams.
* stdout and stderr are associated with the console.
* stdin is associated with the keyboard.
* A list of package's dependencies can be obtained from pip using its command named **show**.
* String literals that are delimited by whitespace are automatically concatenated.
* Lambda functions can have any number of arguments but only one expression.
* `__eq__()` overloads the equal to operator.
* **errno.ENOENT** symbol refers to an error described as No such file or directory.
* None value can not be used as an argument of arithmetic operators.
* `from x.y import z` causes the import of entity z from module y from package x.
* default 'except:' must be last
* A code point is a number which makes up a character.
* `listdir()` never includes the special entries . and ..
* The `math.floor()` method rounds a number DOWN to the nearest integer.
* The `math.ceil()` method rounds a number UP to the nearest integer.
* The `tuple.index()` method expects a value and looks for that value in the tuple. It will return the index of the first value it finds. If it does not find the value, it raises a ValueError.
* The method in Python to immediately terminate a program is `sys.exit()`.
* A string is immutable. You can not change it. You can read something by indexing, BUT you can not write something by indexing.
* A source file named `__init__.py` is used to mark a directory/folder as containing a Python package, and to initialize the package.
* `'' in 'alphabet'` is `True`.
* Pip means Pip Installs Packages.
* The pyc files are created by the Python interpreter when a py file is imported. They contain the compiled bytecode of the imported module.
* Greater than operator and less than operator have the highest precedence. The logical and operator has a higher precedence than the logical or operator.
* Imported files get executed only once.
* The list of possible exceptions has to be in parentheses.
* Every object has the method `__len__()`. Normally we use the function len() which calls the method `__len__()`.
* The folder created by Python used to store **pyc** files is named `__pycache__`.
* The `rfind()` method finds the last occurrence of a specified value.
* The `index()` method finds the first occurrence of a specified value.
* `print('is' in 'This IS Python code.')` is True.
* A string is immutable and if you create two strings with the same value they will both point to the same object and therefore have the same ids.
* In `range(start, end)` The start value has to be lower than the end value. Otherwise range() does not return an element.
* A tuple can be the index of a dictionary.
* Packages can contain modules.
* Since Python 3.4 pip has been included with the Python installer.
* If both operands are an integer the floor division operator will return an integer. If at least one operand is a float the result will also be a float.
* In the list of classes to inherit from a superclass cannot come before its subclass.
* The `dir()` function returns the names of all entities
(properties and methods) of the passed module (or object).
* Dictionary can have different data types as a key.
BUT if an integer and a float have the same value,
the second value overrides the first values.
* The `isdigit()` method checks if all the characters in the string are digits.
* If you try to divide by a string you get a `TypeError`.
* If a class doesn't define its own constructor, the constructor of its superclass is invoked.
* **Error** is not a subclass of **RuntimeError**.
* The code:
    ```python
    def func(data):
        data = [7, 23, 42]
        print('Function scope: ', data)
    
    
    data = ['Peter', 'Paul', 'Mary']
    func(data)
    print('Outer scope: ', data)
    ```
    will print:
    ```
    Function scope: [7, 23, 42]
    'Outer scope: ['Peter', 'Paul', 'Mary']
    ```
* The `read()` method has one optional parameter.
If it is given, that number of characters are read.
* There is no increment operator ++ in Python.
You can add as many plus signs as you like, the number stays positive.
* The output of the code:
    ```python
    for i in range(1):
        print('*')
    else:
        print('*')
    ```
    will be:
    ```
    **
    ```
* The `print()` function called without an argument will print an empty line.
The amount of possible arguments depends on the capacities of your computerbut it is going to be more than you will ever need.
* The empty string is smaller than any other.
* `pip --version` and `pip -V` will show pip version.
* The `read()` function reads the whole file
and returns a string.
The `readlines()` function also reads the whole file
and returns a list of the single lines.
And you can also iterate through the file object.
In each iteration you will get one line.
* `at` mode will allow you to append text in a file.