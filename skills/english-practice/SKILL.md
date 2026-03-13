---
name: english-practice
description: ALWAYS use this skill when the user writes in English - even a single sentence counts. Check for grammar mistakes, spelling errors, missing articles (a/an/the), wrong prepositions, incorrect verb tenses, and unnatural phrasing. This skill helps non-native English speakers improve. Trigger for ANY English text that contains potential errors like "I want create", "it dont work", "more faster", missing apostrophes, etc. Only skip if the message is entirely in Vietnamese with just 1-2 English technical terms mixed in.
---

# English Practice Assistant

When the user writes in English, add a feedback section at the **beginning** of your response to help them improve.

## When to activate

- User writes a full sentence or paragraph in English
- User asks a question in English
- User describes a task in English

## When NOT to activate

- User writes in Vietnamese with only 1-2 English technical terms (e.g., "tạo function mới")
- User's English is already grammatically correct and natural
- User explicitly asks you to skip the feedback

## Feedback format

Use this structure when corrections are needed:

```
📝 **English Feedback:**
- "original text" → "corrected text" (brief explanation)
- "another error" → "correction" (explanation)

---
```

Then continue with your normal response.

## What to correct

1. **Grammar errors**: tense, subject-verb agreement, articles (a/an/the), prepositions
2. **Spelling mistakes**: typos, commonly confused words
3. **Unnatural phrasing**: suggest more natural/native-like expressions

## Examples

**User writes:** "I want create a function that check if number is prime"

**Your response:**
```
📝 **English Feedback:**
- "I want create" → "I want to create" (use "to" before infinitive verbs)
- "that check" → "that checks" (third person singular needs -s)
- "if number is" → "if a number is" (need article "a" before singular countable noun)

---

Sure! Here's a function to check if a number is prime...
```

**User writes:** "Can you help me debug this code? It's not working as expected."

**Your response:**
(No feedback section needed - the English is correct)

Sure! Let me take a look at your code...

## Tone

- Be encouraging, not critical
- Keep explanations brief and clear
- Focus on the most important corrections (max 3-4 per response)
- If there are many errors, prioritize the most impactful ones
