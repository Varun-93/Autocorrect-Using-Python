# **Autocorrect-Using-Python**
Autocorrect is based on natural language processing, As the name suggests it is programmed to correct spellings and errors while typing.


## **How it Works?**
If we type a word in our keyboard, if the word exist in the vocabulary of our device then it will assume that we have written the right word. Now it doesn’t matter whether we write a name, a noun or any word of a planet.
If the word exists in the history of the device, it will generalize the word as a correct word. What if the word doesn’t exist? If the word that we typed is a non-existing word in the history of our device then the autocorrect is programmed to find the most similar words in the history of our device.

Here we have used some words to put the functionality in our autocorrect. So we will use the text from a document(book.txt). 
We have used all the general libraries and a **textdistance** library for comparing distance between two or more sequences.

Following are the libraries used:
- Pandas
- Numpy
- textdistance
- Counter
- re(regular expression)

Here we are sorting similar words according to the Jaccard distance.

## **JACCARD SIMILARITY AND DISTANCE**
In Jaccard similarity instead of vectors, we will be using sets. It is used to find the similarity between two sets.
Jaccard similarity is defined as the intersection of sets divided by their union.

Jaccard similarity between two sets A and B is :

**Jaccard similarity= |A ∩ B| / |A ∪ B|**
              
Imagine we have the set A = {“flower”, “dog”, “cat”, 1, 3} and B = {“flower”, “cat”, “boat”}. 
Then, A ∩ B = 2 and A ∪ B = 6. As a result, the Jaccard similarity is 2/6 = 3.

