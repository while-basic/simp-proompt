---
sidebar_position: 20
---

# 🟢 Prompt Engineering

:::takeaways
- What is prompt engineering?
:::

## What Happens When a Prompt Doesn't Work?

At times, Generative AIs may provide inaccurate responses to prompts. For instance, they may struggle with tasks like multiplying numbers, often delivering incorrect answers with confidence. Give the provided prompt to ChatGPT to observe this phenomenon.

<AIInput>
What is 923 * 99?
</AIInput>

<AIOutput>
The result of multiplying 923 by 99 is 91,377.
</AIOutput>

ChatGPT gave an incorrect answer (the correct answer is 91,377). We can modify our prompt, and prompt ChatGPT to work the problem out step by step.

<AIInput>
What is 923 * 99? Let's go step by step. Always write out the full number of 0s for each term.
</AIInput>

<AIOutput>
Sure, let's break it down step by step:

1. Multiply 923 by 9:
   923 * 9 = 8307

2. Multiply 923 by 90:
   923 * 90 = 83070

3. Add the results from steps 1 and 2:
   8307 + 83070 = 91377

So, the product of 923 and 99 is 91,377.
</AIOutput>

Interestingly, with these extra instructions, ChatGPT successfully tackled the problem. This success stemmed from ChatGPT's meticulous documentation of its steps, ensuring error-free calculations. The mathematical capabilities of Generative AI can be enhanced through prompt engineering. Now, let's explore a different example.

:::caution
Since ChatGPT is <a href="https://learnprompting.org/docs/basics/configuration_hyperparameters">non-deterministic</a>, even this prompt sometimes won't work. You may see answers like 91,177 or 91,077.
:::

### ArchaeologistAI Example

Introducing ArchaeologistAI – your gateway to captivating tales of renowned archaeologists! Unearth the secrets of ancient civilizations and embark on thrilling adventures through history. Discover the past like never before with ArchaeologistAI! #AI #Archaeology #History

<AIInput>
Write a tweet about ArchaeologistAI
</AIInput>

<AIOutput>
Unveil the mysteries of the past with ArchaeologistAI! Delve into captivating narratives of legendary archaeologists and uncover the hidden gems of history. Embark on an epic journey through time like never before. #ArchaeologistAI #HistoryUnearthed 🏺🔍🌍
</AIOutput>

This tweet is inaccurate as ArchaeologistAI solely narrates stories and doesn't engage in new discoveries. However, this discrepancy isn't ChatGPT's responsibility, as it lacked information about ArchaeologistAI. Let's include pertinent details in the prompt.

<AIInput>
Write a tweet about ArchaeologistAI: ArchaeologistAI tells stories about famous archaeologists.
</AIInput>

<AIOutput>
Unveil the captivating tales of renowned archaeologists with ArchaeologistAI! Dive into the rich narratives of history's most fascinating excavators and uncover their remarkable journeys. Explore the past like never before with ArchaeologistAI! #ArchaeologistAI #HistoryUntold 🏺📜🔍
</AIOutput>

This is much better! Now let's try to make ChatGPT write the Tweet in the style of Elon Musk.

<AIInput>
Write a tweet about ArchaeologistAI, in the style of Elon Musk: ArchaeologistAI tells stories about famous archaeologists.
</AIInput>

<AIOutput>
Unearth the riveting chronicles of legendary archaeologists with ArchaeologistAI! Delve into the depths of history's greatest expeditions and unlock the mysteries of ancient civilizations. Embark on an archaeological adventure like never before. #ArchaeologistAI #HistoryReimagined 🏺🌍🔍</AIOutput>

By testing multiple prompts, we can see which one gives the best output. 

## Conclusion

The iterative process of improving our prompts is referred to as prompt engineering. Perfecting a prompt rarely happens on the initial attempt, highlighting the importance of honing our prompt refinement skills. Proficiency in prompt engineering primarily develops through extensive practice, involving trial and error. Subsequent articles in this section will introduce various prompting strategies to aid in your prompt engineering journey.
