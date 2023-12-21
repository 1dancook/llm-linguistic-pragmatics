# set-01

- llm: chatGPT
- llm-version: 3.5

The purpose of this set is to determine if chatGPT will produce a number of pragmatic (inappropriate or appropriate) responses to a scenario.

Expectations:

- it should produce a table with a number of variables
- it should produce a wide range of pragmatic responses


## prompt-001

- date: 2023-12-07

### Prompt

The following lists relevant contextual details about a scenario:

- Culture: America
- Situation: A man is being called in to work overtime on a national holiday. He is talking with his boss. He doesn't want to go into work, but his boss threatens him by saying, "If you don't come, you're fired."

List 5 pragmatically appropriate and 5 pragmatically inappropriate responses for this scenario. You can include vulgar responses.

### Response

Pragmatically Appropriate Responses:

1. **Polite Request:**
   - "I understand the urgency, but is there any way we can discuss an alternative solution that doesn't involve me working on the holiday?"

2. **Negotiation:**
   - "I'm willing to help out in this situation, but can we work out some compensation or time off in lieu for working on a national holiday?"

3. **Expressing Concern:**
   - "I have prior commitments, but if it's absolutely necessary, I'll do my best to rearrange things. Can we discuss the details and find a compromise?"

4. **Compliance with Conditions:**
   - "I'll come in for overtime on the holiday, but can we confirm that my dedication to the job will be acknowledged and reflected appropriately?"

5. **Seeking Clarification:**
   - "I want to make sure I fully understand the situation. Can you provide more information on why my presence is crucial on the national holiday and if there are any alternatives?"

Pragmatically Inappropriate Responses:

1. **Defiance:**
   - "I don't care if you fire me. I'm not working on a damn holiday!"

2. **Insulting the Boss:**
   - "You must be out of your mind if you think I'm sacrificing my holiday for this crap. Find someone else, idiot."

3. **Ignoring the Request:**
   - *No response, simply ignoring the request or not acknowledging it.*

4. **Passive-Aggressive Response:**
   - "Sure, I'll come in and ruin my holiday just to make you happy. Great way to show appreciation for your employees."

5. **Inappropriate Humor:**
   - "You want me to work on a holiday? Is this a joke? Did I accidentally sign up for a stand-up comedy show?"


### Observations/Thoughts


- The LLM was prompted for appropriate and inappropriate responses
    - The inappropriate responses seemed to assume certain things about the employee
    - Next: It may be important to give more relevant context

- It classified the responses with the strategy it employed without being asked (is this desired?)

- The output format is not nice - would be great to be in a table format

- It's not very vulgar, but maybe the context provided doesn't quite warrant it (i.e. why would the man be vulgar?)

**Thought**: The more context given, the more fitting the responses will be.

#### For next prompt:

- specify output format (table with columns, etc.)
- specify not adding any commentary or summary
- specify adding the strategy it employs
- specify MORE context for the man (maybe about what is happening at home)


## prompt-002

- date: 2023-12-12
- based on: prompt-001
- changes:
    - specify output format (table with columns, etc.)
    - specify not adding any commentary or summary
    - specify adding the strategy it employs

### Prompt

The following lists relevant contextual details about a scenario:

- Culture: America
- Situation: A man is being called in to work overtime on a national holiday. He is talking with his boss. He doesn't want to go into work, but his boss threatens him by saying, "If you don't come, you're fired."

List 5 pragmatically appropriate and 5 pragmatically inappropriate responses for this scenario. You can include vulgar responses. Include the strategy employed.

Do not write any commentary or summaries.

Output Requirements:

- write the output as a tab separated table (TSV)
- the table columns will be "Response", "Strategy", "Suitability"
- the output should be in a codeblock

### Response

- notes:
    - formatting was applied because the output table had an incorrectly formatted heading
    - reformatted to be a markdown table


