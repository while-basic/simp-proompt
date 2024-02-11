---
sidebar_position: 10
---
# 🟢 Prompting With ChatGPT

import Interface from '@site/docs/assets/basics/chatgpt_interface.webp';

<div style={{textAlign: 'center'}}>
  <img src={Interface} className="img-docs" style={{width: "80%"}}/>
</div>
<br/>

:::takeaways
- Setting up ChatGPT
- Use ChatGPT to summarize text and solve a math problem
:::

In the preceding module, we covered the concept of AI and how humans can direct AIs to carry out tasks. Prompting, a method of instructing an AI to perform a task, was discussed (@shin2020autoprompt). In this module, we will delve into prompting using ChatGPT, a highly renowned Large Language Model (LLM) accessible at [ChatGPT](http://chat.openai.com)[^a]. Developed by OpenAI, ChatGPT is exceptionally user-friendly and completely free to utilize, making it the most accessible Gen AI currently available for experimentation and implementation.

## Set up ChatGPT

To get started with ChatGPT, follow these steps:

- Navigate to [http://chat.openai.com](http://chat.openai.com)
- Create a new account 
- Log in to ChatGPT.

## Test Some Prompts on ChatGPT

Now that we're all set up, let's try some prompts.

#### 1) Color of the sky

We will start with something very simple: can ChatGPT tell us the color of the sky?

<AIInput>
What color is the sky?
</AIInput>

<AIOutput>
The color of the sky is typically blue.
</AIOutput>

Now let's try another example.

#### 2) Summarizing an Article

Say you are reading an article about rain in Texas. You want to quickly get the main ideas of the article, so you show the AI what you are reading, and ask for a summary[^b]:

<AIInput>
Snowfall in the state of Florida, particularly in its central and southern regions, is exceedingly rare. While some trace amounts or flurries have been recorded, especially in the northern areas, major cities such as Miami, Fort Lauderdale, and Palm Beach have very infrequently experienced snow flurries. The National Weather Service notes that no snow flurries have been reported in the Florida Keys and Key West since European colonization over 300 years ago. In the case of Miami, Fort Lauderdale, and Palm Beach, there has been only one documented instance of snow flurries observed in the air in over 200 years, which took place in January 1977. Since then, these cities have not witnessed any further occurrences of snow flurries.
Summarize this paragraph in a single sentence:
</AIInput>

Here is ChatGPT's response. It is a much shorter read!

<AIOutput>
Snowfall in Florida, particularly in its central and southern regions, is extremely rare. Major cities like Miami, Fort Lauderdale, and Palm Beach have experienced minimal snow events, with only one documented instance of snow flurries observed in over 200 years, occurring in January 1977. The Florida Keys and Key West have not recorded any snow flurries since European colonization over 300 years ago.
</AIOutput>

:::caution
You are more than likely to see a different response. This will be the case for most prompts in this course. We will learn why more later in this module.
:::

#### 3) Math Problem Solving

ChatGPT can also solve math problems! Let's give it a prompt with a simple problem.


<AIInput>
If I have 20 kittens, rehome three of them, and sell three more, how many do I have left?
</AIInput>

<AIOutput>
1. Start with 20 kittens.
2. Rehome 3 kittens: 20 - 3 = 17 kittens left.
3. Sell 3 more kittens: 17 - 3 = 14 kittens left.

You have 14 kittens left.
</AIOutput>


## Conclusion

Ensure you're now familiar with the concept of a %%prompt|prompt%% and basic prompting techniques using ChatGPT. Remember, *prompt* can function as both a verb and a noun. You can either *prompt* a model or provide a model with a prompt, with both actions having the same meaning. This process of giving a model a prompt is referred to as prompting. Further insights into prompting will be covered in the upcoming lesson.