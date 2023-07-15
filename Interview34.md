Input: "In a galaxy far far away"
Output: "far"

Input: "Taco cat ate a taco"
Output: "taco"

Input: "No. Try not. Do or do not. There is no try."
Output: "No" 

Algorithm:
1. Initialize an empty dictionary for word counts.
2. Convert the input string to lowercase.
3. Remove punctuation from the string.
4. Split the string into words using spaces as separators.
5. Iterate through the words:
   - If the word exists in the dictionary, increment its count.
   - If the word doesn't exist, add it to the dictionary with count 1.
6. Find the word with the maximum count by iterating over the dictionary.
7. Return the word with the maximum count.

Code:
```
def find_most_common_word(book):
    word_counts = {}

   
    words = ''
    for c in book:
        if c.isalnum() or c.isspace():
            words += c.lower()
        elif c.isspace() and words[-1:].isalnum():
            words += ' '

    
    words = words.split()

   
    for word in words:
        if word in word_counts:
            word_counts[word] += 1
        else:
            word_counts[word] = 1

 
    max_word = ""
    max_count = 0
    for word, count in word_counts.items():
        if count > max_count:
            max_word = word
            max_count = count

    return max_word
```
Test Cases:
- find_most_common_word("In a galaxy far far away")
  Expected Output: "far"

- find_most_common_word("Taco cat ate a taco")
  Expected Output: "taco"

- find_most_common_word("No. Try not. Do or do not. There is no try.")
  Expected Output: "No"
