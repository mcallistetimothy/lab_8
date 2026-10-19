# debug_log.md
# Author: Maliyah Calliste Timothy

## Bug 1
Error type: KeyError
File + line: week8_buggy/py, line 12
What the error means: program tried to access dictionary key named 'amount' but atleast one record does not contain that
What I told the duck: The function loops through every record and adds rec["amount"] to the total. If one record uses a different spelling for the key, Python cannot find "amount" and raises a KeyError.
What I tried: I added print(f"DEBUG: rec = {rec}") before line 12 and ran the program again.
How I fixed it: I corrected the misspelled key so that all three records use "amount."

## Bug 2
Error type: TypeError
File + line: week8_buggy.py, line 16
What the error means: Python cannot compare the integer stored in amount with the string "1000" using >.
How I fixed it: I changed the limit from a string to an integer vy removing quotations so Python compares two numbers.

## After Fixing Both Bugs
Final output: Total: $5150.00 across 3 records
True
Did pytest pass? Yes

## AI Literacy Reflection
Did I use AI? Yes
If yes -- exact prompt I used: Why isnt pytest running, saying 0 collected
What AI explained: The folders weren't the same, explained to move the files to the same folder so the week8 test can read the buggy file.
What I changed myself: Error 1 & Error 2
Can I explain every fixed line? Yes

## What I learned
I learned how to read a traceback to identify the error type and the line where the problem occurred. I also learned that a KeyError can result from a misspelled dictionary key, while a TypeError can occur when comparing different data types. Finally, I learned that pytest must be able to locate both the test file and the Python module it imports, so the files must be organized in the correct project folders.