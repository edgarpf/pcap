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
    You can combine them with: <br>
        stocks_1 | stocks2 <br>
        stocks_1.update(stocks2) <br>
        {**stocks_1, **stocks2}
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
* 