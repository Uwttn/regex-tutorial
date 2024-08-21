# regex tutorial

regex is a complex form of JavaScript that allows you to create unique formats depending on the setting that you need it be in.

## Summary

REGEX(1): !/^[a-zA-Z0-9]*$
- Sets a parameter for lowercase "a-z", uppercase "A-Z", and numbers with digits "0-9."

REGEX(2): /^#([A-Fa-f0-9]{6}|[A-Fa-f0-9]{3})$/
- Sets a parameter for colors with a code between uppercase "A-F", colors with lowercase "a-f", and colors with digits between "0-9", while setting a maximum of "six {6} characters", then it repeats itself and sets a minimum of "three {3} characters"

## Table of Contents

- [Regex(1)](#regex1-a-za-z0-9)
    - [Anchors](#anchors )
    - [Quantifiers](#quantifiers )

- [Regex(2)](#regex2-a-fa-f0-96a-fa-f0-93)
    - [Anchors](#anchors)
    - [Quantifiers](#quantifiers)
    - [Grouping Constructs](#grouping-constructs)
    - [Bracket Expressions](#bracket-expressions)
    - [Character Classes](#character-classes)
    - [The OR Operator](#the-or-operator)
    - [Flags](#flags)
    - [Character Escapes](#character-escapes)

# REGEX(1): !/^[a-zA-Z0-9]*$/

## Anchors 
    ^: Asserts the start of a line or string.
    $: Asserts the end of a line or string.

## Quantifiers 
    *: Matches the preceding element zero or more times. In this regex, * allows any sequence of characters within the character class [a-zA-Z0-9] to appear zero or more times.
    Bracket Expressions
    [a-zA-Z0-9]: A bracket expression that defines a character class matching any lowercase letter (a-z), uppercase letter (A-Z), or digit (0-9).
    Character Classes
    [a-zA-Z0-9] is a character class, meaning it matches any single character from the set of lowercase letters, uppercase letters, or digits.

# REGEX(2): /^#([A-Fa-f0-9]{6}|[A-Fa-f0-9]{3})$/

## Anchors
    ^: Asserts the start of a line or string.
    $: Asserts the end of a line or string.

## Quantifiers
    {6}: Matches exactly six occurrences of the preceding character class.
    {3}: Matches exactly three occurrences of the preceding character class.

## Grouping Constructs
    ([A-Fa-f0-9]{6}|[A-Fa-f0-9]{3}): Parentheses are used to create a capturing group. This group matches either six or three characters as defined by the | operator.

## Bracket Expressions
    [A-Fa-f0-9]: A bracket expression defining a character class that matches any uppercase letter (A-F), lowercase letter (a-f), or digit (0-9). 
    
## Character Classes
    [A-Fa-f0-9]: A character class, meaning it matches any single character from the set of uppercase letters, lowercase letters, or digits.

## The OR Operator
    |: The OR operator is used between {6} and {3} within the capturing group. It means the regex can match either exactly six characters or exactly three characters from the specified character class.

## Character Escapes
    #: This is not a character escape, but the # is a literal character that must appear at the beginning of the string, following the start anchor ^.

## Summary
    - REGEX(1): This expression checks if a string consists solely of letters (both cases) and digits. If any character outside [a-zA-Z0-9] appears, it won't match.
    - REGEX(2): This expression checks for a string that represents a valid hex color code, either in the 3-digit or 6-digit format, and it must start with a #.

## Author: Jose Muchati 
- I am a passionate developer with a strong foundation on creating and working on multiple branches via GitHub. My experience includes making logo generators, note taking websites, and to do list websites, and even working in the backend making sure servers are functional via the website. I have used render to publish websites and other projects. And I thrive in a collaborative environment where I can continue learning and refining my skills among other developers.
- [GitHub profile](https://github.com/Uwttn)
- [Link to Gist](https://gist.github.com/Uwttn/f4dec3ffa0043a3e52e8e4da68d56e2d)

