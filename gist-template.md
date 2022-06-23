# RegEx Breakdown

Today we will break down an example of RegEx.

## Summary

Regex or Regular expressions are patterns to match combinations of characters within strings.

The Regex example we will use today is
Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

We will break down the characeters in each section of the regex.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

After the / will be the first anchor ^ which notes the beggining of the string.
Before the last /, you will see a $, the final anchor which will note the end of the string.

### Quantifiers

The quantifiers determine the minimum and maximum limits for each sting section.
The number range will be placed between two curly brackets {min, max}.
In this example you find them to the left of the $ anchor tag.
{2,6})$/

### Character Classes

A character class defines a set of characters in input strings to complete a match.

A period (.) matches any character except the newline character (\n).
([a-z0-9_\.-]+)

(\d) denotes any Arabic number and is equal to the bracket expression [0-9].
([\da-z\.-]+)

### Grouping and Capturing

Regular expressions are generally broken up into sections using parentheses ().Below are groups from our example, they are used to query each secton of the message and are numbered from left to right.
([a-z0-9_.-]+) , ([\da-z.-]+) , ([a-z.]{2,6}).

### Bracket Expressions

A bracket expression is anything found within brackets []. Creating a range of characters to match within the text. Below you will find three bracket expressions from our example.
[a-z0-9_\.-] , [\da-z\.-] , [a-z\.]
[0-9] represents a number between 0 and 9.
[a-z] denotes any lowercase leter from a to z.
[.-] denotes the special characters that can be used.

### Character Escapes

A character escape uses a backslash to force a regex to look at the character following the backslash instead of using it in a literal. Meaning we want the expressiion to look directly for a period in the text, instead of the character class using the symbol.

## Author

Keith MacNeil is a student at Denver University.
https://github.com/Kmac5000
