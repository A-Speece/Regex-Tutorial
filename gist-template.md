# Title (Regex Tutorial: Hexadecimal)

Hexadecimals or simply hex is a numbering system with base 16. It can be used to represent large numbers, but using few digits. Developers will use a combination of numbers (typically 0-9), followed by alphabetic characters (6). One of the most commonly used hexadecimal are hex color code which are using in Web Design. We used these hex values define the color that will be used in styling the web application. Some example of hex color coding would be `#808080` which represents the color Gray, or `#FF0000` that represents the color Red.

## Summary

In this Regex Tutorial, we are going to take a look at a regular expression to match any hexadecimals in a string of characters.

A regular expression is defined as a sequence of characters that specifies a search pattern in text or a string.

The regex that we are going to be covering is `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

This regex will allow us to find any hex code that contains a # sign, or has 6 or 3 characters.

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

In the expression `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` , we are using two anchors "^" and "$".

The `^` anchor signifies a string that begins with the character that follows it. For example, ^#abc123 will search for any string that matches the "#abc123", while the `$` signifies the end of the string. So if we were to change and look for "c123$", it would return any string that would end with c123.

### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

## Author

Anthony Speece
[GitHub](https://github.com/A-Speece)
