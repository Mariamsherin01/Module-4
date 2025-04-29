# Exp.No:19  
## CLASS AND OBJECTS - Creating a Dictionary with Words and Their Reverses from User Input

---

### AIM  
To write a Python program that takes a sentence as input from the user and returns a dictionary where the keys are the words from the sentence and the values are their reversed forms.

---

### ALGORITHM

1.Prompt the user to enter a text (sentence).

2.Split the text into individual words using the split() function.

3.Create an empty dictionary.

4.Loop through each word in the list:
a. Reverse the word using slicing ([::-1]).
b. Add the word and its reverse as a key-value pair in the dictionary.

5.Print the resulting dictionary.

---

### PROGRAM

```
reg.no: 212222060143
name: Mariam Sherin
T=input()
l=T.split(' ')
d=dict({})
for word in l:
    d2=word[::-1]
    d[word]=d2
    
print("The obtained dictionary is d = ",d)


```

### OUTPUT

![image](https://github.com/user-attachments/assets/f5e31d85-6a9c-436d-8c06-307f1595df9f)


### RESULT
Thus, The Python program that takes a sentence as input from the user and returns a dictionary where the keys are the words from the sentence and the values are their reversed forms was implemented and executed successfully.



