# Cover letter generator

To use this prompt most effectively, be sure to have your CV as the job description ready in text form (copy-paste). This prompt
will help you generate a nice motivation letter. Any places where you need to copy-paste content below is market with < ... >

The full procesdure is cut into a few (clearly marked below) prompts to avoid using too many tokens at once.


// PROMPT 1 START //

Please carefully read my CV below, as I will ask you to help me with career advice, write letters, etc. based on this and other information. 
Do not hallucinate or provide information that is not accurate just to make things sound better. Do not react until I ask you questions, when you finished reading say "OK".

< copy the text of your CV here >

Here is the job description of a position I am interested in. Read it carefully, do not react until I 
ask you questions, when you finished reading say "OK".

< copy the job description here >

// PROMPT 1 END //

At this point, the system will simply react with the word "OK". The we go to the next prompt.

// PROMPT 2 START //

Based on my background, as you read in my CV, what do you think? Should I apply? If yes, what are the strong points and the weak points of my CV and how to optimize my application?

// PROMPT 2 END //

At this point, you will get a nice analysis of the "job-CV fit" - this is only to induce the system to "think" about those points before asking it for a nice cover letter.

// PROMPT 3 START //

Thank you. Based on the points you made above, can you now prepare a cover letter for me?
The company's name is < company name > and the recruiter's name is < name, if available >.

// PROMPT 3 END //

Done. From my experience, the system will generate already at this point a very good letter, you may need to adjust it a bit to your voice, but otherwise it saves a lot of
time and work.


