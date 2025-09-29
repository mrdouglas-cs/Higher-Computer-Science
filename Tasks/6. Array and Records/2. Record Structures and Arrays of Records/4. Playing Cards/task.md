# Pack of Cards (from a file)

# Starter Code
```
from dataclasses import dataclass

# Card record



# Declare an array for 52 cards


# Read cards from a file
card_file = open("cards.csv", "r")
card_lines = card_file.readlines()
for i in range(52):
  parts = card_lines[i].split(",")
  cards_list[i] = Card(parts[0], parts[1], int(parts[2]))
card_file.close()

# Rest of the program goes here

```

For this program, you've been given some code that reads data about a pack of cards from a file. The file is a csv file, and looks like this:

```
king,spades,13
queen,spades,12
jack,spades,11
```

## Create the Record Structure
Define a record structure for a card - call it `Card`. The cards have three attributes: face (e.g. "king"), suit (e.g. "spades"), and value (e.g. 13).
```
@dataclass
...
...
```

Then, declare an array that can store data for 52 cards. Make sure you call this `cards_list`.

## Standard Algorithms
Now write code that counts how many red cards are in the deck. Think about how you'd check if a card is red. Use a count occurrences algorithm.

```
count_red = 0
...
...
```

## Pick a Random Card
The code below shows data about the 40th card in the list:
```
print(cards_list[39].face, "of", cards_list[39].suit)
```
Using what you remember from National 5 about `import random` and `random.randint()`, write code that will pick a random card from the list, and print similar output.

## Higher or Lower
This part of the program should ask the user for a suit, and a number (e.g "spades" and 3 for the 3 of spades).
```
suit = input("Enter suit:")
number = int(input("Enter value:"))
```
Now, re-using some of your code that picks a random card, add code that will compare the user's value to the value of the random card. Print the random value, as well as "higher", "lower", or "the same", depending on the value.

