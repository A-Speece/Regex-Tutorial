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
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

In the expression `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` , we are using two anchors `^` and `$`.

The `^` anchor signifies a string that begins with the character that follows it. For example, ^#abc123 will search for any string that matches the "#abc123", while the `$` signifies the end of the string. So if we were to change and look for "c123$", it would return any string that would end with c123.

### Quantifiers

Quantifiers are used to set the limits of the sting that you regex expression matches. Quantifiers usually include the minimum and maximum number of characters that the regex is matching for.

In our regex expression `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` we are used the `{}` quantifier. Curly brackets can be used to set limits of the search in three ways.
`{ n }` matches the pattern exactly `n` number of times.
`{ n, }` matches the pattern the least number of times.
While `{ n, x }` will match for the minimum `n` number to the maximum number `x`.
In our example we are using `{ n }` curly bracket that will match for the exact number that is being passed in `{6}` and `{3}`

### OR Operator

In our regex for hexadecimal `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`, we are using the "OR" statement represented by `|` to separate the search into two criteria. We want to match with a string that contains 6 `[a-f0-9]{6}` or `|` a string that contains 3 `[a-f0-9]{3}`

### Bracket Expressions

Bracket expressions are anything within the square brackets `([])` that represent the search we are looking to match.

In our Regex `([a-f0-9]{6}|[a-f0-9]{3})` for the hexadecimal, we have a variety of bracket expressions.
`[a-z]` represents a string of characters
`[0-9]` represents a string that contains numbers
`[_-]` represents a search for underscore or hyphens

So when we take a look at the `([a-f0-9]{6}|[a-f0-9]{3})` used in our tutorial. These bracket expressions will look for any string that has a match of lowercase letters between a-f, any number between 0 and 9, and any match that has a special character of `_` or `-`.

## Author

Anthony Speece
[GitHub](https://github.com/A-Speece)
