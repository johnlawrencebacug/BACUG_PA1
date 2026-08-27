# PROGRAMMING ASSIGNMENT 1
### Bacug, John Lawrence B. | 2ECE-C

## Objectives: 
1. use basic Python functions, operators, and string operations;
2. manipulate strings using indexing, slicing, and built-in string methods;
3. apply sequence unpacking to manipulate the elements of a list; and
4. construct simple Python functions that return a specified result.

## Problem A
Create a function named rotate word() that accepts a non-empty string. Move the first character
of the string to the end while keeping all remaining characters in their original order.

* String Indexing: `text[0]` - it is a line of code that extracts a character positioned at index 0.
* String Slicing: `text[1:]` - extracts the character starting from index 1 to the last index.
* Input: `word = input("Enter a word: ")` - prompts the user to input whatever word they want. it is then stored in the variable `word`
* Print: `print("Rotated word:", rotate_word(text))` - the stored data is then printed and rotated.

#### CODE
```python

def rotate_word(text):
  return text[1:] + text[0]

word = input("Enter a word: ")
print ("Rotated word:", rotate_word(text))
```

## PROBLEM B
Create a function named make username() that accepts two strings: first name and last name. The
function must:
1. convert all letters to lowercase;
2. remove all spaces from the first name;
3. remove all spaces from the last name; and
4. join the processed first and last names using one period (.).

Using string methods and concatenation.

Concatenations:
* `first_name.lower()` - changes all characters to lowercase.
* `first_name.replace()` - replaces the specified substring to another.
* `first_name = first_name.replace(" ", "")` - this part erases the space. the same thing is done for the last name.

String Methods:
* '+' - this operator is addition. in this case adding two strings together.
* `return first_name + "." + last_name` - this part of the code adds a period to the inputs.
#### CODE
```python

def make_username(firstname, lastname):
  first_name = first_name.lower()
    first_name = first_name.replace(" ", "")

    last_name = last_name.lower()
    last_name = last_name.replace(" ", "")

    return first_name + "." + last_name

## PROBLEM C
first_name = input("Enter first name: ")
last_name = input("Enter last name: ")

print("Username:", make_username(first_name, last_name))

```

## PROBLEM C
Create a function named swap bookends() that accepts a list containing at least two elements. Unpack
the list into three variables:
• first – the first element;
• middle – a list containing everything between the first and last elements; and
• last – the last element.
Using these variables, return a new list in which the first and last elements have exchanged positions.
The elements in middle must remain in their original order.

`first, *middle, last = items` - this is extended sequence unpacking. The *middle means "put everything between the first and last elements into a list called middle."
`return [last, *middle, first]` - this creates a new list.
1. last first
2. everything in the middle after.
3. first at the end.
`items = [1, 2, 3, 4, 5]` - i created a list then stored it in the variable `items`.
`result = swap_bookends(items)` - calls the function and then it gives the items list.

#### CODE
```python

def swap_bookends(items):
    first, *middle, last = items
    return [last, *middle, first]

items = [1, 2, 3, 4, 5]

result = swap_bookends(items)

print(result)
print(items)

```
