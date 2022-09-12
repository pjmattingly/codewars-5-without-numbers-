# codewars-5-without-numbers-
Solution to the CodeWars "5 without numbers !!" challenge.

The challenge:

```
Write a function that always returns 5

Sounds easy right? Just bear in mind that you can't use any of the following characters: 0123456789*+-/

Good luck :)
```

----

In UTF16 numbers from 0 to 7 contain numbers in their codes. But numbers 8 and higher translate to strings without numbers or mathematical symbols in them. Then, we can translate those strings without numbers, into numbers, given `charCodeAt(0)`.

see:
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/charCodeAt
https://stackoverflow.com/questions/94037/convert-character-to-ascii-code-in-javascript

Then using `String.fromCharCode()`, I found string values that could be translated into numbers.

see:
https://stackoverflow.com/questions/94037/convert-character-to-ascii-code-in-javascript

Then since subtraction was banned from this challenge, and the modulous operator wasn't, I could use modulous to return a 5 given 13 modulous 8.

see:
https://www.wolframalpha.com/input?i=13+%25+8
