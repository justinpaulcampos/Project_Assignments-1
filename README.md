# Project Assignment 1

### This Assignment is separated into 3 activities which are outlined below:
#### Alphabet soup: https://github.com/justinpaulcampos/Project_Assignments-1/edit/main/README.md#alphabet-soup-1
#### Emoticon problem: https://github.com/justinpaulcampos/Project_Assignments-1/edit/main/README.md#alphabet-soup-1
#### Unpacking List Problem: https://github.com/justinpaulcampos/Project_Assignments-1/edit/main/README.md#unpacking-list-problem-1

## Alphabet Soup
The goal of this program is to sort string input to output the letters of the string in alphabetical method

My approach for this was to convert the string to a list to make use of the sort() function.

As you can see below, the conversion of the word and creating a new string for the output. 
``` python
def alphabet_soup(word):
    #Initialize variable
    new_word = "";  lst=[]
    #Convert the string to list
    lst=list(word)
```
Then, as mentioned, I achieved all sorting using the .sort function. 
``` python
#Sort the string alphabetically
lst.sort()
```
Then, to have an output as a string, I converted the output from a list to a string. This was made using a for loop so that all the items in the list would be added to a string or the variable new_word. Then, finally, outputting the converted string data to print.
``` python
    for x in range(0,len(lst)):
        new_word = new_word + lst[x]
    #print output
    print(new_w)
```
## Alphabet Soup
The goal of the program was to convert a certain text of emotion to an emoticon.

My approach here was to make a dictionary whose keys are certain words and the value of the keys are the emoticons described by the words. 
``` python
def emotify(emo):
    #initiate dictionary for emotions
    emolst = {"sad": ":((","mad": ">:(","grin": ":D","smile": ":)","Sad": ":((","Mad": ">:(","Grin": ":D","Smile": ":)"}
```
After that, using a for loop to replace certain keys with their value.
``` python
for x in emolst:
    emo = emo.replace(x,emolst.get(x))
```
Finally, after it loops through all the items in the dictionary, we can output the data.
```python
#print output
print(emo)
```
## Unpacking list problem
The goal of the problem was to divide the list into 3 parts: the first value, the last value, and what's left in between.
What I did here was just to separate the first and last value into their own variable. For the "first" variable, I put the zeroth index of the list.
```python
#initialize first value
first = lst[0]
```
On the other hand, the "last" value I had to use the function "len" to find the length subtracted by 1, so that we can get the last index of the list.
``` python
#initialize the last value
last = lst[len(lst)-1]
```
As for the "middle" variable, I sliced the array from the second item of the array or the first index to the last index, and due to slicing terminating the stop index, I don't have to account for removing the last item of the list.
``` python
#initialize the middle list
middle = lst[1:len(lst)-1]
```
Finally the output can be printed.
``` python
print("First:", first, " Middle:", middle, " Last:", last,)
```
