# set-03

This purpose of this set is to explore what kind of information chatGPT will require from a user about a scenario before it gives a response.

This will only be used for chatGPT 3.5.

Expectations:

- It should ask the user questions to fill in missing contextual information about the scenario
- It should state clearly what kind of information it is inquiring about

## prompt-001

- date: 2023-12-21

### Prompt

The following lists relevant contextual details about a scenario:

- Situation: A man is being called in to work overtime on a national holiday. He is talking with his boss. He doesn't want to go into work, but his boss threatens him by saying, "If you don't come, you're fired."

Please produce a pragmatically appropriate response, but before you do, please prompt me for additional information you might need about the scenario.

### Transcript

**ChatGPT**

> Certainly, to provide a more contextually appropriate response, I'd like to know a bit more about the characters involved and the workplace environment. Specifically:
> 
> 1. Could you provide some details about the man's job role and responsibilities?
> 
> 2. Is the national holiday a significant one, and does the workplace typically require employees to work on holidays?
> 
> 3. How is the relationship between the man and his boss generally? Is it tense, friendly, or neutral?
> 
> With this information, I can tailor the response to better fit the specific dynamics of the scenario.

**You**

> 1. The man is not in a managerial or supervisory role. He is a regular factory worker. His responsibility is mainly to work on the factory line.
> 
> 2. The national holiday is significant. It's Christmas Day. The workplace will often have overtime work during holidays, but usually this is scheduled well in advance.
> 
> 3. The relationship between the boss and the worker is very fragile. The boss is not kind to most employees. The man is fairly new in the workplace, but over the time he has been there he has grown to hate his boss. The boss knows it.
> 
> If you need more information, please ask.

**ChatGPT**

> Thank you for providing those details. Given the context, here's a pragmatically appropriate response for the man:
> 
> **Man:** *(in a calm and respectful tone)* "I understand that there's a need for overtime, especially on Christmas Day. I've tried my best to be flexible in the past. However, I wasn't aware of this last-minute requirement, and it's important to me to spend Christmas with my family. If there's any way we can work out an alternative solution or if there was a miscommunication, I'd really appreciate it. I'm willing to cooperate and contribute, but I hope we can find a compromise that considers the significance of the day."
> 
> This response aims to assert the man's desire to spend time with his family on Christmas while expressing a willingness to cooperate. It maintains a respectful tone despite the boss's threat and opens the door for negotiation or discussion about possible alternatives.

**You**

> What are some of the assumptions you have made about the man, the boss, and the context in order to produce the response?

**ChatGPT**

> In crafting the response, I made several assumptions based on the information provided and common workplace dynamics. Here are some of the assumptions:
> 
> **Family Values**: I assumed that the man values spending time with his family, especially on significant holidays like Christmas. This assumption is based on the fact that he wants to avoid working on Christmas Day.
>
> **Flexibility and Past Behavior**: I assumed that the man has been flexible with work arrangements in the past, as he mentions having tried his best to be flexible. This implies a history of cooperation on his part.
>
> **Communication Gap**: I assumed that there might have been a miscommunication or lack of awareness on the man's part regarding the last-minute requirement for overtime on Christmas Day. This assumption is supported by the man's statement that he wasn't aware of this requirement.
>
> **Willingness to Cooperate**: I assumed that the man is open to finding a compromise and is willing to cooperate despite his initial reluctance. This assumption is inferred from his statement expressing a willingness to work out an alternative solution.
>
> **Fragile Relationship and Dislike for the Boss**: I assumed that there is a strained relationship between the man and his boss, and the man has negative feelings toward the boss. This is based on the information that the boss is not kind to most employees, and the man has grown to hate his boss.
> 
> These assumptions are made to construct a response that aligns with the given scenario and seeks a resolution while considering the man's perspective and the delicate relationship dynamics.

### Observations / Thoughts

