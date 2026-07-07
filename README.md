[Pyhton assignment_3.py.ipynb](https://github.com/user-attachments/files/29740578/Pyhton.assignment_3.py.ipynb)
{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "7e234c04",
   "metadata": {},
   "source": [
    "# 1.What is a user defined function?\n",
    "------->A User Defined Function is a function created by the programmer to perform a specific task.\n",
    "\n",
    "Write a function to accept two numbers and return their multiplication.\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "0d6ff541",
   "metadata": {},
   "source": [
    "# 2. What is the difference between:Give one example of each.\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 1,
   "id": "408a034c",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "30\n"
     ]
    }
   ],
   "source": [
    "# Function with parameters\n",
    "------->Accepts values from the caller.\n",
    "More flexible.\n",
    "\n",
    "def sum(num1,num2):\n",
    "    print(num1+num2)\n",
    "    \n",
    "sum(10,20)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 4,
   "id": "125e66db",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Hello Punam\n"
     ]
    }
   ],
   "source": [
    "# Function without parameters    ------->Does not accept any values.\n",
    "\n",
    "def message():\n",
    "    print(\"Hello Punam\")\n",
    "    \n",
    "message()\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "759fb1fb",
   "metadata": {},
   "source": [
    "# 3.Predict the output:\n",
    "\n",
    "def fun():\n",
    "    x = 10 \n",
    "    print(x)\n",
    "\n",
    "fun() \n",
    "print(x)\n",
    "\n",
    "# Explain the reason: \n",
    "------->x is a local variable inside the function. It cannot be accessed outside the function."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "7b457e04",
   "metadata": {},
   "outputs": [],
   "source": [
    "10\n",
    "NameError: name 'x' is not defined"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 10,
   "id": "0f92778a",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "10\n"
     ]
    },
    {
     "ename": "NameError",
     "evalue": "name 'x' is not defined",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
      "\u001b[1;31mNameError\u001b[0m                                 Traceback (most recent call last)",
      "Cell \u001b[1;32mIn[10], line 6\u001b[0m\n\u001b[0;32m      3\u001b[0m     \u001b[38;5;28mprint\u001b[39m(x)\n\u001b[0;32m      5\u001b[0m fun() \n\u001b[1;32m----> 6\u001b[0m \u001b[38;5;28mprint\u001b[39m(x)\n",
      "\u001b[1;31mNameError\u001b[0m: name 'x' is not defined"
     ]
    }
   ],
   "source": [
    "def fun():\n",
    "    x = 10 \n",
    "    print(x)\n",
    "\n",
    "fun() \n",
    "print(x)\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "bc28dcae",
   "metadata": {},
   "source": [
    "# 4. Write a function that does not return anything but prints a message.\n",
    "\n",
    "Explain the default return value of such a function.\n",
    "------->The function only prints a message."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 5,
   "id": "781e10ce",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Welcome to Python\n"
     ]
    }
   ],
   "source": [
    "def greet():\n",
    "    print(\"Welcome to Python\")\n",
    "\n",
    "greet()"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "002c7c38",
   "metadata": {},
   "source": [
    "# 5. What is the difference between:\n",
    "print()-----> Displays output,Cannot be reused\n",
    "return------>Sends value back to caller,Value can be stored and reused\n",
    "\n",
    "# Explain with function example."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 7,
   "id": "49a6b7f9",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "30\n"
     ]
    }
   ],
   "source": [
    "# Using print()\n",
    "\n",
    "def add(a, b):\n",
    "    print(a + b)\n",
    "\n",
    "add(10, 20)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 8,
   "id": "d148c89c",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "30\n"
     ]
    }
   ],
   "source": [
    "# Using return\n",
    "\n",
    "def add(a, b):\n",
    "    return a + b\n",
    "\n",
    "result = add(10, 20)\n",
    "print(result)"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "22b5dbd9",
   "metadata": {},
   "source": [
    "# 6. Write a program to display:\n",
    "Data type Memory address Size in bytesof a variable entered by the user.\n",
    "-------->\n",
    "type() → Data type\n",
    "id() → Memory address\n",
    "getsizeof() → Memory size"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "7d00b587",
   "metadata": {},
   "outputs": [],
   "source": [
    "value = input(\"Enter a value: \")\n",
    "\n",
    "print(\"Data Type:\", type(value))\n",
    "print(\"Memory Address:\", id(value))\n",
    "print(\"Size in Bytes:\", sys.getsizeof(value))"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "38f8b4c4",
   "metadata": {},
   "source": [
    "# 7. Predict the output:\n",
    "\n",
    "What Python feature does this demonstrate?\n",
    "----->Dynamic Typing:\n",
    "Python automatically changes the datatype of a variable based on the assigned value.\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 9,
   "id": "aa1a60c4",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "<class 'int'>\n",
      "<class 'float'>\n",
      "<class 'str'>\n"
     ]
    }
   ],
   "source": [
    "a = 5\n",
    "print(type(a))\n",
    "\n",
    "a = 5.5\n",
    "print(type(a))\n",
    "\n",
    "a = \"Python\" \n",
    "print(type(a))"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "4d336dca",
   "metadata": {},
   "source": [
    "# 8. Explain why the following code works without declaration:\n",
    "------>Python automatically creates variables when a value is assigned.\n",
    "No datatype declaration is required.Python is dynamically typed, while C and Java are statically typed.\n",
    "\n",
    "100\n",
    "\n",
    "Compare this with Cor Java.\n",
    "\n",
    "-->#Pyhton a = 100\n",
    "-->#c      int a = 100;\n",
    "-->#java   int a = 100;"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "a1e29741",
   "metadata": {},
   "source": [
    "# 9. What is the difference between:\n",
    "\n",
    "10\n",
    "-->10 is an integer.\n",
    "\n",
    "\"Ten\"\n",
    "-->\"Ten\" is a string.\n",
    "\n",
    "\n",
    "# Is this allowed? Why?\n",
    "------>Yes, this is allowed because Python supports multiple data types."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "be47127a",
   "metadata": {},
   "source": [
    "# 10. Explain how Python manages memory automatically.\n",
    "\n",
    "----->Python automatically manages memory using.\n",
    "\n",
    "1)Memory Allocation\n",
    "-----> Python allocates memory when objects are created.\n",
    "2)Garbage Collection\n",
    "----->Unused objects are removed automatically.\n",
    "3)Reference Counting\n",
    "----->Python keeps track of how many variables refer to an object.\n",
    "\n",
    "a = 10\n",
    "b = a\n",
    "\n",
    "del a\n",
    "\n",
    "The object remains in memory because b is still referring to it.\n",
    "\n",
    "# Why does the programmer not need to explicitly allocate or free memory?\n",
    "\n",
    "Because Python automatically:\n",
    "1)Allocates memory\n",
    "2)Tracks object usage\n",
    "3)Removes unused objects\n",
    "This reduces programming errors and makes development easier."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "0e0b2b1d",
   "metadata": {},
   "outputs": [],
   "source": []
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "9fca499e",
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.11.5"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
