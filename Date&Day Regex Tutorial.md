# Title (Regex Date Validation DD/MM/YYYY,day of the week)

 
## Summary

Regex or regular expression is a type of object that can be constructed with a written  literal value by enclosing a pattern in forward slash (/) characters.
These regular expressions are patterns used to match character combinations in strings.  

Another way to create a regex is by using the constructor function of the RegExp object.  

The Regex described in this tutorial is an pattern to validate date and day of the week.    

Let Regex = /^([0]?[1-9]|[1|2][0-9]|[3][0|1])\/([0]?[1-9]|[1][0-2])\/([0-9]{4}|[0-9]{2})\,((mon|tues|wed(nes)?|thur(s)?|fri|sat(ur)?|sun)(day)?)$/i   

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

The function of the Anchor components in a Regex is to represent the beginning and the end of the string. The "^" represents the beginning of the string and the "$" represents the end, when found at the beginning and end, respectively.  
In this example, these anchors indicate the last part of the expresion should be the day of the week and the beginning of the expresion is the day date.

### Quantifiers  

x{n}, where "n" is a positive integer, matches exactly "n" occurrences of the preceding item "x". In this example, [0-9]{2}, the expresion will match if there 2 ocurrences one for each number from 0 to 9, including those two.

Another example of quantifiers that we can be found in this case is "x?".
For instance when this "(day)?" is written after (mon) means that expression will match whether mon is written or monday.

### Grouping Constructs

They can be enclosed in parentheses (...). The result of enclosing part of the parterm in parantheses is that a quantifier is put after the parentheses, it applies to the parentheses as a whole. In this regex, we can see this when all the week days are grouped in () and then "(day)?" is added at the end, quantifier affects to all the options whithin the parenthesis.

### Bracket Expressions

The Brackets indicate a set of characters to match.It can express different things to match depending on the expresion within the brackets.
For instance in the regular expression described in this file, a bracket expresion used is 
[1-9], this mean that al numbers between 1 and 9, inclusing these two will match the expresion.

### Character Classes
Character classes distinguish kinds of characters such as, for example, distinguishing between letters and digits.

An example of a Character class is a character escape, that is describe below.
In this example the character escape used is "\". It is used to find literal dot in a expresion "\.". This matches "."


### The OR Operator

This operator is represented by the symbol "|" and means the expression will match what is written on the left or on the right of this symbol.
x|y	Matches 'x' OR 'y'.

In this example is used serveral times, first on the date validation, so the expresion will match one or two digits for the day and month.
It is also used on the day of the week validation.

### Flags

A flag is an optional parameter to a regex that modifies its behavior of searching.
they are written after the second slash that wraps the regex.

The flap used in this example is "i". This flag is used to make the expression search case-insensitively.

In this date validation,the expression will match any day of the week in lowercase or uppercase.

### Character Escapes

In this example the character escape used is "\". This character causes the preceded symbol or character to be interpreted literally. "\." will match "."  

## Author

[Alicia Santidrian GitHub](https://github.com/asantidrian/AS_Regex_Date-Day)  
Alicia Santidrian Email: asantidrian83@gmail.com

