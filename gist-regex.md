# Regex Tutorial

What is a regex? Regex stands for regular expression. A regular expression is a sequence of characters that define a search pattern.

## Summary

A fun regex I will be explaining is one that can find all words in a string that begin with a certain letter.

## Table of Contents

- [Breakdown](#breakdown)
- [Code Snippet](#code-snippet)
- [Output](#output)
- [Author](#author)

## Regex Components

Lets say we have the following string:

    let string = "The florist loves to plant flowers from the Iris family, specifically freesias"

If we want to find all the words starting with the letter 'f' we can use the regex listed below:
    
    '/\bf\w+/g'

### Breakdown 

Lets breakdown the regex:

    '/\b' matches a word. This is so it only matches words that beginn with the letter 'f'.

    'f' matches the letter 'f'.

    '\w+' matches one or more word characters.

    '/g' is a flag, so we get all the words that begin with 'f' and not just one.

### Code Snippet 

To implement this regex we will use JavaScript code:

    let string = "The florist loves to plant flowers from the Iris family, specifically freesias"
    let regex = /\bf\w+/g;
    let matches = string.match(regex);
    console.log(matches);


### Output

Once you run the javaScript file and open the console/terminal, you would see the following array returned : ['flourist', 'flowers', 'family', 'freesias'].

## Author

My name is Adrienne Cordell I am currently in a full-stack coding bootcamp. If you would like to see more of my work please head over to my Github profile! <a href="https://github.com/adriennecordell">AdrienneCordell at Github</a>. 
