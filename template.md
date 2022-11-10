# Email Regex by Tutorial Legend

#### Welcome to Tutorial Lengend! This tutorial will help you understand the regex provided in the summary below. We will be going over how the regex works by explorying it's structure.

## Summary
#### The regex shown will provid the abuility to search for email addresses. It will use specific criteria to narrow down the search and identify what is and what is not concidered an email address. We will be able to sort through all sorts of random strings and tell what is a correct address!

#### This is the regex we will be going over today: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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
#### Let's identify the first and last characters in the regex. At the very beginning, you will notice the character "^". <br/> This character will tell the regex, this is the first point in the string, <br/> however this is only the case when accompanied by the "$" at the end, [whcih] you will notice at the end of the regex. <br/> This brings us to the last character, "$". <br/> When accompanied by the "^" at the beginning, both these symbols identify the beginning and end points <br/> of the string, as interpreted by the regex. Therefore, "^" combined with "$" will tell the regex that anything between the two symbols will be our string, but the "^" must be at the beginning, and "$" at the end. <br/> This is an example of a regex anchor. Anchors don't match any characters, <br/> but assert something about the string, or matching process. They provide structure for the rest of the characters.


### Quantifiers
#### Quantifiers are symbols that indicate a token must be matched a certain number of times. By default, quantifiers are greedy, which means they match as many characters as possible. An example of a quantifier in our regex is the "+" sign which is meant to match 1 or more of the preceding tokens. If we were to make our quantifier lazy, we could simply place a "?" at right after the quantifier. In our case, to the right of the "+" sign. This would cause it to repeat the minimal number of times.

### OR Operator
#### The OR operator functions how you might expect it to. It allows a choice between criteria depending on the search result. If one set of criteria is not found, but the other is, we can use an OR operator, "|", to create a second route. <br/> Emaple: ((^|, )(part1|part2|part3))+$ . <br/> Our regex doesn't have an example of this, so we will move on.

### Character Classes
#### Character classes can be identified by the brackets enclosing them. The characters inside a bracket expression are referred to as "Character Classes". <br/> Example: [xyz]. In this case, the Character class matches any one enclosed character, ie, x, y, or z. A range of characters can be found by using a dash between characters, [a-z]. In our regex above you can see each range enclosed by brackets. <br/> [a-z0-9_\.-], [\da-z\.-], [a-z\.]. As you can see here, we have a range of letters, a-z, a range of numbers, 0-9, etc. 

### Flags
#### Flags are ways to narrow the search by adding broad criteria such as having a search be case-insensitive. <br/> There are six flags: global, case insensitive, multiline, single line (dotall), unicode, and sticky. To define a few, case insensitive allows for the search to see capital A and lowercase a as the same for example.<br/> Sticky: If sticky is chosen, it will only match from its lastIndex position and ignores the global flag if set. 

### Grouping and Capturing
#### These can be identified by using "()" to enclose Character sets. In our regex you can see three examples of this. They are used to group multiple tokens.

### Bracket Expressions
#### Bracket Expressions enclose Character Classes such as [abc], [0-9], [d\]. In out regex we have three examples. And each are enclosed in a Capturing group.

### Greedy and Lazy Match
#### A Greedy Match is used by quantifiers. When a match is greedy is will try to match as many sets as possible. It's opposite is the lazy match. A lazy match will cause the match to repeat the minimal number of times. Matches are normally greedy by default. If you were to make a match lazy, you would place "?" to the right of a quantifier.

### Boundaries
#### Using a previouse example, "^" and "$", set at the beginning and end of the regex can be considered boundry markers. They provide a reference point for the regex. The forward slash is also a boundry, as seen here in this example: /^[A-Z]$/.

### Back-references
#### Back-References are regular expression commands which refer to a previous part of the matched regex. They are specified using a backslash followed by a number. <br/> Example: "\1". <br/> There are no back-references in our regex.

### Look-ahead and Look-behind
#### Both of these collectively are called "lookaround". Both lookahead and lookbehind have positive and negative versions. "Positive lookahead" Matches a group after the main expression without including it in the result, "Negative lookahead" will specify a group that can't match after the main expression, and if it does match, it will be discarded. <br/> "Positive lookbehind" Will match a group before the main expression without including it in the result, and " "Negative lookbehind" will specify a group that can't match before the main expression. Just like the Negative lookahead, the Negative lookbehind will discard any matches. There are no examples of a lookaround in our regex.

## About the Author

#### Josiah Stelzl is an amateur full stack web developer with experience in JavaScript, HTML, CSS, GIT, Node, Express, and SQL. 
#### Examples of the author's work can be found by visiting the provided GitHub link below or the author's portfolio.
####  Josiah Stelzl's portfolio: https://jstelzl.github.io/portfolio/
#### Josiah Stelzl's GitHub: https://github.com/Jstelzl