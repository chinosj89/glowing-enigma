# Matching an Email - A Regex Tutorial

in this simple tutorial, we will be explaining the use of regex to match emails using this expression <br />
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` 

## Summary

Regular expressions, or regex for short, are a series of special characters that define a search pattern. For this specific tutorial, we will be focusing on the regex that we will call: “Matching an Email”:

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
The Anchors signifies the strings that will follow it and precede it. In this case, the Anchors that indicates the beginning is `^`. While, `$`, indicates the end of the string. 
### Quantifiers
Quantifiers sets the limits of the string that the regex matches. 
- `{2,6}`
    - this matches the patter from a minimum numbers of 2 and a maximum number of 6
### OR Operator
This Regex does not contain any OR operators
### Character Classes
Character classses defines a set of characters that can occur in an input string to fullfill the match. 
- `\d` 
    - This matches any single digit numbers from 0-9
### Flags
This Reges does not contain any flags
### Grouping and Capturing
- `([a-z0-9_\.-]+)` 
    - This matches the user's email name
- `([\da-z\.-]+)`
    - This matches the user's email service
- `([a-z\.]{2,6})`
    - This matches the user's email service's domain extension
### Bracket Expressions
Bracket Expressions are a range of characters that we want to match within `[]`. In the case of Matching an Email, we see these Bracket Expression 3 times. 
- `[a-z0-9_\.-]` 
    - Letters between a-z. Please note that this is only for lowercase letters. 
    - Numbers between 0-9
    - Special Characters: "_", "-", and "."
- `[\da-z\.-]`
    - Letters between a-z. Please note that this is only for lowercase letters. 
    - Numbers between 0-9
    - Special Characters: "-" and "."
- `[a-z\.]`
    - Letters between a-z. Please note that this is only for lowercase letters.
    - Special Characters: "."
### Greedy and Lazy Match
Greedy matches that are included in this Regex are as follows:
- `+`
    - This is also know as "As Many As Possible"
    - This allows the engine to match one or more of the token it quantifies
    - In this regex it allows the user to use as many alphanumerics as possible
### Boundaries
Boundaries are used to specify where in the input string a match should occur. There are no Boundaries in this Regex
### Back-references
Back-references allow you to match the same text as captured by a capturing group earlier in the regex. There are no Back-references in this Regex
### Look-ahead and Look-behind
Lookaheads and lookbehinds are used to check if a certain pattern is (or is not) followed by another pattern, without including the second pattern in the match. There are none of these in the Regex
## Author
Hi! My name is Raphael SanJuan. This is my github: https://github.com/chinosj89 
