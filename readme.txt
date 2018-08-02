Hi! Here's the dictionary attack code we went over in class.

To generate your dictionary for the attack, run the following
in your command prompt:
>> python dictionarygenerator.py < 1000words.txt > dictionaryattack.txt

To use that generated dictionary to crack the password, run the
following in your command prompt:
>> python passwordentry.py < dictionaryattack.txt

Try using your own password! Here are the steps to do that:
1. replace "#a string of your choice" in hasher.py with whatever
password you want to use, and run the following:
>> python hasher.py
2. copy the entire output (including the b and both single-quotes)
and replace the current value of myHashedPassword in passwordentry.py
with that output

Then, try running your password attack again!

QUESTIONS TO CONSIDER
What passwords are crackable?
What passwords aren't?
Are the following passwords crackable:
  -b4Nk
  -b3causE
  -c3ll
  -billion
  -Language
How would you modify your program to crack any of the uncrackable passwords above?
How would you modify your program to crack passwords like "li9hT",
"Ma9azine", and "pRo9ram"? What about passwords like "so1diEr", "nEar1y",
and "suCcessfu1"?
Suppose the user were smarter, and made every character that could be
converted to a number that number (e.g. "b4n4n4", "m3l0n", "str4wb3rry").
How would you crack these passwords?
CHALLENGE: Now say the user was required to have a special character in their
password. The user is still lazy, and a) only includes one special character
in their password, and b) uses only #, !, or $ as their character. How might
you write code to crack this password? Try cracking the following passwords if
you think you've written something that works:
  -b4Ll!
  -s$t0rE
  -W0r#ld
  -wOnd3r$
  -#w0mAn
