# Newsletter Content Generator & Quality Control

## Description

Two-stage system for generating newsletter summaries from sources and performing quality control.

## Use Case

- Automated newsletter generation
- Executive summary creation
- Quality assurance for AI-generated content
- HTML-formatted content production

## Implementation Notes

- Two separate prompts: generation and QC
- Produces clean HTML output
- Includes iterative improvement capability
- Multiple prompt versions preserved for reference

---

## Stage 1: Content Generation Prompt

You will get some sources for our Newsletter. Provide a top level summary in HTML: prioritize the most
important sources, be concise, don't be critical but just report facts. For each source you mention,
create a hyperlink to the source, using maximum a couple of words of the sentence for the hyperlink.
Max one sentence per each reported news, but make the discourse flow, it shouldn't be the equivalent of a
list or a bullet point. Add <br><br> in natural places to make it easier to read. Don't make up connections
between the facts, but if two facts share the same subject, connect the sentences to make the period more flowing.

Please present just the source summaries in clean HTML that can be directly inserted into a <div> that I will create,
so don't use divs but just plain text, for line breaks explicit <br><br> and for links <a>s. Maintain objectivity and avoid
any critical analysis or commentary.

[Insert source materials]

---

## Stage 2: Quality Control Prompt

You will get some sources for our Newsletter and a top level summary in HTML.
Your task is to perform a quality check of the top level summary. The summary should only contain the most
important sources, be concise, not critical but just reporting facts. It should be in clean html that can
be directly inserted into a <div> that I will create, so don't use divs but just plain text, for line breaks
explicit <br><br> and for links <a>s.

Your response must contain three elements:

- quality_control: A Boolean (True or False) indicating whether the top level summary meets the requirements.
- suggestions: Any recommendations for corrections or improvements. If you approve the top level summary, just state "Approved, no suggestions".
- text_output: If you provided suggestions, rewrite the top level summary here incorporating those suggestions. If you approved, simply paste the top level.

Sources:
[Insert original sources]

Top Level Summary:
[Insert generated summary to review]
