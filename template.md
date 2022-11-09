# Title (replace with your title)

#### Welcome to Tutorial Lengend! This tutorial will help you understand the regex provided in the summary below. We will be going over how the regex works by explorying it's structure.

## Summary
#### The regex shown will provid the abuility to search for email addresses. It will use specific criteria to narrow down the search and identify what is and what is not concidered an email address. We will be able to sort through all sorts of random strings and tell what is a correct address!

#### This is the regex we will be going over today: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
<!-- Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary. -->

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
#### Basic Elements: \   .   $   *   ?   +  [ ]   (   )   | <br/> Qualifying Characters: *   +   ?

### Anchors
#### Let's identify the first and last characters in the regex. At the very beginning, you will notice the character "^". <br/> This character will tell the regex, this is the first point in the string, <br/> however this is only the case when accompanied by the "$" at the end, whcih you will notice at the end of the regex. <br/> This brings us to the last character, "$". <br/> When accompanied by the "^" at the beginning, both these symbles identify the beginning and end points <br/> of the string, as interpreted by the regex. Therefore, the structure of \^ $\ will tell the regex that anything between the two symples will be our email criteria.

### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## About the Author

#### Josiah Stelzl is an amateur full stack web developer with experience in JavaScript, HTML, CSS, GIT, Node, Express, and SQL. 
#### Examples of the author's work can be found by visiting the provided GitHub link below or the author's portfolio at: https://jstelzl.github.io/portfolio/
 
#### Josiah Stelzl's GitHub: https://github.com/Jstelzl
<!-- A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile) -->