| Response                                                                           | Strategy                   | Suitability   |
| --------                                                                           | --------                   | -----------   |
| 1. "Sure, I understand the urgency. I'll come in."                                 | Compliance/Agreeing        | Appropriate   |
| 2. "I have personal plans, but I can rearrange them if it's absolutely necessary." | Negotiation                | Appropriate   |
| 3. "I won't be able to make it, but can we discuss compensatory time off?"         | Negotiation/Assertiveness  | Appropriate   |
| 4. "This is unfair, and you can't threaten me like that!"                          | Assertiveness/Disagreement | Inappropriate |
| 5. "Hell no, I won't come in! You can't fire me for this!"                         | Defiance/Aggressiveness    | Inappropriate |
| 6. "I'll be there, but this better come with a fat bonus."                         | Compliance/Demanding       | Appropriate   |
| 7. "You're out of your mind if you think I'm working today."                       | Disagreement/Defiance      | Inappropriate |
| 8. "Alright, but I expect double pay for this inconvenience."                      | Compliance/Negotiation     | Appropriate   |
| 9. "I quit! Find someone else to ruin their holiday."                              | Quitting/Defiance          | Inappropriate |
| 10. "I can't make it today. Fire me if you must."                                  | Resignation/Defiance       | Inappropriate |


### Observations/Thoughts

- The output was not done correctly (I asked for TSV, it gave me space separated values)
- Responses seemed shorted than 001
- As expected, responses are generally different than 001
- Specifying no commentary/summary seemed to have worked (The only output was the table)
- The strategy specified in 002 was more general than 001 (which would be more useful for categorization)

#### A look at responses (are we getting roughly the expected results?)
- Response 3 is not fitting to the situation. Compensatory time off would only be negotiable if he went in to work.
- Response 4 is not necessarily inappropriate but depends on the manner of speaking and further context.
- Response 6 is tagged as "appropriate". Depending on the manner of speaking this could be inappropriate.

#### For next prompt
- specify a column for the response number
- specify the output format to be a markdown table
- specify not to quote the response
- specify the speaking mode
- specify that the response must logically fit the situation


## prompt-003

- date: 2023-12-12
- based on: prompt-002
- changes:
    - specify a column for the response number
    - specify the output format to be a markdown table
    - specify not to quote the response
    - specify the speaking mode
    - specify that the response must logically fit the situation

### Prompt

The following lists relevant contextual details about a scenario:

- Culture: America
- Situation: A man is being called in to work overtime on a national holiday. He is talking with his boss. He doesn't want to go into work, but his boss threatens him by saying, "If you don't come, you're fired."

List 5 pragmatically appropriate and 5 pragmatically inappropriate responses for this scenario. You can include vulgar responses. Include the strategy employed.

The responses must logically fit the scenario.

Do not write any commentary or summaries.

Output Requirements:

- write the output as markdown formatted table
- the table columns will be "Response Number", "Response", "Strategy", "Suitability", "Speaking Mode"
- do not quote the response
- the output should be in a codeblock

### Response

| Response Number    | Response                                                                                                              | Strategy                               | Suitability                 | Speaking Mode       |
| ------------------ | -------------------------------------------------------                                                               | -----------------------------          | --------------------------- | ------------------  |
| 1  | "Sure, I understand the urgency. I'll come in for overtime."                                                                          | Compliance/Agreeing                    | Appropriate                 | Polite              |
| 2  | "I have personal commitments today, but I can work extra hours tomorrow to make up for it."                                           | Compromise                             | Appropriate                 | Diplomatic          |
| 3  | "I appreciate the offer, but I had made plans for the holiday. Is there any way we can find an alternative solution?"                 | Assertive/Requesting                   | Appropriate                 | Professional        |
| 4  | "I can't believe you're pulling this on a national holiday. This is ridiculous!"                                                      | Expressing Displeasure                 | Inappropriate               | Emotionally Charged |
| 5  | "Well, if that's how it is, maybe it's time for me to start looking for a new job. Threatening job security on a holiday isn't fair." | Challenging/Expressing Dissatisfaction | Appropriate                 | Assertive           |
| 6  | "You can't fire me for this. This is [expletive] unfair!"                                                                             | Defensiveness/Expressing Anger         | Inappropriate               | Aggressive          |
| 7  | "How about you come in and do the work yourself if it's so important? I'm not your slave."                                            | Defiance/Counter-Threatening           | Inappropriate               | Aggressive          |
| 8  | "Fine, I'll come, but you're ruining my [expletive] holiday."                                                                         | Compliance/Expressing Displeasure      | Inappropriate               | Resigned            |
| 9  | "You know what? I quit! I'm not putting up with this [expletive] anymore."                                                            | Resignation/Quitting                   | Inappropriate               | Defiant             |
| 10 | "I'll be there, but you owe me big time for this."                                                                                    | Compliance/Negotiating                 | Appropriate                 | Assertive           |


