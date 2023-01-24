# Regex Tutorial for Email Match

This is a simple explanation for a regular expression, or regex, to search for email adresses.

## Summary

The regex below is designed to search for the characters in an order that matches email address patterns. I will be explaining why and how it works in a precise and simple manner.
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

This regex is wrapped in slash characters, ex. / ----- /. This means the expression is a literal.
That makes the expression only look for the characters inside the expression in the order they are called.

### Anchors

The anchors in this expression are the `^` and `$` characters. The `^` character is verifying the beginning of the input is matched and the `$` character is verifying the end of the input.

### Quantifiers

The quantifiers in this regular expression are the `+` operator, which will connect the users email name + email service + `.com`. The other quantifier for this regex includes `{2,6}`, which will allow a match range of 2-6 characters for the character set of `[a-z\.]`.

### Character Classes

The character class in this expression is `\d`, which will only match a single character that is a digit from 0-9. An example of this would be, it is able to find the single "5", but not "55".

### Grouping and Capturing

The first capturing group in this expression is `([a-z0-9_\.-]+)` that matches the user email name. The second capturing group is `([\da-z\.-]+)` which will match the email service. Then lastly, capture group #3 is `([a-z\.]{2,6})` to capture the `.com` or any other finalizers in an email such as `.net`, `.edu`, or `.gov`.

### Bracket Expressions

Bracket expressions for email validation includes the character sets of `[a-z0-9_\.-]`, which is matching any letter a-z and is case senstive. It also matches a character 0-9 and matches the characters "\_" , "-" , and "."; `[\da-z\.-]`, which is matching a single digit from 0-9, any character a-z (case senstive), and the characters "." and "-".; `[a-z\.]` matches any character a-z(case senstive) and the character ".".

### Greedy and Lazy Match

This regular expression does include greedy matches. It includes the `+` Quantifier, so it will match as many times as possible giving back as needed. The other greedy Quantifier used in this regex is `{}` when matching `{2,6} for the final capture group.

## Author

My name is Zane Nichols and my github profile is https://github.com/NicholsZane13.
