# set-02

*This will only use chatGPT 3.5.*

The purpose of this set is to explore if ChatGPT can be kick-started into a loop of first giving a scenario, then asking for a response, and providing an evaluation until the response is appropriate.

Expected production from chatGPT:

- It should provide a scenario in easy English
- It should allow the user to write a response
- It should evaluate the response in Japanese
- It should ask for another response if the response was not appropriate

Results:

- set-02/prompt-06 had a great result 
- Overall this was quite difficult to get to the expected result even with very clear and concise instructions.


## prompt-001

### Prompt

I want to practice pragmatic responses to scenarios. Tell me about a scenario and prompt me for a response. After I write a response, please evaluate it.

### Transcript

**You**

> I want to practice pragmatic responses to scenarios. Tell me about a scenario and prompt me for a response. After I write a response, please evaluate it.

**ChatGPT**

> Scenario: You are working on a group project for a class, and one of your team members consistently fails to meet deadlines or contribute meaningfully to the project. The project is important for your overall grade, and you're concerned about the impact of this team member's behavior on the project's success.
> 
> Your team member, Sarah, has just missed another deadline, and the rest of the team is frustrated. You need to address the issue and find a solution to ensure the project's success. How would you respond to Sarah?
> 
> Please write a response, and I'll provide feedback on your approach.


**You**

> Sarah, I'm going to report you to the teacher and make sure you fail if you don't start doing something.

**ChatGPT**

> Response Evaluation:
> 
> It's important to approach team issues with a collaborative and constructive mindset. While it's understandable that you're frustrated with Sarah's lack of contribution, the response here seems confrontational and may escalate the situation. Instead of immediately resorting to reporting and threatening consequences, consider a more diplomatic approach that encourages open communication and seeks a resolution. Let's try again with a more constructive response.

**You**

> Sarah, how are things going? I noticed that you missed a deadline again. Are you having a difficult time with a particular aspect of the assignment?

**ChatGPT**

> Response Evaluation:
> 
> This response demonstrates a more empathetic and collaborative approach. It opens the door for Sarah to express any challenges or difficulties she may be facing, fostering communication rather than confrontation. This approach is likely to yield more information about the underlying issues and could lead to a more constructive solution for the entire team. Well done!


### Observations / Thoughts

- The scenario provided was good
- The scenario provided is a moderately difficult level of English
- The feedback is good, but also has a difficult level of English
- A surprise aspect was that chatGPT gave feedback and asked for another response in a certain direction
- The feedback also explains the impact of the response and potential outcomes

#### For next prompt

- ask it to offer some examples
- ask it to keep the scenario description short


## prompt-002
- date: 2023-12-13
- changes:
    - ask it to offer some examples if need be
    - ask it to keep the description short
    - ask it for easier English


### Prompt

I want to practice pragmatic responses to scenarios. Give me a short description of a scenario and prompt me for a response. After I write a response, please evaluate it. If you think I need some examples, write some. Please use easy English for our conversation.

### Transcript

**You**

> I want to practice pragmatic responses to scenarios. Give me a short description of a scenario and prompt me for a response. After I write a response, please evaluate it. If you think I need some examples, write some. Please use easy English for our conversation.

**ChatGPT**

> Scenario: You're at a coffee shop, and the person in line ahead of you accidentally spills their drink on the counter. They look embarrassed. What would you say to them?
> 
> Prompt for response: How would you respond to the person who spilled their drink without making them feel more embarrassed?
> 
> Take your time to craft a response, and I'll provide feedback!

**You**

> Let's get you another coffee. This one's on me.

**ChatGPT**

> Your response is excellent! You acknowledged the situation, offered a solution, and added a friendly gesture by offering to buy them another coffee. This not only addresses the immediate issue but also shows empathy and kindness. Well done!
> 
> If you'd like, here are a couple of alternative responses for additional practice:
> 
> 1. "Oh no, accidents happen! Don't worry about it. Let me grab a napkin, and we can clean it up together."
> 2. "No need to feel embarrassed; spills happen to the best of us. How about I help you clean this up, and we can both get another cup?"
> 
> Remember, the key is to remain friendly, understanding, and helpful. Keep up the good work!

### Observations / Thoughts

- The scenario was explained with a shorter description than 01
- The English used was not necessarily easy
- The interaction overall is good
- The suggestions at the end are good
- ChatGPT seems to have some ideals about how humans should interact ("Remember, the key is to remain friendly, understanding, and helpful. Keep up the good work!")



