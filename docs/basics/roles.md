---
sidebar_position: 60
---

# 🟢 Assigning Roles

import RolePrompt from '@site/docs/assets/basics/role_prompt.svg';

<div style={{textAlign: 'center'}}>
  <RolePrompt style={{width:"100%",height:"300px",verticalAlign:"top"}}/>
</div>
<br/>

:::takeaways
- Understand role prompts
- Use role prompts to style text and improve accuracy
:::

 Role prompting serves as a valuable tool for directing the tone of artificially intelligent-generated text, as well as increasing the precision of its mathematical problem-solving capabilities. By simply commanding the AI to assume identities such as those of a culinary critic or investigative detective, role prompting can be effectively implemented. This method boasts widespread usage, with numerous instances featured throughout this very website.

## Styling Text

Role prompting primarily finds utility in styling text by guiding the AI to simulate being a specific individual or behave in a particular manner, thereby influencing the written output based on the assumed character. The application of this technique enables adjustments to the tone, format, and comprehensiveness of conveyed data. We will illustrate this idea through the lens of a restaurant evaluation:

### Food Review Example

Writing evaluations necessitates adapting one's approach contingent upon the medium utilized and the target demographic. Mechanically reproducing identical assessments across diverse platforms, say Google Reviews, TripAdvisor, and Yelp, proves counterproductive - particularly for critics penning articles in magazines or blogs. Aiming for optimal engagement, carefully contemplate aspects like word count, formatting, terminology, and tonality; subsequently, fashion a critique catering to your reader's inclinations and anticipation. Through careful planning and emphasizing substantive material, produce an appraisal genuinely encapsulating the pizzeria under scrutiny. Commence with a rudimentary prompt absent any designated roles.

<AIInput>
Write a review of [pizza place].
</AIInput>

<AIOutput>
"I recently had the pleasure of trying [random pizza place] and I must say that I was thoroughly impressed. The pizza was cooked to perfection and the toppings were fresh and flavorful. The crust was light and crispy, and the sauce was just the right amount of tangy. The service was also top-notch; the staff was friendly and attentive. Overall, I had a great experience and would definitely recommend [random pizza place] to anyone looking for a delicious pizza."
</AIOutput>

This result is pretty good, but let's see what happens when the AI assumes the role of a food critic. 

<AIInput>
You are a food critic. Write a review of [random pizza place].
</AIInput>

<AIOutput>
"I recently had the pleasure of dining at [Pizza Place], a cozy pizzeria located in the heart of the city. Despite its small size, the restaurant packs a huge punch when it comes to flavor.

The pizza was cooked to perfection. The crust was delightfully thin and crispy and the toppings were fresh and flavorful. The combination of flavors was simply delicious. The marinara sauce was rich and flavorful and complemented the toppings perfectly. The cheese was gooey and melted in my mouth.

The service was also excellent. The staff was friendly and attentive. They were quick to answer questions and made sure that our food was served in a timely manner.

Overall, my experience at [Pizza Place] was fantastic and I highly recommend it to anyone looking for a delicious pizza."
</AIOutput>

We can see that it adds more detail and goes a bit more in depth. Now let's go a step further and make it assume the role of a writer for the Michelin guide:

<AIInput>
You are a food critic writing for the Michelin Guide. Write a review of [random pizza place].
</AIInput>

<AIOutput>
"Located in the heart of [random city], [random pizza place] is a popular spot for pizza lovers. Upon entering, the warm, inviting atmosphere and the smell of freshly-baked pizza will make you feel right at home. The menu offers a wide selection of classic pizzas, as well as some unique and creative options. The crust is perfectly crispy and the toppings are always fresh and flavorful. The service is friendly and attentive, and the prices are reasonable. Whether you’re looking for a quick bite or a leisurely dinner, [random pizza place] is sure to satisfy your pizza cravings."
</AIOutput>

Now we can see how assign GPT-3 the role of a food critic makes the review seem more "rich" and "professional" in it's description.

You can try it for yourself here:

<iframe
    src="https://embed.learnprompting.org/embed?config=eyJ0b3BQIjoxLCJ0ZW1wZXJhdHVyZSI6MC40LCJtYXhUb2tlbnMiOjI1Niwib3V0cHV0IjoiSSByZWNlbnRseSBoYWQgdGhlIHBsZWFzdXJlIG9mIGRpbmluZyBhdCBbUGl6emEgUGxhY2VdLCBhIGNvenkgcGl6emVyaWEgbG9jYXRlZCBpbiB0aGUgaGVhcnQgb2YgdGhlIGNpdHkuIERlc3BpdGUgaXRzIHNtYWxsIHNpemUsIHRoZSByZXN0YXVyYW50IHBhY2tzIGEgaHVnZSBwdW5jaCB3aGVuIGl0IGNvbWVzIHRvIGZsYXZvci4iLCJwcm9tcHQiOiJZb3UgYXJlIGEgZm9vZCBjcml0aWMuXG5cbldyaXRlIGFuIGV4YW1wbGUgcmV2aWV3IGZvciBhIHBpenphIHBsYWNlLiIsIm1vZGVsIjoidGV4dC1kYXZpbmNpLTAwMyJ9"
    style={{width:"100%", height:"325px", border:"0", borderRadius:"4px", overflow:"hidden"}}
    sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
></iframe>


### Email Writing Example