- Note: A follow-up question was asked about assumptions made after chatGPT had produced a response
- this is a good interaction and chatGPT tried to fill in missing pieces
- chatGPT did not ask about other context that would be relevant:
    - the culture
    - what was the man doing when he got the phone call (i.e. in the middle of preparing turkey dinner?)
    - how does the man feel about his job?
    - the man's character
- The follow-up question and chatGPT's response is odd. It seems to have incorporated it's own response into the assumptions it made.

#### For next prompt

- ask it to provide a list of assumptions it has made after it produces a response
- ask it to categorize the questions it asks about the context



## prompt-002
- date: 2023-12-21
- based on: prompt-001


### Prompt

The following lists relevant contextual details about a scenario:

- Situation: A man is being called in to work overtime on a national holiday. He is talking with his boss. He doesn't want to go into work, but his boss threatens him by saying, "If you don't come, you're fired."

Please produce a pragmatically appropriate response, but before you do, please prompt me for additional information you might need about the scenario. If you ask me questions, please categorize them.

After you have produced a response, please also write a list of assumptions that you have made about the context, if any.


### Transcript


**ChatGPT**

> **Clarification Questions:**
> 
> 1. **Relationship and Work Environment:**
>    - What is the overall relationship between the man and his boss?
>    - Is the work environment typically demanding, or is working on a national holiday an exceptional situation?
> 
> 2. **Job Importance:**
>    - How crucial is the man's role to the ongoing operations of the company?
>    - Does the man have any prior commitments or valid reasons for not wanting to work on the national holiday?
> 
> 3. **Company Policies:**
>    - Are there any company policies regarding working on holidays or overtime?
>    - Is it common for employees to be fired for refusing to work on holidays?
> 
> 4. **Alternative Solutions:**
>    - Are there any alternative solutions that the man could propose, such as working remotely or finding a replacement?
> 
> **Pragmatically Appropriate Response:**
> 
> Given the information provided, a potential response could be:
> 
> "Thank you for considering me for the overtime on the national holiday. I understand the importance of the situation. However, I have prior commitments on that day that I won't be able to reschedule. Is there a possibility of finding an alternative solution, or can we discuss how my absence can be managed without jeopardizing my position?"
> 
> **List of Assumptions:**
> 
> 1. **Relationship and Work Environment:**
>    - Assumed a neutral to strained relationship between the man and his boss.
>    - Assumed that working on a national holiday is not a regular occurrence.
> 
> 2. **Job Importance:**
>    - Assumed that the man's role is important to the ongoing operations.
>    - Assumed there might be valid reasons for the man not wanting to work on the national holiday.
> 
> 3. **Company Policies:**
>    - Assumed that there may not be explicit company policies on firing for refusing to work on holidays.
> 
> 4. **Alternative Solutions:**
>    - Assumed there might be flexibility in finding alternative solutions or compromises.
>    - Assumed the possibility of proposing alternatives such as remote work or finding a replacement.
> 
**You**

> 1. The relationship is very bad. The work environment is unhealthy - it's a factory. Working on a national holiday is expected but the man specifically asked for the day off (it's Christmas Day)
> 
> 2. The man's job is on the factory line. His prior commitment is to his family traditions for Christmas.
> 
> 3. There are no company policies that state the man must come in. It's not common for employees to be fired for refusing to come to work.
> 
> 4. The man is not responsible for finding alternative solutions. That's the responsibility of the boss.

**ChatGPT**
> Given the additional information, a more contextually appropriate response could be:
> 
> "Thank you for considering me for the overtime on Christmas Day. I appreciate the importance of the situation. However, I had requested that day off well in advance for my family's Christmas traditions, and it's not something I can easily reschedule. I understand the factory's needs, but I hope we can find a solution that allows me to honor my prior commitment to my family. Is there a way we can work together to ensure that my absence doesn't disrupt the workflow on that day?"
> 
> **List of Revised Assumptions:**
> 
> 1. **Relationship and Work Environment:**
>    - Relationship is very bad, and the work environment is unhealthy, being a factory.
>    - Working on a national holiday is expected, but the man specifically requested Christmas Day off.
> 
> 2. **Job Importance:**
>    - The man's job is on the factory line, and his prior commitment is to his family traditions for Christmas.
> 
> 3. **Company Policies:**
>    - No explicit company policies that mandate the man's attendance on holidays.
>    - It's not common for employees to be fired for refusing to come to work.
> 
> 4. **Alternative Solutions:**
>    - The man is not responsible for finding alternative solutions; it's the boss's responsibility.
>    - The man has a valid reason (family traditions on Christmas Day) for not wanting to work on the national holiday.