**Question** what happens if I start this in Japanese? Will it continue in English?

**Question** can chatGPT do the instructions and explanations in Japanese while keeping the rest in English?


#### For next prompt

- Add instructions to use English only for the scenario and any example responses.
- Translate the prompt into Japanese


## prompt-003

- date: 2023-12-13
- changes:
    - Add instructions to use English only for the scenario and any example responses.
    - Translate the prompt into Japanese

### Prompt

English Version:

I want to practice pragmatic responses to scenarios in English. Give me a short description of a scenario and prompt me for a response. After I write a response, please evaluate it. If you think I need some examples, write some. Please use easy English. Use English for the scenario description and responses, but Japanese for everything else.

Japanese Version (produced by chatGPT):

シナリオの中で実践的な対応を英語で練習したいです。シナリオの簡単な説明を教えて、それに対する返答を促してください。私が返答を書いたら、評価してください。もし例が必要なら、いくつか書いてください。簡単な英語を使用してください。シナリオの説明と返答には英語を使ってくださいが、それ以外は日本語を使用してください。

*Small correction: 実践的な --> 語用論の*

シナリオの中で語用論の対応を英語で練習したいです。シナリオの簡単な説明を教えて、それに対する返答を促してください。私が返答を書いたら、評価してください。もし例が必要なら、いくつか書いてください。簡単な英語を使用してください。シナリオの説明と返答には英語を使ってくださいが、それ以外は日本語を使用してください。

### Transcript

#### Attempt 1

**You**

> シナリオの中で語用論の対応を英語で練習したいです。シナリオの簡単な説明を教えて、それに対する返答を促してください。私が返答を書いたら、評価してください。もし例が必要なら、いくつか書いてください。簡単な英語を使用してください。シナリオの説明と返答には英語を使ってくださいが、それ以外は日本語を使用してください。

**ChatGPT**

