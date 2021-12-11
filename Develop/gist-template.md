# Langdons-Regex-tutorial
the purpose of this is to learn and understand regex in a form where i can then explain it to someone who knows nothing about it
## Summary
this would be an example of regex in the form of an email verification
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#Character-Classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors
The anchors used in this regex expression for matching an email are ^ , which indicates the beginning of the string and $to indicate the ending of the string. (m) or it saying that the multiline is not enabled, so the regex will end at $.
### Quantifiers
Quantifiers in this regex includes the + operator, which will connect the users email name + email service + .com. Another quantifier for this regex includes {2,6}, which will allow a match range of 2-6 characters for the character set of [a-z\.].
### Character Classes
The character class in this expression is \d, which matches a single characters that is a digit from 0-9. It will only match a single digit such as "4", but not "44".
### Grouping and Capturing
Capturing group #1 in this expression is ([a-z0-9_\.-]+) that matches the user email name. The second capturing group is ([\da-z\.-]+) which will match the email service. Then lastly, capture group #3 is ([a-z\.]{2,6}) to capture the .com.
### Greedy and Lazy Match
This regex includes greedy matches. Since it includes the + Quantifier, it will match as many times as possible giving back as needed in which giving it the name greedy. Another greedy Quantifier used in this regex is {} when matching `{2,6} for the last capture group.
### Bracket Expressions
Bracketed expressions for email validation includes the character sets of [a-z0-9_\.-], which is matching any letter a-z and is case sensitive. It also matches a character 0-9 and matches the characters "_" , "-" , and "."; [\da-z\.-], which is matching a single digit from 0-9, any character a-z (case sensitive), and the characters "." and "-".; [a-z\.] matches any character a-z(case sensitive) and the character ".".
## Author
I am Langdon Echols a new fullstack developer starting in the UT coding bootcamp 
