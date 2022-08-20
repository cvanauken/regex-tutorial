# regex-tutorial

# Regex Tutorial - Matching Email

Regular Expressions, also known as Regex for short, can be used to find certain patterns of characters, numbers or symbols inside a string. With Regex you can also find and replace a character or sequence of characters within a string as well. Regex is commonly used to validate an input within a string of text. The regex for this tutorial is used to match characters, numbers & symbols to check for a valid email address.

## Summary

The Regex code that we will be examining today is the following:
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
- [Author](#author)

## Regex Components

### Anchors

The anchor used for this Regex: Start `^` & to finish `$`.

### Quantifiers

For this Regex `+` is used to show there is another sequence to be matching as a greedy quantifier. `{2,6}` is also used. This is a greedy quantifer as well to make sure that the input should be a min of 2 letters, numbers or symbols and a max of 6.

### Grouping Constructs

For the email Regex, the grouping construct is capturing the data. The first group `([a-z0-9_\.]+)` captures the email username. The second group `([\da-z\.-]+)` captures the provider (i.e. gmail, aol, verizon, yahoo ect) of the email. The third group `([a-z\.]{2,6})` captures the domain input from the user.

### Bracket Expressions

For this Regex, bracketed expressions within the validation are inside of `[]` also known as bracket expressions. The first part of the email Regex `[a-z0-9_\.]+)`, anything inside of `[]` will match any letters and numbers within the parameter set which in this case is `a-z & 0-9`. It also can grab the characters `_ , . , -` because they are commonly used in emails as well. For this Regex, there are three sets of `[]` looking for different parts of the email address.

### Character Classes

This expression contains a shing character class of `/d`. This means it will grab any digit between 0-9.

### The OR Operator

The OR operator looks like `|` which is a vertical straight line. It matches the expression before and after it. This quantifier can affect specific characters or expression. For the email Regex, there is none present for validation.

### Flags

Flags are optional arguments that changethe meaning of the expression. An example of this is `i` will tell the Regex search to ignore a capital letter vs a lowercase letter because they are the same thing when searching.

### Character Escapes

Character escapes are used to pick specific characters that an expression could interpret incorrectly or not recognize. They can be used as a shortcut to a specifc string. Character escape can be identified with the `\` forward slash. Some examples of character escapes include `\*\.` which matches a peroid.

## Author

Hello! My name is Adam McLane. I hope this tutorial is helpful in understanding Regex when it comes to email validation. If you have any questions my email is mclanea92@gmail.com. You can also visit my github with the link below.

https://github.com/mclanea92
