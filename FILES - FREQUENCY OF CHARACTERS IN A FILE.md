# Exp.No:18  
## FILES - FREQUENCY OF CHARACTERS IN A FILE

---

### AIM  
To write a Python program that reads a file and counts the frequency of each character in it.

---

### ALGORITHM

1. Begin the program.  
2. Define the function `create_file()` that accepts two arguments:  
   - `file_path`: The path to the file.  
   - `content`: The string content to be written into the file.  
3. Open the file specified by `file_path` in write mode (`'w'`), and write the provided `content` into the file.  
4. Close the file (this is automatically done when exiting the `with` block).  
5. Define the function `character_frequency()` that accepts one argument:  
   - `file_path`: The path to the file whose character frequency is to be calculated.  
6. Open the file specified by `file_path` in read mode (`'r'`), and read its content into the variable `content`.  
7. Initialize an empty dictionary (`d1`) to store the frequency of each character using `defaultdict(int)`.  
8. Loop through each character in the `content`:  
   - For each character `ch`, increment its corresponding frequency in the dictionary `d1`.  
9. Return the dictionary `d1`, which contains the frequency of each character in the file.  
10. Terminate the program.

---

### PROGRAM

```
reg.no: 212222060143
name: Mariam Sherin
from collections import defaultdict

# Function to create a file with given content
def create_file(file_path, content):
    with open(file_path, 'w') as f:
        f.write(content)

# Function to calculate character frequency
def character_frequency(file_path):
    with open(file_path, 'r') as f:
        content = f.read()

    d1 = defaultdict(int)
    for ch in content:
        d1[ch] += 1
    return d1

# Example usage
file_name = "sample.txt"
file_content = "Python Programming"

create_file(file_name, file_content)
frequency = character_frequency(file_name)

print("Character frequencies in the file:")
for char, freq in frequency.items():
    print(f"'{char}': {freq}")

```


### OUTPUT


### RESULT
Thus, The Python program that reads a file and counts the frequency of each character in it was implemented and executed successfully.
