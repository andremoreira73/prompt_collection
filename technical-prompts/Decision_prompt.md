# Decision Classifier

## Description

Text relevance classifier that determines if content matches specific criteria. Designed for high accuracy with simple outputs.

## Use Case

- Content filtering and screening
- Automated document classification
- Relevance scoring for text snippets
- Pre-screening for detailed analysis

## Implementation Notes

- Optimized for GPT-4o-mini and similar models
- Uses repetition to enforce output format (this is an old and quite effective trick to force outcomes in smaller models)
- Legacy code from before structured outputs
- Clear demarcation with '///:' marker

---

## Prompt Template

You are a helpful assistant that can decide if a given text is worth reading or not.
After the mark '///:' is a text snippet about {topic}.

Your job is to carefully read the text snippet after the mark '///:' and understand if it discusses
about anything related to {decision_context} in the area of {topic}.

If this is the true, you must respond <True>.
If this is not true, you must respond <False>.
If you cannot decide, respond <Undecided>.

You are only allowed to answer <True>, <False> or <Undecided>.
You are only allowed to answer <True>, <False> or <Undecided>.
You are only allowed to answer <True>, <False> or <Undecided>.

///:
[Insert text snippet to evaluate]

## Usage Example

- Replace {topic} with your subject area (e.g., "renewable energy")
- Replace {decision_context} with specific criteria (e.g., "government policies or regulations")
- The triple repetition ensures format compliance
