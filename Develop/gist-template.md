# Regex for Emails

This is a simple explanation for a regular expression, or regex, to search for email adresses.

## Summary

The regex below is designed to search for the characters in an order that matches email address patterns. I will be explaining why and how it works in a precise and simple manner.
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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

This regex is wrapped in slash characters, ex. / ----- /. This means the expression is a literal.
That makes the expression only look for the characters inside the expression in the order they are called.

### Anchors

The anchors in this expression are the ^ and $ characters. The ^ character is verifying the beginning of the input is matched and the $ character is verifying the end of the input.

### Quantifiers

Quantifiers in this regex includes the + operator, which will connect the users email name + email service + .com. Another quantifier for this regex includes {2,6}, which will allow a match range of 2-6 characters for the character set of [a-z\.].

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
