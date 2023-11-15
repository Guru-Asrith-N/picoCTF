### writeup on crytography

#### miniRSA

opened the challenge
downloaded the file using `wget https://jupiter.challenges.picoctf.org/static/ee7e2388b45f521b285334abb5a63771/ciphertext`
opened the file using `cat ciphertext`
the formula is given in primer for this ( `m^e mod n = c `)
although it looks difficult , there is a small chance that `m^e <n`  in which case `m^e = c` . e is also very small which shows that the chance of this occuring is very high 
therefore `m = c^(1/e)` 
directly substituting the values will not give the answer as it will give shortened form
searched in google about how to write a program for this but didn't get it 
finally read a writeup  'https://github.com/VermillionBird/CTF-Writeups/blob/master/2019/picoCTF/Cryptography/miniRSA/README.md' and got the program from there 'https://github.com/VermillionBird/CTF-Writeups/blob/master/Useful-Scripts/Cryptography/invpow.py'
got the flag
```
flag : 
```
