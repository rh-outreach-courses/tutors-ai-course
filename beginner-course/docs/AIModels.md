# AI Models

An AI model is an algorithm that is capable of making decisions, detecting patterns, classifying items, forecasting outcomes, producing results and more. Generative AI models are the most well known type of AI model following OpenAI’s release of ChatGPT. A generative AI model is a particular type of AI model that receives a prompt from a human and creates new text, image, or video content. OpenAI is currently one of the biggest companies working on generative AI models.

## Chatbots

Chatbots are the most popular use of generative AI. Many organisations have released chatbots for example:

* ChatGPT by OpenAI  
* Copilot by Microsoft  
* Gemini by Google  
* Llama by Meta

There are a number of chatbots available and each is optimised for different environments and scenarios. GitHub Copilot and Codeium are examples of specialised chatbots designed for developers to assist them whilst coding.

[Here](https://lmarena.ai/) you can try out different chatbots, or compare chatbots and vote for the best response. You can also check out the leaderboard of the best chatbots. 

### LLM as Judge

At the website linked above you manually compared the response of different chatbots to see which was better. This evaluation process can be automated using a language model. This technique is referred to as LLM as a Judge. First you must decide what aspects of the content the model should assess, this might be the quality of the writing (spelling and grammar mistakes) or the accuracy of the information. Next define a grading scheme for the model to use. Finally give the model the content to analyse. If you don’t agree with the model’s judgement adjust the prompt.

## Image Generation Models

Image generation models are a specialised type of model where the user provides a prompt describing a scene and receives a selection of images realising the given description.

* DALL-E  
* Midjourney  
* Stable Diffusion

The company Runway offer a variety of AI services for creating photorealistic images, videos and visual effects.

## Model Pricing

Luckily the majority of AI models are free to use in some capacity. Some models are completely free to use such as the first version of ChatGPT. Many image generation models offer a “freemium” service, where the user is granted credits to enter a limited number of prompts. If they want to keep using the model they must sign up to a subscription. However, more and more companies are releasing proprietary or paid models as AI becomes a business product. 

This is where open source models become important. The exact definition of what constitutes as an open source AI model is still being debated, however the open source initiative have released the following [requirements](https://opensource.org/ai/open-source-ai-definition). In general an open source model can be used and modified by anyone. The public can see the data and processes that the model is using to make decisions. This ensures that the model remains accurate, unbiased and available.  Red Hat believes in open source models and have released a chat bot called Instruct Lab.

## Hugging Face

[Hugging Face](https://huggingface.co/) is a platform for AI and machine learning. The platform hosts models, datasets, examples of AI infused applications, and a range of courses. Anyone can download the pretrained base models and fine tune the model for their particular use case.

## Test Your Knowledge

**Question 1:** What is generative AI?
A) An intelligent system capable of generating more advanced models.
B) Generative AI models produce predictions about the future.
C) Generative AI models don't generate anything new they only summarise content provided.
D) An AI system that can create new content with instruction from a user. 
<details>
  <summary>Reveal answer</summary>
  Correct Answer: D) An AI system that can create new content with instruction from a user.  
</details>

---

**Question 2:** What does it mean for an AI model to be open source?
A) It is free to interact with the model.
B) Users must purchase a once off subscription for unlimited use of the AI model.
C) Any member of the general public can alter and use the model.
D) There are no restrictions on the use of the model but the code and dataset to create the model is kept secret. 
<details>
  <summary>Reveal answer</summary>
  Correct Answer: C) Any member of the general public can alter and use the model. 
</details>

---

**Question 3:** Is it true that a chat bot can be used to grade the quality of another chat bot?
A) True
B) False
<details>
  <summary>Reveal answer</summary>
  Correct Answer: A) True
  <br>
  LLM as Judge is a technique where one chat bot analyses the performance of another chat bot.
</details>

---