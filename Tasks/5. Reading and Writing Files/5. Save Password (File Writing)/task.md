# Save Password (writing files)

Write a program that asks the user to enter a new password. Use input validation to make sure that the password is at least 6 characters long. Once a valid password is entered, save it in a file.

Your program should have a *function* called getValidPassword() that asks the user to enter a password, and validates it.

You should then add a *procedure* that takes the password as a parameter, and writes it to a file called password.txt.

**Data flow table:**
```
getValidPassword     IN     --
                     OUT    password
saveToFile           IN     password
                     OUT    --
```

Look at your notes, to remind you how to write files. It's in the Python practical notes (complete example on page 28).
