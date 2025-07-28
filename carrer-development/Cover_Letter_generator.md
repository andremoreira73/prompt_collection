# Cover Letter Generator

## Description

A multi-step process that analyzes CV-job fit and generates tailored cover letters by understanding both the candidate's background and the position requirements.

## Use Case

- Job application preparation
- Career transition support
- Highlighting relevant experience for specific roles
- Overcoming application weaknesses
- Time-saving for multiple applications

## Implementation Notes

- Three-step process for optimal results
- First reads CV and job description
- Analyzes fit before generating letter
- Produces personalized, position-specific content

---

## PROMPT 1

Please carefully read my CV below, as I will ask you to help me with career advice, write letters, etc. based on this and other information.
Do not hallucinate or provide information that is not accurate just to make things sound better. Do not react until I ask you questions, when you finished reading say "OK".

<copy the text of your CV here>

Here is the job description of a position I am interested in. Read it carefully, do not react until I ask you questions, when you finished reading say "OK".

<copy the job description here>

[Wait for "OK" response]

## PROMPT 2

Based on my background, as you read in my CV, what do you think? Should I apply? If yes, what are the strong points and the weak points of my CV and how to optimize my application?

[Wait for analysis]

## PROMPT 3

Thank you. Based on the points you made above, can you now prepare a cover letter for me?
The company's name is <company name> and the recruiter's name is <name, if available>.
