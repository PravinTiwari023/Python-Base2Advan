# Python-Base2Advan

This Jupyter Notebook provides a comprehensive introduction to Python programming, starting from basic concepts and progressing to more advanced topics. It is designed to be a valuable resource for beginners and intermediate learners.

## Contents

- **Hello World**: Introduction to the `print` function.
- **Lambda Function**: Explanation and examples of lambda functions in Python.
- **Map Function**: Usage and examples of the `map` function.
- **Filter Function**: Usage and examples of the `filter` function.
- **File Operations**: Reading and writing files in Python.
- **Working with File Paths**: Handling file paths effectively.
- **Exception Handling**: Understanding and using try-except blocks.
- **Object-Oriented Programming (OOP)**: Introduction to OOP concepts.
- **Inheritance**: Explanation and examples of inheritance in Python.

## How to Use

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/your-username/your-repository.git
    ```
2. **Navigate to the Repository**:
    ```sh
    cd Python-Base2Advan
    ```
3. **Open the Notebook**:
    You can open the notebook in Jupyter Notebook, JupyterLab, or any compatible environment. Use the following command to start Jupyter Notebook:
    ```sh
    jupyter notebook
    ```

## Requirements

- Python 3.x
- Jupyter Notebook

Install the requirements using:
```sh
pip install jupyter
```

## Getting Started

This notebook is designed to guide you through various Python programming concepts:

1. **Print Statement**: Start with a simple print statement.
    ```python
    print("hello python!!")
    ```

2. **Lambda Function**: Learn the syntax and use of lambda functions.
    ```python
    # Lambda function can have any number of arguments but only one expression
    """
    Syntax
        lambda arguments: expression
    """
    ```

3. **Function Definitions and Usage**:
    ```python
    def addition(a, b):
        return a + b

    addition = lambda a, b: a + b
    print(addition(22, 28))
    ```

4. **Map Function**: Apply a function to all items in an input list.
    ```python
    numbers = [1, 2, 3, 4]
    squares = list(map(lambda x: x**2, numbers))
    print(squares)
    ```

5. **Filter Function**: Filter items in a list based on a condition.
    ```python
    numbers = [1, 2, 3, 4, 5, 6]
    evens = list(filter(lambda x: x % 2 == 0, numbers))
    print(evens)
    ```

6. **File Operations**: Reading from and writing to files.
    ```python
    with open('example.txt', 'w') as file:
        file.write('Hello, World!')

    with open('example.txt', 'r') as file:
        content = file.read()
        print(content)
    ```

7. **Exception Handling**: Using try-except blocks to handle exceptions.
    ```python
    try:
        result = 10 / 0
    except ZeroDivisionError:
        print("You can't divide by zero!")
    ```

8. **Object-Oriented Programming (OOP)**:
    ```python
    class Dog:
        def __init__(self, name, age):
            self.name = name
            self.age = age

        def bark(self):
            print("Woof!")

    my_dog = Dog("Rex", 2)
    my_dog.bark()
    ```

9. **Inheritance**: Understanding and implementing inheritance.
    ```python
    class Animal:
        def __init__(self, name):
            self.name = name

        def speak(self):
            raise NotImplementedError("Subclass must implement abstract method")

    class Dog(Animal):
        def speak(self):
            return "Woof!"

    class Cat(Animal):
        def speak(self):
            return "Meow!"

    my_dog = Dog("Rex")
    my_cat = Cat("Whiskers")
    print(my_dog.speak())
    print(my_cat.speak())
    ```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