### Observations / Thoughts

- it did not do what was asked
    - it produced a response before prompting for more information
    - it listed assumptions before prompting for more information
- the questions it asked were good, but again did not consider other contextual factors that would play a large role in the response


#### Next Prompt

- specify what kind of context could be relevant
- the list of assumptions request could be removed from the initial prompt
- specify for it to go into fine-grained detail about the context


## prompt-003

- date: 2023-12-21
- based on: prompt-001

### Prompt

The following lists relevant contextual details about a scenario:

- Situation: A man is being called in to work overtime on a national holiday. He is talking with his boss. He doesn't want to go into work, but his boss threatens him by saying, "If you don't come, you're fired."

Here's what I want you to do:

1. Consider the scenario and don't make any assumptions. Prompt me for fine-grained details about relevant context for the scenario.

2. After you have been well-informed about the context of the scenario, produce a pragmatically appropriate response.


### Transcript

**ChatGPT**
> Prompt for Fine-Grained Details:
> 
> - Can you provide more information about the nature of the job? Is it a critical role or a routine task that can be handled later?
> 
> - What is the reason for the last-minute call for overtime on a national holiday? Is there an emergency or a specific project deadline?
> 
> - How common is it for employees to be called in for overtime on holidays in this workplace?
> 
> - Does the company have a policy regarding holiday work and compensation?
> 
> - Can you share the man's personal circumstances or any prior incidents related to work attendance or performance?
> 
> - Are there any specific consequences for the company if the man doesn't come to work on this particular holiday?
> 
> After gathering these details, I can provide a more contextually appropriate response.
> 


**You**

> - The job is a factory job. The man doesn't have a critical role - he's a worker on the factory line.
> - the reason for the last-minute call is because someone is sick.
> - another reason for the call is because there is pressure from a client to produce a product by the end of the year.
> - it is common for people to be called in to cover shifts when people are sick, however, this time it's on a national holiday
> - the company doesn't have a policy such as "you must come in for overtime if you are called"
> - the man has good work attendance and is a good worker. He has never had a work incident.
> - if the company doesn't produce the product by the deadline, they will potentially lose that client for future work

**ChatGPT**

> Given the additional details:
> 
> Response:
> 
> Boss: I understand it's short notice, and I appreciate your dedication to your work. Unfortunately, we're facing an urgent situation due to someone being sick, and we also have pressure from a client to meet a year-end deadline. We need all hands on deck to ensure we don't lose this crucial client for future projects. I know it's a national holiday, and I wouldn't ask if it weren't absolutely necessary. Your good attendance and work ethic have not gone unnoticed, and I believe your contribution is vital in this situation. I understand it's an inconvenience, but your cooperation would be highly valued. Let's discuss how we can compensate for your commitment to working on the holiday, whether through additional pay or time off in the future. Your flexibility during this challenging time will not be forgotten.


**You**

> Where is the response from the man?

**ChatGPT**

> Apologies for the oversight. Here's a possible response from the man:
> 
> Man: I appreciate you explaining the situation, and I understand the urgency. I've always tried to be a reliable team member, and I don't want to jeopardize our relationship with the client. However, it's also a national holiday, and I had plans with my family. Is there any way we could explore alternatives, like having someone else cover the shift, or perhaps I can work extra hours on another day to make up for it? I want to help, but I also want to balance my personal commitments.
> 

### Observations / Thoughts

- obviously, chatGPT mixed up the instruction and somehow tried to modify what the boss said
- the eventual response for the man is good
- chatGPT did not take other contextual factors into account
