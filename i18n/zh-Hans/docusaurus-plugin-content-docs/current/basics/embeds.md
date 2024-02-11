---
sidebar_position: 3
---

# 🟢 学习提示嵌入

:::takeaways 本文要点

- 配置学习提示嵌入（Learn Prompting Embed）
- 在课程网站上运行 ChatGPT 的提示

:::

The ChatGPT website is useful, but wouldn't it be nice if you could write and test prompts right on this website? With [Learn Prompting Embeds](https://embed.learnprompting.org/), you can! Read on to see how to set this up. We will include these interactive embeds in the most articles.

ChatGPT 网站非常有用，但如果你能在本网站上编写和测试提示，那不是更好吗？通过[学习提示嵌入](https://embed.learnprompting.org/)（Learn Prompting Embeds），你可以实现这一点！继续阅读以了解如何设置。我们将在大多数文章中包含这些交互式嵌入。

## 准备工作

观看视频教程:

<iframe width="560" height="315" src="https://www.youtube.com/embed/sNUKiwd2DWU" title="YouTube video player" frameBorder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowFullScreen></iframe>

Here is an **image** of what an embed looks like:

import lp_embed from '@site/docs/assets/basics/lp_embed.webp';
import key from '@site/docs/assets/basics/API_key.webp';

<img src={lp_embed} class="img-docs" style={{width: "100%"}}/>

You should be able to see an embed that looks just like the image right below this paragraph. If it is not visible, you may need to enable JavaScript or use a different browser. If you still cannot see it, join the [Discord](https://discord.com/invite/learn-prompting) and tell us about your problem.

<iframe
    src="https://embed.learnprompting.org/embed?config=eyJ0b3BQIjowLCJ0ZW1wZXJhdHVyZSI6MCwibWF4VG9rZW5zIjoyNTYsIm91dHB1dCI6IkNob2NvbGF0ZSwgVmFuaWxsYSwgU3RyYXdiZXJyeSwgTWludCBDaGlwLCBSb2NreSBSb2FkLCBDb29raWUgRG91Z2gsIEJ1dHRlciBQZWNhbiwgTmVhcG9saXRhbiwgQ29mZmVlLCBDb2NvbnV0IiwicHJvbXB0IjoiR2VuZXJhdGUgYSBjb21tYSBzZXBhcmF0ZWQgbGlzdCBvZiAxMCBpY2UgY3JlYW0gZmxhdm9yczoiLCJtb2RlbCI6ImdwdC0zLjUtdHVyYm8ifQ%3D%3D"
    style={{width:"100%", height:"320px", border:"0", borderRadius:"4px", overflow:"hidden"}}
    sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
></iframe>

Assuming that you can see the embed, click on the **Generate** button. If this is your first time using it, you will be prompted to input an OpenAI API key. An OpenAI API key is just a string of text that the embed uses to link to your OpenAI account.

### Get an OpenAI API Key

- First, navigate to [https://platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys)
- Then, sign up for or sign into your OpenAI account.
- Click the **Create new secret key** button. It will pop up a modal that contains a string of text like this:

<div style={{textAlign: 'center'}}>
  <LazyLoadImage src={key} class="img-docs" style={{width: "80%"}} />
</div>

- Copy and paste this key into the embed on this website and click **Submit**.

You should now be able to use the embeds throughout this site. Note that OpenAI charges you for each prompt you submit through these embeds. If you have recently created a new account, you should have 3 months of free credits. If you have run out of credits, don't worry, since using these models is very cheap. ChatGPT only costs about $0.02 for every seven thousand words you generate[^a].

### Using the Embed

Discover how to utilize the embed feature by modifying the "Type your prompt here" section. This embed functions similarly to ChatGPT, with the main difference being the inability to engage in extended dialogues. Within this course, embeds serve to illustrate various prompt engineering strategies.

<iframe
    src="https://embed.learnprompting.org/embed?config=eyJ0b3BQIjowLCJ0ZW1wZXJhdHVyZSI6MCwibWF4VG9rZW5zIjoyNTYsIm91dHB1dCI6Ik91dHB1dCBhcHBlYXJzIGhlcmUiLCJwcm9tcHQiOiJUeXBlIHlvdXIgcHJvbXB0IGhlcmUiLCJtb2RlbCI6ImdwdC0zLjUtdHVyYm8ifQ%3D%3D"
    style={{width:"100%", height:"300px", border:"0", borderRadius:"4px", overflow:"hidden"}}
    sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
></iframe>

Beneath the Generate button, you'll notice four details, with the leftmost indicating the model used, 'gpt-3.5-turbo' (which is the formal identifier for ChatGPT). To customize your own embed, select the edit this embed option.


## Conclusion

Utilizing these embeds will facilitate your learning process in the course by allowing for immediate testing of prompts without the need to switch tabs. Nonetheless, if you prefer working directly with the ChatGPT interface, you're free to do so by simply copying and pasting your prompts into ChatGPT. Should you choose to work with embeds, remember to securely note your API key, as OpenAI's site reveals it only once.

:::caution
Never tell anyone your API key, this will charge your account with prompts.
:::

[^a]: See full pricing information [here](https://openai.com/pricing)
