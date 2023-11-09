# Title (replace with your title)

Title: Regex Tutorial\_ Matching an Email

Introduction:
Welcome to the "Regex Tutorial: Matching an Email." In this tutorial, we will delve into the regular expression (regex) pattern used to validate and extract email addresses from text data. Understanding this regex will help you work with email-related tasks more effectively.

## Summary

This tutorial will focus on a specific regex pattern designed to match valid email addresses. We will break down each component of the regex, explaining its purpose and how it contributes to the overall pattern.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)

- [Grouping and Capturing](#grouping-and-capturing)

## Regex Components

^

@ - Matches the '@' symbol, which separates the local part from the domain part of the email.

[\da-z\.-]+ matches one or more characters that are digits (0-9), lowercase letters (a-z), period (.), or hyphen (-). This allows for a wide range of characters in the domain part of the email.

$ - Anchors the regex at the end of the string.




### Anchors
 - Anchors the regex at the beginning of the string.
([a-z0-9_\.-]+) - This is the first capturing group. It matches the local part of the email address, which is the part before the '@' symbol. Breaking it down further

### Quantifiers
\.([a-z\.]{2,6}) - This part matches the top-level domain (TLD) of the email address, which is the part after the last dot (.). Breaking it down further:
\.([a-z\.]{2,6}) matches a dot (.) followed by 2 to 6 characters that are lowercase letters (a-z) or a period (.). This enforces that the TLD is between 2 and 6 characters.




### Character Classes
[a-z0-9_\.-]+ matches one or more characters that are lowercase letters (a-z), digits (0-9), underscore (\_), period (.), or hyphen (-). This allows for a wide range of characters in the local part of the email.



### Grouping and Capturing
([\da-z\.-]+) - This is the second capturing group. It matches the domain part of the email address. Breaking it down further







## Author

This tutorial was written by Vanessa Decopin, a software developer with a passion for building websites. You can learn more about me and explore additional resources om my GitHub profile: https://github.com/v4nessa44

The local part (before '@') can contain lowercase letters, digits, underscores, periods, and hyphens.
The domain part (after '@' and before the last dot) can contain digits, lowercase letters, periods, and hyphens.
The top-level domain (TLD) is restricted to 2 to 6 characters and can only contain lowercase letters and periods.



