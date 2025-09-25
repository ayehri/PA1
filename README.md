# Programming Assignment #1

This file contains the codes for Programming Assignment #1, which includes the following problems:

1. Alphabet Soup Problem
- Create a function that takes a string and returns a string with its letters in alphabetical order.

2. Emoticon Problem
- Create a function that changes specific words into emoticons.
- Given a sentence as a string, replace the words smile, grin, sad, and mad with their corresponding emoticon.

3. Unpacking List Problem
- Unpack the list into three variables: first, middle, and last.
- middle should contain everything in between the first and last element.
- Print all three variables.

I. Intended Learning Outcomes

1. To identify the basic codes and functions in Python programming.

2.  To be able to apply the different codes and functions in creating a Python program.

# Code, Ouput, and Explanation:

## 1. Alphabet Soup Problem
   
   
   
         ### Code:
         def alphabet_soup(word):
         letters = sorted(word)
         sort_alphabet_soup = "".join(letters)
         print(sort_alphabet_soup)
         user_input = input("Enter a word: ")
         alphabet_soup(user_input)


### Output:
   
   Enter a word: hello
   - ehllo

### Explanation: 
   
   
   def alphabet_soup(word): def is used to define a function named alphabet_soup with one parameter, word.
   
   
   letters = sorted(word): The sorted() function arranges all the characters in the string into alphabetical order and stores them in a list.
   
   
   sort_alphabet_soup = "".join(letters): The "".join() function combines the list of letters back into a single string.
   
   
   print(sort_alphabet_soup): Displays the final sorted word.
   
   
   user_input = input("Enter a word: "): Prompts the user to type a word and stores it in the variable user_input.
   
   
   alphabet_soup(user_input): runs the function and uses the word typed by the user.


## 2. Emoticon Problem
   
   
         ### Code:
         def emoticon(sentence):
         emoticons = {"smile": ":)", "grin": ":D", "sad": ":((", "mad": ">:("}
         return " ".join(emoticons.get(word.lower(),word) for word in sentence.split())
         text = input ("Enter a sentence: ")
         print(emoticon(text))


  ### Output: 
   
   Enter a sentence: I am sad
   - I am :((
   

  ### Explanation: 
   
   
   def emoticon(sentence): defines a function called emoticon that takes a sentence.
   
   
   emoticons = {}: dictionary that matches words (smile, grin, sad, mad) to their emoticons.
   
   
   " ".join(emoticons.get(word.lower(),word) for word in sentence.split()): splits the sentence into words, replaces them 
   if they are in the dictionary, and then joins them back into a sentence.
   
   
   text = input("Enter a sentence: "): prompts the user to type a sentence.
   
   
   print(emoticon(text)): runs the function and prints the sentence with emoticons.


## 3. Unpacking List Problem
   
   
         ### Code:
         n = [1,2,3,4,5,6]
         print("First:",n[0])
         print("Middle:",n[1:-1])
         print("Last:",n[5])
   

   ### Output:
   First: 1
     
   Middle: [2, 3, 4, 5]
   
   Last: 6
   

  ### Explanation:
   
   
   n = [1,2,3,4,5,6]: creates a list of numbers.
   
   
   n[0]: gets the first element of the list which is 1.
   
   
   n[1:-1]: gets all the elements except the first and last (the middle part).
   
   
   n[5]: gets the last element of the list which is 6.
   
   
   print(): prints the results.


   

