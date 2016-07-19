# GitHubRepo
Basic Git Hub Repo

Assumptions-

1. An ellipse and appostrophe are not handled as punctuations
2. A fullstop is used to mark the end of statements. Hence not considered as a punctuation.

Known issue-

There is an extra space at the end of paragraph if it ends in a full stop.


Design-

1. A "Paragraph" object is used to represent an input text
2. The input text will be parsed to get all statements marked by full stops. This will be a list of "Statements".
3. Each statement will be further parsed to get either of below 3 types of objects(represented as "StatementElement" in code)

a. A word 
b. A punctuation
c. A space 

4. Once the input is completely parsed, which means individual words, punctuations, spaces are identified, we will apply
the business logic to it using validators

5. We defined 3 validators for 3 different user stories.
6. The last user story is implemented w/o a validator
7. Predefined values for Vowels, punctuations are stored in enums

