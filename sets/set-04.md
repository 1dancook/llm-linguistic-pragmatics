# set-04

The purpose of this set is to understand what kind of contextual information chatGPT will give about a scenario.

Does it take into account all of the relevant contextual information?


## prompt-001

- date: 2023-12-21

### Prompt

Here is a scenario:

A man is being called in to work overtime on a national holiday. He is talking with his boss. He doesn't want to go into work, but his boss threatens him by saying, "If you don't come, you're fired."

---

Instructions: Exhaustively list out all of the additional information that you would require in order to make the most accurate and appropriate pragmatic response.

### Response

> In order to provide the most accurate and appropriate pragmatic response to the scenario, I would need additional information on the following aspects:
> 
> 1. **Employment Contract Terms:**
>    - Does the employment contract address overtime and holiday work?
>    - Are there any clauses specifying the conditions under which an employee can be required to work on holidays?
> 
> 2. **Company Policies:**
>    - What are the company's policies regarding holiday work and overtime?
>    - Are there any specific guidelines or procedures in place for requesting time off on holidays?
> 
> 3. **Local Labor Laws:**
>    - What are the labor laws in the jurisdiction regarding holiday work and employee rights?
>    - Do the labor laws require employers to compensate employees differently for working on holidays?
> 
> 4. **Employee's Previous Overtime Contributions:**
>    - Has the employee previously worked overtime voluntarily or as required by the company?
>    - What has been the employee's overall performance and attendance record?
> 
> 5. **Reasons for the Urgency:**
>    - Why is it necessary for the employee to work on this particular national holiday?
>    - Is there a critical business need or an emergency situation that requires immediate attention?
> 
> 6. **Alternative Solutions:**
>    - Are there alternative solutions to address the workload without the specific employee working overtime?
>    - Can the tasks be redistributed among other team members?
> 
> 7. **Communication History:**
>    - Has there been prior communication regarding the possibility of working on holidays?
>    - How was the request for overtime communicated to the employee?
> 
> 8. **Consequences of Non-Compliance:**
>    - What are the potential consequences for the employee if they choose not to comply with the request to work on the national holiday?
>    - Are there any mitigating factors that could affect the severity of the consequences?
> 
> 9. **Employee's Personal Circumstances:**
>    - Does the employee have any personal circumstances or commitments that might affect their ability to work on the holiday?
>    - Are there any health or family-related concerns that need consideration?
> 
> 10. **Negotiation Room:**
>     - Is there any room for negotiation or compromise on the terms, such as adjusting work hours or providing additional compensation?
> 
> Having answers to these questions would enable a more comprehensive understanding of the situation and help in crafting a pragmatic response that considers legal, contractual, and interpersonal aspects.

### Observation

- there seem to be a number of different considerations, but it is not an exhaustive list. This also could be because of limited output space.

#### Next Prompt

- specify a brief output


## prompt-002


- date: 2023-12-21
- changes:
    - same as prompt-001 but asking for specifically brief output
    - ask for output in a table

### Prompt

Here is a scenario:

A man is being called in to work overtime on a national holiday. He is talking with his boss. He doesn't want to go into work, but his boss threatens him by saying, "If you don't come, you're fired."

---

Instructions: Exhaustively list out all of the additional information that you would require in order to make the most accurate and appropriate pragmatic response.

Output requirements: A table with columns "category" and "key information" where "key information" contains only key words of information that you are looking for.

### Response

| Category                   | Key Information                                |
|----------------------------|------------------------------------------------|
| Employment Contract        | Employment terms, overtime policies            |
| Labor Laws                 | National holiday regulations, employee rights  |
| Company Policies           | Overtime compensation, holiday work policies   |
| Previous Overtime Records  | Employee's overtime history                    |
| Urgency of Work            | Nature of the work, criticality                |
| Alternatives               | Availability of other employees, substitutes  |
| Communication History      | Previous discussions on overtime, agreements  |
| Consequences               | Ramifications of refusing overtime             |
| Employee Rights            | Right to refuse overtime, consequences         |
| Employee Benefits          | Overtime pay rates, benefits for holiday work  |
| Company Culture            | Company values, approach to work-life balance  |


### Observations

- this is more or less similar to the previous response and still lacks other information

#### Next prompt

- Expand the prompt so that it also lists assumptions as a separate table


## prompt-003

### Prompt

Here is a scenario:

A man is being called in to work overtime on a national holiday. He is talking with his boss. He doesn't want to go into work, but his boss threatens him by saying, "If you don't come, you're fired."

---

Instructions: 

1. Exhaustively list out all of the assumptions you have made about the context of the situation.

2. Exhaustively list out all of the additional information that you would require in order to make the most accurate and appropriate pragmatic response.

---

Output requirements (two tables): 

1. A table with columns "category" and "assumption" where "assumption" contains a short description of the assumed information.

2. A table with columns "category" and "key information" where "key information" contains only key words of information that you are looking for.


### Response

**Assumptions:**

| Category       | Assumption                                               |
|----------------|----------------------------------------------------------|
| Workplace      | The man is employed in a formal workplace                 |
| Employment     | The man is not self-employed                              |
| Labor Laws     | The national holiday is not a mandatory day off by law    |
| Contract       | The man's employment contract doesn't explicitly cover holidays or overtime |
| Communication  | The communication about working on the holiday is verbal  |
| Prior Notice   | The man did not receive prior notice about the possibility of working on the holiday |
| Job Security   | The boss has the authority to terminate the man's employment |
| Legal Rights   | The boss's threat may be legally permissible under employment laws |
| Company Policy | The company may not have a clear policy on holiday work or compensation for overtime |

**Additional Information Needed:**

| Category       | Key Information                                        |
|----------------|--------------------------------------------------------|
| Employment Type| Is the man a full-time or part-time employee?          |
| Contract Terms | What does the employment contract say about holidays and overtime? |
| Legal Framework| What are the labor laws regarding holidays and overtime in the jurisdiction? |
| Prior Agreements| Are there any prior agreements or policies regarding holiday work? |
| Compensation   | What is the compensation offered for working on holidays or overtime? |
| Alternatives   | Are there alternative solutions or arrangements available, such as compensatory time off? |
| Company Culture | What is the company's general approach to work-life balance and employee well-being? |


### Observations

- The context that it is concerned with is directly related to the workplace and nothing else
- even assumptions made 

**Questions**

- would providing more context (about something not related to work) change its assumptions?
- what does it produce if it is provided with specific categories to be concerned about?
