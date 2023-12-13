---
date: 2023-12-12
title: Prompt 005
based on: prompt-004
changes:
    - Provide more specific names and descriptions for columns
    - Specify several new columns (features) for the output
    - Specify output to be CSV and pipe separated
    - Organize output instructions to be in it's own section
    - Change "Output Requirements" to "Output Format Requirements"
---

The following lists relevant contextual details about a scenario:

- Culture: America
- Situation: A man is being called in to work overtime on a national holiday. He is talking with his boss. He doesn't want to go into work, but his boss threatens him by saying, "If you don't come, you're fired."

Output Instructions:
    - List 5 pragmatically appropriate and 5 pragmatically inappropriate responses for this scenario.
    - The responses must logically fit the scenario.
    - Do not write any commentary or summaries.
    - You can include vulgar responses.
    - Expletives can be included and should be written out. Do not omit expletives with a substitution.

Output Format Requirements:
    - Write the output as CSV with a pipe (|) as the delimiter
    - Do not wrap the response in double quotes
    - The output should be in a codeblock
    - The table columns are listed here as the name and description. Only use the name in the output:
        - Number: The number of the response
        - Response: The response given
        - Suitability: Is it an appropriate or inappropriate response?
        - Intent/Strategy: The intended meaning or purpose behind the speaker's utterance or the strategy employed
        - Illocutionary Force: The speaker's intended communicative function or speech act
        - Emotion/Tone: The emotional tone or attitude expressed in the utterance.
        - Politeness Level: Degree of politeness in the response (Rude, Casual, Polite, Respectful, Formal)
        - Humor: Presence and type of humor in the response (if any)
