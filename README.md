# Programming-Assignment-1
## Experiment 1 - Introduction to Python Programming
### Intended Learning Outcomes
1. To identify the basic codes and functions in Python Programming
2. To be able to apply the different codes and functions in creating a Python Program
### Given Problems
1. ALPHABET SOUP PROBLEM
2. EMOTICON PROBLEM
3. UNPACKING LIST PROBLEM
------------------------------------------
## ALPHABET SOUP PROBLEM
For this problem, I have to create a function that takes a string and returns a string with its letters in alphabetical order
#### Example
alphabet_soup("hello") --> ehllo

alphabet_soup("hacker") --> acehkr
### My Code
```python
def alphabet_soup(word):              #create a function that takes a word and rearrange the letters into alphabetical order
    sortletters = sorted(word)        #Sort the letters  
    strd = str(sortletters)           #Converting the list to string
    strd = strd.replace("[", "")      #Removes the opening bracket
    strd = strd.replace("]", "")      #Removes the closing bracket
    strd = strd.replace("'", "")      #Removes the single quote
    strd = strd.replace(", ", "")     #Removes the comma
    return strd                       
```
```python
print(alphabet_soup("hello"))
```
ehllo
```python
print(alphabet_soup("hacker"))
```
acehkr
### Explanation
1. **Defining the Function** - 
The function 'alphabet_soup(word)' takes in a string ('word') as input
2. **Sorting the letters** - 
sorted(word) arranges the letters of the word in alphabetical order and stores them in a list
3. **Converting the list to string** - 
By using 'str(sortletters), this allows the list to be converted into a string
4. **Removing unwanted characters** - 
The following 'replace()' functions is used to remove any unnecessary characters such as the opening and closing brackets, single quotes, and commas to the necessary output
------------------------------------------
## EMOTICON PROBLEM
For the second problem, I have to create a function that changes a specific word into an emoticon. Given a sentences as a string, I will be replacing the words such as smile, grind, sad and mad to their corresponding emoticon
#### Example
emotify(“Make me smile”) --> Make me :)

emotify(“I am mad”) --> I am >:(
### My Code
```python
def emotify(emoticon):     #Function that takes an a specific word and changes into emoticons
    emoticon = emoticon.replace("smile", ":)")       #Emotifies the word smile to :) 
    emoticon = emoticon.replace("grin", ":D")        #Emotifies the word grin to :D
    emoticon = emoticon.replace("sad", ":((")        #Emotifies the word sad to :((          
    emoticon = emoticon.replace("mad", ">:(")        #Emotifies the word mad to >:(
    return emoticon
```
```python
print(emotify("Make me smile"))
```
Make me :)
```python
print(emotify("I am sad"))
```
I am :((
### Explanation
1. **Defining the Function** - 
The function 'emotify(emoticon)' takes in a string ('emoticon') as input
2. **Emotify the specific words** - 
The 'replace()' function is used to look for the specific words in the sentences and replace them to their corresponding emoticon such as smile --> :), grind --> :D, sad --> :((, and mad --> >:(
3. **Return new sentences** - 
Once the specific words have been changed to a specific emoticon, the output will show the updated sentence
------------------------------------------
## UNPACKING LIST PROBLEM
For the last problem, I have to unpack the list writeyourcodehere into three variables, first, middle, and last, with middle having every element between the first and last element. Once unpacked, the three variables must be printed
#### Example
1st = [1, 2, 3, 4, 5, 6]

first: 1  
middle: [2, 3, 4, 5]  
last: 6
### My Code
```python
writeyourcodehere = [1, 2, 3, 4, 5, 6]              #The list writeyourcodehere

first = writeyourcodehere[0]                        #Takes the first element of the list
middle = writeyourcodehere[1:-1]                    #Takes the elements in beteween of the first and last element
last = writeyourcodehere[-1]                        #Takes the last element
```
```python
print("first: ", first)
```
first: 1
```python
print("middle: ", middle)
```
middle: [2, 3, 4, 5]
```python
print("last: ", last)
```
last: 6
### Explanation
1. **Defining the list** - 
The list 'writeyourcodehere' is created with the values [1, 2, 3, 4, 5, 6]
2. **Getting the first element** - 
The 'writeyourcodehere[0]' takes the element at index 0, the first element of the list
3. **Getting the middle elements** - 
The 'writeyourcodehere[1:-1]' uses slicing to take all elements between the first and last element
4. **Getting the last element** -
The 'writeyourcodehere[-1]' then takes the last element
5. **Printed output** -
Each variable (first, middle, and last) is printed separately