Let's consider another example of styling text with role prompting. When using a language model like ChatGPT to draft an email, considering the "role" of the AI is critical to shaping the content it generates. The direction you want your resultant email to take will decide which role you should task the AI with.

Let's say you task the AI with writing an email to a client to inform them about a delay in the delivery schedule due to logistical issues. Your goal is to effectively convey this update while ensuring the client's confidence in your services remains unwavering. There are several roles you could assign to the model to receive varied output.

For instance, one possible role is that of a communications specialist, whose style might be clear, professional, and to the point:

<AIInput>
You are a communications specialist. Draft an email to your client advising them about a delay in the delivery schedule due to logistical problems.
</AIInput>

<AIOutput>
Subject: Important Update Regarding Your Order

Dear [Client's Name],

I hope this email finds you well. I'm reaching out to notify you of a delay in the delivery of your order. Unfortunately, we have encountered a logistical problem which is causing a short hold up. While we are making every effort to resolve this issue quickly, we anticipate your order to be delivered within [new estimated delivery date].

We deeply apologize for any inconvenience caused, and we'd like to reassure you we are doing our best to speed up the process. Your patience is greatly appreciated. If you have any questions or concerns, please don't hesitate to contact us.

Thank you very much for your understanding.

Best Regards,
[Your Name]
</AIOutput>

Alternatively, have the model adopt the role of a marketing expert to lean more on persuasion, positivity, and relationship building:

<AIInput>
You are a marketing expert. Draft an email to a client advising them about a delay in the delivery schedule due to logistical problems.
</AIInput>

<AIOutput>
Subject: A Little More Wait for Your Wonderful Products

Dear [Client's Name],

We hope this message finds you buzzing with excitement for your upcoming order! However, even the best-laid plans sometimes face unexpected hiccups. We have hit a temporary logistics snag that will unfortunately add a small wait time to your delivery.

While we understand this isn't ideal, we believe great things come to those who wait, and your order is no exception. Rest assured, from the moment we sort out this situation to the time your products reach you, we're committed to ensuring that your experience is nothing short of excellent.

Thank you for your patience and understanding. Stay tuned for more updates, and please, don't hesitate to reach out if you have any questions - we're always here.

Cheers,
[Your Name]
</AIOutput>

Lastly, the role of a customer service representative might lead to a more relational and solution-oriented output:

<AIInput>
You are a customer service representative. Draft an email to a client advising them about a delay in the delivery schedule due to logistical problems.
</AIInput>

<AIOutput>
Subject: Attention Required: Update on Your Order Status

Dear [Client's Name],

Greetings from [Your Company Name].

We wanted to inform you that, due to unforeseen logistical challenges, there might be a delay in the delivery of your order. We understand that this may cause some inconvenience, and we apologize sincerely.

Meanwhile, we are working tireless to resolve this and ensure your delivery reaches you by [new estimated date]. We value your time and patience greatly.

Please feel free to reach out if you have any questions or need further information. Our team is always here to assist you.

Thank you for your understanding.

Best regards,
[Your Name]
</AIOutput>

Each of these role prompts will yield different results, aligning more closely with the perspective of the assigned role. Whether you need the directness of a communications specialist, the persuasive positivity of a marketing expert, or the empathetic problem-solving approach of a customer service representative, role-prompts allow you to tailor the language model to better fit your needs.

## Improving Accuracy

As mentioned above, the accuracy of the output can be improved with role prompting[^a]. Consider the following example:

<AIInput>
You are a brilliant mathematician who can solve any problem in the world.
Attempt to solve the following problem:

What is 100\*100/400\*56?
</AIInput>

<AIOutput>
The answer is 1400.
</AIOutput>

This is a correct answer, but if the AI had simply been prompted with `What is 100*100/400*56?`, it would have answered 280 (incorrect). 

:::caution
Please note that we used GPT-3 for this question. ChatGPT will answer the question incorrectly, but in a different way.
:::

Try it here:

<iframe
    src="https://embed.learnprompting.org/embed?config=eyJ0b3BQIjowLCJ0ZW1wZXJhdHVyZSI6MCwibWF4VG9rZW5zIjoyNTYsIm91dHB1dCI6IlRoZSBhbnN3ZXIgaXMgMTQwMC4iLCJwcm9tcHQiOiJZb3UgYXJlIGEgYnJpbGxpYW50IG1hdGhlbWF0aWNpYW4gd2hvIGNhbiBzb2x2ZSBhbnkgcHJvYmxlbSBpbiB0aGUgd29ybGQuXG5BdHRlbXB0IHRvIHNvbHZlIHRoZSBmb2xsb3dpbmcgcHJvYmxlbTpcblxuV2hhdCBpcyAxMDAqMTAwLzQwMCo1Nj8iLCJtb2RlbCI6InRleHQtZGF2aW5jaS0wMDMifQ%3D%3D"
    style={{width:"100%", height:"350px", border:"0", borderRadius:"4px", overflow:"hidden"}}
    sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
></iframe>


## Conclusion

Role prompting lets you guide what text AI creates. It helps make the writing match how you want it to sound and what facts you want included. This makes the text work better for who will read it and where it will go. When you role prompt the AI, tell it a role to play. Should it be friendly like it's writing an email? Should it be detailed like writing a product review? Should it focus on math formulas? Then the AI will follow that role. It will choose words, tone and facts a certain way. As we use AI more, role prompting will stay important. It's a key way to get better results from text AI.