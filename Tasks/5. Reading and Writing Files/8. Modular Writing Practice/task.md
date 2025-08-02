# Modular writing practice...

I need this program to be modular, e.g.:

`def readSentences():`

`def findLongest(sentences):`

`def writeLongest(longest):`

Write a program that (1) reads a list of sentences from a file, (2) uses `len()` and *find-max* to find the longest sentence, and (3) saves that sentence to a file called `results.txt`.

---

**First module**: write a function from that reads the array of sentences from the file, and returns an array of sentences.

**Second module**: write a function that takes the array of sentences as a parameter. Loop through all the sentences, and use *find-max* to find the longest sentence. Use the pseudocode below:

1. Define the function/parameter(s)
2. Set max to length of the first sentence
3. Set a long-sentence variable to the first sentence
3. Loop through every sentence
4. Inside the loop, get length of each sentence
5. Inside the loop, if sentence length is > max, update max
6. Inside the if, store the long sentence in a string variable
7. After the loop, return the long sentence

**Third module**: Take the longest sentence as a parameter, and save it to a file. Open a file called `results.txt` and use it to store the long sentence. Close the file after you've written.
