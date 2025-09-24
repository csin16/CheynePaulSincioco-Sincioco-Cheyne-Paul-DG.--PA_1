_Cheyne Paul DG. Sincioco-2ECEA_PA-1_

_PA#1 INTRODUCTION TO PYTHON PROGRAMMING_

# __About the Programming Assignment__

This assignment aims to hone our programming skills in basic coding in Python. This task requires us to create user-defined functions and apply them to different problems. 

-------------------------------------------------------------------------------------------------------------------------------------------
1. __ALPHABET SOUP PROBLEM: Create a function that takes a string and returns a string with its letters in alphabetical order.__
   
__Code:__
```
word = []      #List to store all letters
```
The code __word = []__ is a list to store all letters in the word.

__Code:__
```
def alphabet_soup(string):   #Function that takes a word and arrange it alphabetically
```
Function to alphabetically arrange the word.

__Code:__
```
    for x in string:       #A loop that stops to go through every letter in the word
```
A loop that stops if all letters in the word are read.

__Code:__
``` 
        word.append(x)    #Puts all the letters into the list 
    word.sort()           #Sorts it alphabetically 
```
The letters in the word were inserted using __.append()__, sorted using __.sort().__.

__Code:__
```
    print (''.join(word))    #Combines all the letters in the list
```
The letters in the list were joined together by the code __' '.join()__, 

__Code:__
```
inp = input("Enter a Word: ")      #Takes the user's input
alphabet_soup(inp)                 #Puts the input into the function
```
The code __input()__ takes the user's input and puts it in the function.

__Example Output:__
```
Input: Hello
Output: ehllo
```
-------------------------------------------------------------------------------------------------------------------------------------------
2. __EMOTICON PROBLEM: Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad, and mad with their corresponding emoticon:__
   
__Code:__
```
emojis = {"Smile" : ":)", "Grin": ":D", "Sad": ":((", "Mad" : ">:("}      #Dictionary to store data in pairs
new = []                                                                  #Storage for the new phrase with the emoticon
```
The code displays the use of a dictionary __emojis = {"Smile" : ":)", "Grin": ":D", "Sad": ":((", "Mad": ">:("}__ to store data in pairs. Also, the list __new=[]__ was initialized to store the new phrase with the emoticon.

__Code:__
```
def emotify(phrase):             #Function to emotify the phrase
```
This is a user-defined function that takes the user's input in order to achieve a certain result.

__Code:__
```
    words = phrase.split()     #Splits every word in the phrase
```
The code shows the use of __.split()__ to split each word in the phrase, and store it in the variable words.

__Code:__
```
    for x in words:         #Stops if every word was used
```
To repeat the process, a for loop was used to take each word in the variable words into the function.

__Code:__
```
        if x in emojis:                               #Condition if the word was in the dictionary
            new.append(emojis.get(x))                 #Gets its corresponding pair
        else:
            new.append(x)                             #Return the words that did not fit the condition             
```
An if-else loop was used to sort phrases. If the word in the variable words fits a word in the dictionary, the corresponding pair will be displayed as an emoticon. Then all words that do not fit into the condition will be the same.

__Code:__
```
    print(' '.join(new))                      #Joins every word in the dictionary
 ```
The code __' '.join__ was used to combine the designated output since they are in a list with commas separating them.

__Code:__
```
inp = input("Enter a Phrase: ")            #Takes the user's input
emotify(inp)                               #Takes the input the put it in the function

```
Lastly, the function needs an input. The code __input()__ will take the user's input, then it will be put in the emotify function.

__Example Output:__
```
Input: I am Sad
Output: I am :(
```
-------------------------------------------------------------------------------------------------------------------------------------------
3. __UNPACKING LIST PROBLEM: Unpack the list writeyourcodehere into three variables, being first, middle, and last, with middle being everything in between the first and last element. Then print all three variables.__

__Code:__
```
inp = input("Enter Numbers Separated by a Comma: ")   #Takes integers from the user input and stores it to variable inp
```
The input was taken and was stored in the variable inp.

__Code:__
```
list = inp.split(",")      #Splits the integers from variable inp and stores them in
list.sort()                #Sorts the list to arrange it in order
```
Then inp was split using the code __.split()__ and was stored in a list. To arrange it, __.sort()__ was used.

__Code:__
```
first, *middle, last = list                                               #Stores the value of list to first,middle, and last
print("First:", first, "     Middle:", middle, "     Last:", last)        #Displays the integers in arranged order
```
And to arrange them, variables __first, *middle, last__ were stored to __list__, which was used. Then, the output  was displayed as first, middle, and last. 

__Example Output:__
```
Input: 2,1,3,5,4,2
Output: First: 1, Middle: ['2', '2' ,'3' ,'4'], Last: 5
```
-------------------------------------------------------------------------------------------------------------------------------------------
__Lessons Learned__:

This programming assignment taught me basic coding in Python. It taught me to make use of different predefined data structures, such as lists, dictionaries, and input, and create user-defined functions to apply to diverse problems.

__Tech(s) Used__: Jupyter Notebook
