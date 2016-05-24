# Decryption
Simple program to encrypt and decrypt messages using Ceaser ciphers, completed as part of an assignment and with helper code from MIT open-courseware Python class.

-The basic purpose of this program is to first create a function that will take a string and encrypt it using a Ceaser cipher. The way the Ceaser cipher works is it takes in a tuple or multiple tuples such as [(0,6)]. This tuple baically represents [(location to start shift, number of letters to shift text)]. So a shift of (0,6) will start at the 0th value of the string and shift every letter thereafter by 6 letters so an A would become an F.
When multiple tuples are input into the program, they will be applied sequentially, so for [(0,3),(3,6)] will first shift the entire string by 3 letters then take that shifted text and shift it 6 letters starting at the 3rd letter in the string. 

The second part of this program will take an encrypted string to which a shift or multiple shifts have been applied and decrypt it by basically doing the following;  
      1) Starting at the 0th element in the string, begin shifting the string by applying shifts from 0 to 27
      2) Try to identify possible words by looking for spaces in the string
      3) Check the possible word against the wordlist
      4) If possible word is found within wordlist, recursively call the function with a start location of wherever the space was found and begin applying shifts and checking for words to the remaining section of the string
      
      
