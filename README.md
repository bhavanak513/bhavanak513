{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Variable Assignment\n",
    "\n",
    "## Rules for variable names\n",
    "* names can not start with a number\n",
    "* names can not contain spaces, use _ intead\n",
    "* names can not contain any of these symbols:\n",
    "\n",
    "      :'\",<>/?|\\!@#%^&*~-+\n",
    "       \n",
    "* it's considered best practice ([PEP8](https://www.python.org/dev/peps/pep-0008/#function-and-variable-names)) that names are lowercase with underscores\n",
    "* avoid using Python built-in keywords like `list` and `str`\n",
    "* avoid using the single characters `l` (lowercase letter el), `O` (uppercase letter oh) and `I` (uppercase letter eye) as they can be confused with `1` and `0`"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Dynamic Typing\n",
    "\n",
    "Python uses *dynamic typing*, meaning you can reassign variables to different data types. This makes Python very flexible in assigning data types; it differs from other languages that are *statically typed*."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "my_dogs = 2"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "my_dogs"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "my_dogs = ['Sammy', 'Frankie']"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "my_dogs"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Pros and Cons of Dynamic Typing\n",
    "#### Pros of Dynamic Typing\n",
    "* very easy to work with\n",
    "* faster development time\n",
    "\n",
    "#### Cons of Dynamic Typing\n",
    "* may result in unexpected bugs!\n",
    "* you need to be aware of `type()`"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Assigning Variables\n",
    "Variable assignment follows `name = object`, where a single equals sign `=` is an *assignment operator*"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a = 5"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "Here we assigned the integer object `5` to the variable name `a`.<br>Let's assign `a` to something else:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a = 10"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "You can now use `a` in place of the number `10`:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a + a"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Reassigning Variables\n",
    "Python lets you reassign variables with a reference to the same object."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a = a + 10"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "There's actually a shortcut for this. Python lets you add, subtract, multiply and divide numbers with reassignment using `+=`, `-=`, `*=`, and `/=`."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a += 10"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a *= 2"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Determining variable type with `type()`\n",
    "You can check what type of object is assigned to a variable using Python's built-in `type()` function. Common data types include:\n",
    "* **int** (for integer)\n",
    "* **float**\n",
    "* **str** (for string)\n",
    "* **list**\n",
    "* **tuple**\n",
    "* **dict** (for dictionary)\n",
    "* **set**\n",
    "* **bool** (for Boolean True/False)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "type(a)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a = (1,2)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "type(a)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Simple Exercise\n",
    "This shows how variables make calculations more readable and easier to follow."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "my_income = 100\n",
    "tax_rate = 0.1\n",
    "my_taxes = my_income * tax_rate"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "my_taxes"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "Great! You should now understand the basics of variable assignment and reassignment in Python.<br>Up next, we'll learn about strings!"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
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
   "version": "3.8.8"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}
