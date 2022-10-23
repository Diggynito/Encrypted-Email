Understanding the Code
Starting at line one, declare variable result and assign it an empty string. For line three, create a choice variable and assign it an input. This particular choice is asking the user to enter either a numerical 1 or 2.
choice = input("\nEnter 1 to Encrypt or 2 to Decrypt:\n>>")
Lines five through ten use an if statement to determine the user’s choice. Starting at line eight, the code becomes a bit trickier. range() reads a string, chr() converts an integer into a character, ord() converts a character into an integer, and - 4 subtracts four. Meanwhile, ASCII is utilized to formulate a numerical representation. For example, if the character is “A”, you’ll get “=” as the result. If you encrypt “Derek”, the output will display “@anag”. To make the concept easier to understand, if the code is changed to - 1 and inputting “B”, the output will be “A”.
If the user chooses to decrypt, which will come into play when receiving encrypted emails, lines twelve through seventeen does the complete opposite by adding four.
Finally, lines nineteen and twenty utilize an else statement to prevent incorrect inputs.
Sending Encrypted Emails
There’s a plethora of examples regarding sending emails using Python. This example uses Gmail, and it should be noted that Google’s security and authentication might unexpectedly change. In order for this to work, you’ll need to allow less secure apps. For this section, I couldn’t use Trinket because it doesn’t allow the smtplib module.
