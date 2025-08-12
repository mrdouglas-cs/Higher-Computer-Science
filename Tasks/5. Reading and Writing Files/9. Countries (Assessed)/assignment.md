# Countries (writing files) - marked program

**I want to review this program, so make sure to let me know when done**. Treat it like a mini version of the assignment, with similar conditions in class. Always check your practical notes. You can discuss it, but don't copy exact work from each other.

---

You've used the countries.txt file before.

This time, write a **modular** program to (1) read the countries from the file, (2) find the shortest country's name, (3) find countries starting with a letter E, and write them to a file.

**Data flow**:
```
getCountries    IN    ---
                OUT   countries[]
findShortest    IN    countries[]
                OUT   shortestName
countE          IN    countries[]
                OUT   ---
```

**First module**: read the countries from a text file, and return the array of countries. Your main algorithm should have a line like `countries = getCountries()`.

**Second module**: Take the array of countries as a parameter. Do a *find-min* algorithm and `len()` to find the country with the shortest name. Return the shortest name, and in the main algorithm, use `print()` to display it.

**Third module**: Inside the module, open a file called `results.txt`. Then do a loop, and loop through each country. If the first letter of the country is E (use substring), write this one to the file. When you're done, close the file. Some pseudocode for this is below:

1. Define the module
2. Open file in write mode
3. Loop through all countries
4. Inside the loop, get the first letter using substring
5. Inside the loop, if the first letter is E, write this country to the results file
6. Outside the loop, close the file