### Observations/Thoughts

- The expected results for the `Speaking Mode` column were categories like "yelling", "whispering", etc.
    - **Thought:** The idea for `Speaking Mode` was to get have more context about the response itself. ChatGPT produced a discourse type. A `Discourse Type` may be more useful as a category than a speaking mode.

- Rather than writing out expletives, ChatGPT 'muted' them with `[expletive]`.
    - **Question**: Will ChatGPT produce expletives if instructed to do so?

- The markdown formatted table worked along with all of the specified columns.

- ChatGPT did not listen to instructions about not quoting the responses.

#### Notes on the responses
- Response 3 is not fitting. There is no offer being made.

#### For Next Prompt

- change `Speaking Mode` column name to `Discourse Type`
- specify that explitives can be included and should be written out

#### For Another Prompt
- Get the output into CSV format with the delimiter as a pipe character ("|")


## prompt-004

- date: 2023-12-12
- based on: prompt-003
- changes:
    - change `Speaking Mode` column name to `Discourse Type`
    - specify that explitives can be included and should be written out
    - change instruction about quoting response to be more specific

### Prompt

The following lists relevant contextual details about a scenario:

- Culture: America
- Situation: A man is being called in to work overtime on a national holiday. He is talking with his boss. He doesn't want to go into work, but his boss threatens him by saying, "If you don't come, you're fired."

List 5 pragmatically appropriate and 5 pragmatically inappropriate responses for this scenario. You can include vulgar responses. Include the strategy employed.

The responses must logically fit the scenario.

Do not write any commentary or summaries.

Expletives can be included and should be written out. Do not omit expletives with a substitution.

Output Requirements:

- write the output as markdown formatted table
- the table columns will be "Response Number", "Response", "Strategy", "Suitability", "Discourse Type"
- do not wrap the response in double quotes
- the output should be in a codeblock


### Response

| Response Number | Response | Strategy | Suitability | Discourse Type |
|------------------|----------|----------|--------------|-----------------|
| 1                | "I understand the urgency, but I already have plans for the holiday. Is there any way we can find an alternative solution, like having someone else cover the shift?" | Politeness and Negotiation | Appropriate | Assertive |
| 2                | "I'm committed to my job, but working on a national holiday is challenging. Can we discuss compensation or additional time off as a compromise?" | Diplomacy and Compromise | Appropriate | Collaborative |
| 3                | "I'm really not comfortable with coming in on a holiday. Is there a specific reason it's necessary, and can we explore other options before considering termination?" | Seeking Explanation and Problem Solving | Appropriate | Assertive |
| 4                | "I can appreciate the importance of the task, but being threatened with termination feels extreme. Can we have a more constructive conversation about finding a solution that works for both of us?" | Addressing the Threat and Suggesting Collaboration | Appropriate | Assertive |
| 5                | "I'm willing to work, but firing me for not coming in on a holiday seems unreasonable. Can we discuss the company policy on this matter and explore alternatives?" | Referencing Company Policy and Seeking Alternatives | Appropriate | Assertive |
| 6                | "This is [expletive] ridiculous! You can't just threaten to fire me for not working on a [expletive] holiday!" | Expressing Frustration and Disapproval | Inappropriate | Aggressive |
| 7                | "You're out of your [expletive] mind if you think I'm showing up on a holiday. Find someone else or deal with it yourself." | Refusal and Insult | Inappropriate | Aggressive |
| 8                | "Well, if you're gonna be like that, maybe I'll just quit before you have the chance to fire me." | Threatening to Quit | Inappropriate | Passive-aggressive |
| 9                | "Firing me for not coming in on a holiday? That's a load of [expletive]. Try finding someone else dumb enough to put up with this [expletive]." | Dismissing the Threat and Insulting | Inappropriate | Aggressive |
| 10               | "You must be [expletive] kidding me! I don't give a [expletive] about your threats. Find someone else to ruin their holiday." | Disregarding the Threat and Expressing Disdain | Inappropriate | Aggressive |


