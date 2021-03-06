Decorator pattern allows a user to add new functionality to an existing object 
without altering its structure. In simple words: they are functions which modify
the functionality of another function.

Before start, please, look at this example below.

```
def do_twice(func):
    def wrapper_do_twice():
        func()
        func()
    return wrapper_do_twice
```

function do_twice DOUBLES any function's return value.
from decorators import do_twice
@do_twice

here, "@" sign is used to call the decorator. Decorator is called  right before a target #function.
```
def say_whee():
    print("Whee!")
```
>>> say_whee()
Whee!
Whee!

1. Look at the file stringify_decorator.py

2. There are tests for decorators, you are going to write. Look at the file tests_for_decorators.py, located in tests folder.

3. Run tests with command:

    ```python3 -m unittest tests/tests_for_decorator.py```

4. Now, complete the functions in stringify_decorator.py

5. Run tests and all of them should be passed.

6. Compare your answer with mine located in answers/stringify_decorator.py

7. Good! Now you know basics about decorators. Commit and push your changes. 

8. Now, do all this steps for file called decorator_with_argument.py and decorator_with_positional_argument.py
