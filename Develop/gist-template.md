# Regex-Tutorial

This Page will guide the user on how to use the following expressions. 

## Summary

this snippit is what a regular expression or regex looks like to match a URL

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

the expression above is checking to see if the string containing all the required characters is of a valid URL. every component in this code will be broken down and explained. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors
Anchors match a position of a character. They're use to define where in the code a match should occur. 

^ ( this carrot is similar to the first character of a string)

& (likewise this dollar sign represents the last character of the string)

### Quantifiers
Quantifiers are used to identify occurrences of a character or a set of characters within a text. They define the frequency with which the preceding character or group of characters should appear. These quantifiers can be integrated with other elements in regular expressions to construct intricate patterns.

The asterisk denotes 0 or more occurrences of the preceding element.

The plus sign signifies 1 or more instances of the preceding element.

?
The question mark indicates 0 or 1 occurrence of the preceding element.

{4,8}
This specific quantifier dictates that the preceding pattern must appear at least 4 times but no more than 8 times.


### OR Operator
The OR Operator, denoted by the pipe symbol (|), is employed when searching for alternative patterns outside of a bracket expression. This proves useful when seeking variations in strings or numbers.

Examples:

(yes|no) matches either 'yes' or 'no'.

(1|2|3) matches 1, 2, 3, and even 321.

### Character Classes
Character classes establish a set of characters, and a match is valid if any character from that set is present.

\d
This class validates any numerical digit, equivalent to [0-9].

\w
This class matches any alphanumeric character from the basic Latin alphabet, including the underscore (_), equivalent to [A-Za-z0-9].

### Flags
Flags are positioned at the end of a regex and alter the functionality of the expression.

g
The global flag facilitates searching for all occurrences, not just the first one.

i
The case-insensitive flag allows matching without considering case differences.

m
The multi-line flag supports searching across multiple lines.

### Grouping and Capturing
Grouping constructs serve to combine characters together, achieved through the use of parentheses. Employing these constructs enables the treatment of one or more characters as a unified entity.

(https?://)?
This group is optional and corresponds to the URL protocol, for instance, 'http://'.

([\da-z.-]+)
This group identifies the subdomain and second-level domain in a URL, like 'post.techblog'.

([a-z.]{2,6})
This group captures the top-level domain, as seen in examples like '.com'.

([/\w .-])
This group matches any potential instances of a page path, if applicable, such as '/business'.

### Bracket Expressions
Bracket expressions are utilized to specify a range of character matches, and they are denoted by square brackets.

[\da-z.-]
This expression is designed to match any digit (\d or [0-9]), any single character in the range a-z (case-sensitive), and any instances of '.' or '-' characters.

[a-z.]
This expression targets any single character in the range a-z (case-sensitive) and a '.' character.

[/\w .-]
This expression captures any word character (equivalent to [a-zA-Z0-9_]) and occurrences of '/', whitespace, '.', or '-' characters.

## Author
This tutorial was creted by Rajvir Chaggar. a aspiring full-stack developer. a recent and passionate programming enthusiast. Feel Free to search my GitHub profile for more exciting tutorials and project that i have worked on! if you have any feedback or questions please reach out to me on GitHub. Username: Chaggar25 