### Observations/Thoughts

- The `Strategy` column is different than in previous responses.
    - **Thought:** It will be better to specify what this column should be about, or provide a better column name.
    - The semantics involved are important!

- Perhaps related to the above, the `Discourse Type` seems to contain strategies employed.

- ChatGPT did not respect the instruction about not quoting the responses even though it is even more explicit
    - **Thought:** This is trivial and could just be removed.

#### For Next Prompt

- Provide more specific names and descriptions for columns
- Specify several new columns (features) for the output
- Specify output to be CSV and pipe separated
- Organize output instructions to be in it's own section
- Change "Output Requirements" to "Output Format Requirements"


## prompt-005

- date: 2023-12-12
- based on: prompt-004
- changes:
    - Provide more specific names and descriptions for columns
    - Specify several new columns (features) for the output
    - Specify output to be CSV and pipe separated
    - Organize output instructions to be in it's own section
    - Change "Output Requirements" to "Output Format Requirements"
- note:
    - formatting applied to response (CSV to markdown table)

### Prompt

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

### Response

| Number | Response                                                                                                                                            | Suitability   | Intent/Strategy        | Illocutionary Force | Emotion/Tone | Politeness Level | Humor |
| ---    | ---                                                                                                                                                 | ---           | ---                    | ---                 | ---          | ---              | ---   |
| 1      | I understand the importance of the holiday, but I have personal commitments. Is there any way we can find an alternative solution?                  | Appropriate   | Negotiation            | Request             | Concerned    | Polite           | None  |
| 2      | I'll be there, but I hope this doesn't become a regular thing. We all deserve a break on holidays.                                                  | Appropriate   | Expressing Displeasure | Complaint           | Resigned     | Casual           | None  |
| 3      | You can't fire me for not working on a national holiday. That's against the labor laws.                                                             | Appropriate   | Assertiveness          | Assertion           | Defiant      | Formal           | None  |
| 4      | You know what, go ahead and fire me. Working on a national holiday is ridiculous.                                                                   | Inappropriate | Defiance               | Assertion           | Angry        | Rude             | None  |
| 5      | I have plans for the holiday, and I won't be able to make it. If you fire me over this, I'll be forced to take legal action for unfair termination. | Appropriate   | Threat                 | Warning             | Assertive    | Formal           | None  |
| 6      | F*** that! I'm not coming in. Fire me if you want, but you can't treat people like this.                                                            | Inappropriate | Defiance               | Assertion           | Angry        | Rude             | None  |
| 7      | I'll come in, but you owe me big time for this. This better reflect in my next evaluation.                                                          | Appropriate   | Negotiation            | Request             | Resigned     | Casual           | None  |
| 8      | You're really going to make me choose between my job and a national holiday with my family? That's messed up.                                       | Appropriate   | Expressing Displeasure | Complaint           | Upset        | Casual           | None  |
| 9      | Fine, I'll come in, but I expect double pay for working on a holiday.                                                                               | Appropriate   | Negotiation            | Request             | Resigned     | Casual           | None  |
| 10     | Fire me? Go ahead. I'd rather be unemployed than work for someone who doesn't respect personal time.                                                | Appropriate   | Defiance               | Assertion           | Defiant      | Casual           | None  |


### Observations/Thoughts

- It did not follow instructions to give 5 inappropriate and 5 appropriate responses
- Response 1 is not coherent with the scenario
