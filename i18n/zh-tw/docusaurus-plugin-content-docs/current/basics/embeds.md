---
sidebar_position: 40
---

# 🟢 學習提示嵌入

:::takeaways 本文要點

- 配置學習提示嵌入（Learn Prompting Embed）
- 在課程網站上執行 ChatGPT 的提示

:::

ChatGPT 網站非常有用，但如果你能在本網站上直接編寫和測試提示，那不是更好嗎？透過[學習提示嵌入](https://embed.learnprompting.org/)（Learn Prompting Embeds），你可以實現這一點！繼續閱讀以瞭解如何設定。我們將在大多數文章中包含這些互動式嵌入。

## 準備工作

觀看影片教程:

<iframe width="560" height="315" src="https://www.youtube.com/embed/sNUKiwd2DWU" title="YouTube video player" frameBorder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowFullScreen></iframe>

下列是 embed 跑起來的範例圖像:

import lp_embed from '@site/docs/assets/basics/lp_embed.webp';
import key from '@site/docs/assets/basics/API_key.webp';

<img src={lp_embed} class="img-docs" style={{width: "100%"}}/>

您應該可以看到一個與本段正下方的圖像類似的嵌入內容。如果它不可見，您可能需要啟用 JavaScript 或使用其他瀏覽器。如果您仍然看不到它，請加入 [Discord](https://discord.com/invite/learn-prompting) 並告訴我們您的問題。

<iframe
    src="https://embed.learnprompting.org/embed?config=eyJ0b3BQIjowLCJ0ZW1wZXJhdHVyZSI6MCwibWF4VG9rZW5zIjoyNTYsIm91dHB1dCI6IkNob2NvbGF0ZSwgVmFuaWxsYSwgU3RyYXdiZXJyeSwgTWludCBDaGlwLCBSb2NreSBSb2FkLCBDb29raWUgRG91Z2gsIEJ1dHRlciBQZWNhbiwgTmVhcG9saXRhbiwgQ29mZmVlLCBDb2NvbnV0IiwicHJvbXB0IjoiR2VuZXJhdGUgYSBjb21tYSBzZXBhcmF0ZWQgbGlzdCBvZiAxMCBpY2UgY3JlYW0gZmxhdm9yczoiLCJtb2RlbCI6ImdwdC0zLjUtdHVyYm8ifQ%3D%3D"
    style={{width:"100%", height:"320px", border:"0", borderRadius:"4px", overflow:"hidden"}}
    sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
></iframe>

假設您可以看到嵌入內容，請按一下 **Generate** 按鈕。如果這是您第一次使用它，系統將提示您輸入 OpenAI API 金鑰。 OpenAI API 金鑰只是嵌入程式用來連結到您的 OpenAI 帳戶的一串文字。

### 取得一個 OpenAI API Key

- 首先，導覽至 [https://platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys)
- 然後，註冊或登入您的 OpenAI 帳戶。
- 點擊 **Create new secret key** 按鈕。它將彈出一個包含如下視窗：

<div style={{textAlign: 'center'}}>
  <LazyLoadImage src={key} class="img-docs" style={{width: "80%"}} />
</div>

- 將此金鑰複製並貼上到彈出視窗中，然後點擊 **Submit**。

現在您應該能夠在整個網站中使用提示嵌入內容。請注意，OpenAI 會針對您透過這些嵌入提交的每個提示收取費用。如果您最近建立了一個新帳戶，您應該有 3 個月的免費積分。如果您的積分用完了，請不要擔心，因為使用這些型號非常便宜。每產生 7000 個單詞，ChatGPT 只需花費約 0.02 美元[^a]。

### 使用提示 Embed

讓我們學習如何使用提示嵌入。編輯 "Type your prompt here" 欄位。此提示嵌入實際上與使用 ChatGPT 相同，只是您無法進行完整的對話。在本課程中，提示嵌入僅用於展示即時提示工程的範例。

<iframe
    src="https://embed.learnprompting.org/embed?config=eyJ0b3BQIjowLCJ0ZW1wZXJhdHVyZSI6MCwibWF4VG9rZW5zIjoyNTYsIm91dHB1dCI6Ik91dHB1dCBhcHBlYXJzIGhlcmUiLCJwcm9tcHQiOiJUeXBlIHlvdXIgcHJvbXB0IGhlcmUiLCJtb2RlbCI6ImdwdC0zLjUtdHVyYm8ifQ%3D%3D"
    style={{width:"100%", height:"300px", border:"0", borderRadius:"4px", overflow:"hidden"}}
    sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
></iframe>

您可以在 Generate 按鈕下看到四個資訊。左邊的「gpt-3.5-turbo」是模型（gpt-3.5-turbo 是 ChatGPT 的技術名稱）。這三個數字是[LLM設定](https://learnprompting.org/docs/basics/configuration_hyperparameters)，我們將在幾篇文章中了解它們。如果您想製作自己的提示嵌入，請點擊 **edit this embed** 超鏈結。

## 結論

這些提示嵌入將使您在整個課程中更輕鬆地學習，因為您可以快速測試提示，而無需單擊不同的選項卡。但是，如果您喜歡 ChatGPT 介面，則不必使用提示嵌入。只需繼續將提示複製並貼上到 ChatGPT 中即可。如果您確實打算使用提示嵌入內容，請在某處寫下您的 API 金鑰，因為 OpenAI 網站只允許您查看一次。

:::caution
切勿告訴任何人您的 API 金鑰，因為他們可能會使用這個金錀來使用OpenAI而導致您的帳戶費用的提高。
:::

[^a]: 在[這裡](https://openai.com/pricing)查看完整的 OpenAI 定價訊息