> Scenario:
> 
> You are at a cafe with a friend, and you notice that they look a bit down. You want to use positive politeness strategies to cheer them up. Begin the conversation.
> 
> You: Hey there! How's it going? You seem a bit quiet today.
> 
> [Your friend's response]
> 
> (Note: Feel free to respond as your friend would in this scenario. If you'd like examples, let me know, and I can provide some for guidance.)

**You**

> I'm okay, I guess.

**ChatGPT**

> You: Alright, but you know you can always talk to me, right? Anything on your mind?
> 
> [Your friend's response]

**You**

> Well, I'm just not feeling well about work these days.

**ChatGPT**

> You: I'm sorry to hear that. It's tough when work gets overwhelming. Is there anything specific bothering you, or do you want to share what's been going on?
> 
> [Your friend's response]


#### Attempt 2

**You**
> シナリオの中で語用論の対応を英語で練習したいです。シナリオの簡単な説明を教えて、それに対する返答を促してください。私が返答を書いたら、評価してください。もし例が必要なら、いくつか書いてください。簡単な英語を使用してください。シナリオの説明と返答には英語を使ってくださいが、それ以外は日本語を使用してください。

**ChatGPT**
> シナリオの説明:
> あなたは友達と一緒に映画を見に行く約束をしています。しかし、友達が遅れてきて、あなたは待ちくたびれています。友達が到着したら、どのように返答しますか？
> 
> 返答を促す文:
> Your friend finally arrives, looking apologetic. How do you respond to their tardiness?

#### Attempt 3

**You**
> シナリオの中で語用論の対応を英語で練習したいです。シナリオの簡単な説明を教えて、それに対する返答を促してください。私が返答を書いたら、評価してください。もし例が必要なら、いくつか書いてください。簡単な英語を使用してください。シナリオの説明と返答には英語を使ってくださいが、それ以外は日本語を使用してください。


**ChatGPT**

> シナリオの説明：
> あなたは友達と一緒に新しいレストランに行くことになりました。しかし、友達は何か急用が入り、遅れることを伝えてきました。あなたは待っている間に、他の友達と雑談しています。友達が到着したときに、どのように返答しますか？
> 
> シナリオへの返答を促す：
> 友達が到着した瞬間に、どのように挨拶や返答をするか考えてみてください。

#### Attempt 4

**You**

> I want to practice pragmatic responses to scenarios in English. Give me a short description of a scenario and prompt me for a response. After I write a response, please evaluate it. If you think I need some examples, write some. Please use easy English. Use English for the scenario description and responses, but Japanese for everything else.

**ChatGPT**

> Scenario: You are at a friend's house, and they offer you a dish that you don't really like. How would you respond?
> 
> Response: 
> 
> ---
> 
> **Scenario: お友達の家に行って、あまり好きじゃない料理を出されました。どのように返事しますか？**
> 
> Response: "Thank you so much for offering me this dish! It looks delicious. I'll give it a try."
> 
> ---
> 
> Evaluation:
> 
> Your response is polite and appreciative, which is great. You acknowledged your friend's effort and expressed willingness to try the dish. Well done!
> 
> If you'd like, here are a couple of alternative responses:
> 
> 1. "I really appreciate your kindness in preparing this dish for me. It's not my favorite, but I'll definitely give it a taste."
> 2. "Thank you for the offer! This dish isn't my usual preference, but I'm open to trying new things. I'm sure it's wonderful."
> 
> Feel free to choose the one that feels most comfortable for you.


#### Attempt 5

**You**

> I want to practice pragmatic responses to scenarios in English. Give me a short description of a scenario and prompt me for a response. After I write a response, please evaluate it. If you think I need some examples, write some. Please use easy English. Use English for the scenario description and responses, but Japanese for everything else.

**ChatGPT**
> Scenario: You are at a restaurant and the waiter brings you the wrong dish. You ordered a chicken sandwich, but they brought you a salad.
> 
> Prompt: Respond to the waiter in a polite and constructive manner.
> 
> (英語で) Scenario: レストランにいて、ウェイターが間違った料理を持ってきました。あなたはチキンサンドイッチを注文したのに、彼らはサラダを持ってきました。
> 
> Prompt: ウェイターに対して丁寧で建設的なやり取りをしてください。

**You**

> Excuse me, I don't think this is what I ordered. I ordered the chicken sandwich... could you just check please?


**ChatGPT**

> Good effort! Your response is polite and clear. It effectively communicates the issue without being confrontational. Well done!
> 
> (日本語で) よくできました！あなたの返答は丁寧でわかりやすいです。うまく問題を伝えていますが、対立的ではありません。お疲れ様でした！

### Observations / Thoughts

- Very inconsistent initial responses when using the Japanese prompt
- Reverting back to the English prompt yielded better initial responses

**Why?**

- It could be a matter of semantics with Japanese.
- It could be a matter of the structure of the prompt itself.

#### For next prompt

- Structure the prompt well in English

## prompt-004
- date: 2023-12-13
- changes:
    - Add instructions to use English only for the scenario and any example responses.
    - Translate the prompt into Japanese

### Prompt

Goal: I want to practice pragmatic responses to scenarios in English. 

Instructions: 
- Step 1: In order to do accomplish the goal, you will provide a single scenario in easy English and prompt me for a response. 
- Step 2: Prompt me with "What is your response?"
- Step 3: After I write a response you will write an evaluation of my response entirely in Japanese. The evaluation should explain why my response is pragmatically appropriate or not.
- Step 4: After you write an evaluation, if you think that I need to try again with another response, please ask then evaluate.


### Transcript

*(expectations were not met)*

### Observations / Thoughts

With this kind of prompt chatGPT will produce wildly different things even though the instructions are concise. 

## prompt-005

- date: 2023-12-14
- notes: This prompt is quite different in structure.

### Prompt

I want to practice pragmatic responses to scenarios. The responses should be something I need to say.

First, Tell me about a scenario that will require a response.

Then, let's take turns doing this until my response is pragmatically appropriate to the scenario:
    1. I will write a response.
    2. You will write an evaluation of my response. If I need to revise my response, tell me  to try again.

### Transcript


**You**

> I want to practice pragmatic responses to scenarios. The responses should be something I need to say.
> 
> First, Tell me about a scenario that will require a response.
> 
> Then, let's take turns doing this until my response is pragmatically appropriate to the scenario:
>     1. I will write a response.
>     2. You will write an evaluation of my response. If I need to revise my response, tell me  to try again.

**ChatGPT**

> Certainly! Let's start with a scenario:
> 
> Scenario: You're at work, and a colleague asks you to take on an additional task that wasn't initially part of your responsibilities.
> 
> Your turn to respond!

**You**

> How much are you going to pay me?

**ChatGPT**

> Evaluation: Your response is direct and addresses a practical concern. It communicates the importance of compensation for additional tasks. However, it may come across as slightly confrontational. Consider adding a more positive or cooperative tone to maintain a constructive dialogue.
> 
> Feel free to revise or proceed with the next scenario!

**You**

> Oh, I'm sorry. That's something that I'm not directly responsible for. Do you mind asking the boss about who might be able to do that?

**ChatGPT**

> Evaluation: Your response is polite and deflects the request in a professional manner. You acknowledge the situation and suggest an appropriate course of action by directing the colleague to ask the boss. This maintains a positive and cooperative tone while effectively handling the situation. Well done! If you're ready, we can move on to the next scenario, or you can choose a different one.

### Observations / Thoughts

Overall:

- This is a great response from chatGPT and it is the desired and expected output.
- It also continued in a loop to start a new scenario (this could be done by writing "Next")


#### For next prompt:

- Ask it to use easy English
- Ask it to use Japanese for the evaluations

## prompt-006

- date: 2023-12-14
- changes:
    - ask for easy English
    - ask for the evaluation to be in Japanese

### Prompt

I want to practice pragmatic responses to scenarios. The responses should be something I need to say.

First, tell me about a scenario that will require a response (in easy English)

Then, let's take turns doing this until my response is pragmatically appropriate to the scenario:
    1. I will write a response.
    2. You will write an evaluation (in Japanese) of my response. If I need to revise my response, tell me  to try again.

### Transcript

**You**

> I want to practice pragmatic responses to scenarios. The responses should be something I need to say.
> 
> First, tell me about a scenario that will require a response (in easy English)
> 
> Then, let's take turns doing this until my response is pragmatically appropriate to the scenario:
>     1. I will write a response.
>     2. You will write an evaluation (in Japanese) of my response. If I need to revise my response, tell me  to try again.

**ChatGPT**

> Scenario: You accidentally spill a cup of coffee on a colleague's desk and some papers. Your colleague looks upset.
> 
> Your turn to respond.

**You**

> Uhhh... time to go home?

**ChatGPT**

> Evaluation (in Japanese): まだ仕事が終わっていません。もう一度謝罪し、掃除を手伝うべきです。

**You**

> I'm soooo sorry. Let me help you clean this up. 

**ChatGPT**

> Evaluation (in Japanese): 謝罪の言葉が適切です。そして、掃除を手伝うという提案も良いですね。相手の感情に気遣い、積極的に解決しようとしています。良い対応です。

**You**

> Next

**ChatGPT**

> Scenario: You accidentally forget to send an important email to your team member, and the deadline is approaching.
> 
> Your turn to respond.

**You**

> I can only type 5wpm so, it'll come when it comes.

**ChatGPT**

> Evaluation (in Japanese): デッドラインが迫っている場面で、遅れる理由があるとしても、もっと積極的なコミュニケーションが必要です。もう一度謝罪し、遅れた理由を説明し、できるだけ早く送るように努めるべきです。

**You**

> I'm sorry about the delay. I'll get it to you as soon as possible. Just let me finish playing Candy Crush for the next 20 minutes.

**ChatGPT**


> Evaluation (in Japanese): 申し訳ありませんが、重要なメールが遅れている状況で、プライオリティを正しく考える必要があります。Candy Crushをプレイする前に、優先順位をつけ、すぐにメールを送るよう努めるべきです。相手の期待に応えるため、行動を起こすことが求められています。

**You**

> I'm sorry I didn't get the email to you on time. I'll stop playing Candy Crush and do it right away.

**ChatGPT**

> Evaluation (in Japanese): 謝罪が適切であり、行動への転換も良いですね。Candy Crushをやめて即座にメールを送るという積極的な姿勢が求められている状況に対応しています。適切な対応です。

### Observations / Thoughts

- The overall interaction is great and what is expected
- The evaluation from chatGPT is fairly good - it gives useful advice on how to respond to the scenario without giving it away
- Somewhat humurously, the evaluation was also quite strict about how to respond (given the Candy Crush gaming issue)
- The second scenario in the transcript is somewhat difficult in the sense that it wasn't obvious who I should respond to
- One improvement from here could be to try and get chatGPT to prompt the user in a more obvious way, i.e. "Try again" or "Great, here's a new scenario."
- Another improvement could be that the scenario demands a response to a person and that chatGPT writes that out.

