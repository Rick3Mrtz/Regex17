# Regex17

# Description

Regex (Regular Expression) can be used for validations of multiple aspects in the coding world.

# Topic at hand

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

Do you know what the expression above represents? If not, read to find out more! We can break the expression down piece by piece as well.

# Summary

Lets find out how the regex stated above that is commonly used to match and validate email addresses in a format that conforms to common standards.

/ and / denote the start and end of the regex pattern.
^ and $ denote the start and end of the string being matched, respectively.
Now let's look at the pattern inside the slashes:

([a-z0-9_\.-]+) matches one or more characters that are lowercase letters, digits, underscores, dots or hyphens, and captures them in a group. This is the username part of the email address.

@ matches the @ symbol that separates the username from the domain name.
([\da-z\.-]+) matches one or more characters that are digits, lowercase letters, dots or hyphens, and captures them in a group. This is the domain name part of the email address.

\. matches a literal dot (.), which separates the domain name from the top-level domain (TLD).

([a-z\.]{2,6}) matches between 2 and 6 characters that are lowercase letters or dots, and captures them in a group. This is the TLD part of the email address.


So in summary, the regex pattern /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ matches email addresses in the format of "username@domainname.tld", where the username contains only lowercase letters, digits, underscores, dots or hyphens, and the domain name and TLD contain only lowercase letters, digits, dots or hyphens, with the TLD being between 2 and 6 characters long.

