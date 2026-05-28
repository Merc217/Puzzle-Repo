# Puzzle-Repo
   - A short explanation of how you found the hidden challenge
To be fully transparent, I came across this job posting on Indeed while in bed. I eyeballed the challenge and didn't see any noticable patterns but did get the feeling it was encoded. I plugged the challenge into GPT which confirmed it was Base64.
     
   - How you decoded the original string
Opened Notepad++ > Pasted Encoding > Plugins > MIME Tools > Base64 Decode

   - What this script does
The script creates an environment variable called "DONT_PANIC" and sets the value of the variable to 1.
Python is then launched and fed the puzzle.py file as well as a --candidate argument value of yours truly.
The file gets parsed but there is no actual output since it treats this file as one giant text string.

   - The command you ran
$env:DONT_PANIC="1"
py puzzle.py --candidate "Dirk Fisher"
# Used Powershell so it had to be a bit different.

   - The exact output you received
SyntaxError: unterminated triple-quoted string literal (detected at line 39)
# I had to add the triple quote at the end to close it and then re-ran the script successfully.

   - The final decrypted answer
The actual answer itself was the set of instructions to create this Git Repot + Readme.

   - Any tools you used, including AI tools
ChatGPT
Powershell CLI
Python
Github
