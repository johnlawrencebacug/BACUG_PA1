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

* String Indexing: 'text[0]' - it is a line of code that extracts a character positioned at index 0.
* String Slicing: 'text[1:]' - extracts the character starting from index 1 to the last index.

#### CODE
'''python
def rotate_word(text):
  return text[1:] + text[0]

word = input("Enter a word: ")
print ("Rotated word:", rotate_word(text))


'''
