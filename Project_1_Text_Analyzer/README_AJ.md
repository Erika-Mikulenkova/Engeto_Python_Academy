# **Engeto_project_1: Text Analyzer**

## Project Description:
The goal of this project was to create a text analyzer – a program that can process any length of text and provide various information about it. The program works with three predefined texts, but it is not limited to a fixed number of texts — it should work correctly with any number of texts.

## Predefined Texts:
TEXTS = [
    '''Situated about 10 miles west of Kemmerer,
    Fossil Butte is a ruggedly impressive
    topographic feature that rises sharply
    some 1000 feet above Twin Creek Valley
    to an elevation of more than 7500 feet
    above sea level. The butte is located just
    north of US 30 and the Union Pacific Railroad,
    which traverse the valley.''',
    '''At the base of Fossil Butte are the bright
    red, purple, yellow and gray beds of the Wasatch
    Formation. Eroded portions of these horizontal
    beds slope gradually upward from the valley floor
    and steepen abruptly. Overlying them and extending
    to the top of the butte are the much steeper
    buff-to-white beds of the Green River Formation,
    which are about 300 feet thick.''',
    '''The monument contains 8198 acres and protects
    a portion of the largest deposit of freshwater fish
    fossils in the world. The richest fossil fish deposits
    are found in multiple limestone layers, which lie some
    100 feet below the top of the butte. The fossils
    represent several varieties of perch, as well as
    other freshwater genera and herring similar to those
    in modern oceans. Other fish such as paddlefish,
    garpike and stingray are also present.'''
]

## Project Structure:
Create a single repository dedicated to this project. The repository should contain only one file named main.py. Each project has its own separate repository. The source code in main.py must not exceed 150 lines (empty lines and comments count toward the limit). 

## User Login:
At the beginning, the program should ask for a username and password. Both values must match a correct pair (username ~ password). Verification occurs only after both values are entered. If the user is registered, the program greets them and allows them to analyze the texts. If the user is not registered, the program should notify them and terminate.

Registered users: 
```
+------+-------------+  
| user |   password  |  
+------+-------------+  
| bob  |     123     |  
| ann  |   pass123   |  
| mike | password123 |  
| liz  |   pass123   |  
+------+-------------+
```

## Program Flow:
The user must select a text by its numeric index. If the user enters an invalid text number (outside the available range), the program should notify them and terminate. If the user enters non-numeric input (e.g., a word or special character), the program should also notify them and terminate.

## Output:
The program should display: Number of words (a word is a string separated by spaces); Number of words starting with a capital letter; Number of words written in UPPERCASE; Number of words written in lowercase; Number of numeric strings (not digits); Sum of all numeric values in the text. Additionally, the program should display a simple bar chart representing the frequency of different word lengths.

Example output:

```
----------------------------------------
There are 54 words in the selected text.  
There are 11 titlecase words.  
There are 1 uppercase words.  
There are 38 lowercase words.  
There are 4 numeric strings.  
The sum of all the numbers 8540.
----------------------------------------
LEN|     OCCURRENCES    |NR.
----------------------------------------
  1|*                   |1  
  2|**********          |10  
  3|*****               |5  
  4|***********         |11  
  5|************        |12  
  6|***                 |3  
  7|****                |4  
  8|*****               |5  
  9|*                   |1  
 10|*                   |1  
 11|*                   |1
```
