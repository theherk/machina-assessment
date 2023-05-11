# OpenAI ChatGPT

## Description 🌐

Have you been living under a rock? If so, [ChatGPT](https://chat.openai.com/) is a chat tool developed by OpenAI that makes use of GPT-3.5 and GPT-4 LLM's. These models have captivated many, and the chat tools is "the fastest growing consumer application to date." [^1]

> ChatGPT is fine-tuned from GPT-3.5, a language model trained to produce text. ChatGPT was optimized for dialogue by using Reinforcement Learning with Human Feedback (RLHF) – a method that uses human demonstrations and preference comparisons to guide the model toward desired behavior.
>
> -- https://help.openai.com/en/articles/6783457-what-is-chatgpt

## Usage 🛠️

Basically, given a "System Message" (context about who the bot should act as) and a prompt, a conversation is initiated. That's basically it. The tool can seemingly reason with you, is open to correction if called out on mistakes, can remember what it told you in the past, write code for you, takeover powergrids ensuring mass chaos around the world (ok, I hope not), debug code with stack traces, find bugs in snippets, etc. The thing is, nobody knows what all it can do, or on a deep level, how these LLM's work.

One way aside from the chat interface to interact with GPT, and the other language models and API's provided by OpenAI, is to use the [Playground](https://platform.openai.com/playground). Here you can select the model, tuning, and set the system message explicitly.

You can of course make this as obtuse as you see fit:

Given the system message:

> You are a 1337 h4x0r with a minor in Memeology, and you like to name your variables using emojis.

And the prompt:

> Write me some python to scrape content from wikileaks.

Here is the primary snippet returned:

```python
import requests
from bs4 import BeautifulSoup

# Define the URL of wikileaks
🌐 = "https://wikileaks.org"

# Get the content from the URL
🔍 = requests.get(🌐)

# Check if the request was successful
if 🔍.status_code == 200:
    # Parse the content using BeautifulSoup
    🍜 = BeautifulSoup(🔍.content, "html.parser")

    # Find all links in the content
    🖇️ = 🍜.find_all("a")

    # Print the text and the link
    for 🔗 in 🖇️:
        print(🔗.text, 🔗["href"])

else:
    print("Failed to fetch the content.")
```

Code review rejected. 🙅

> Step into my office, cuz your fucking fired!
>
> -- There's Something About Mary

## Benefits 🌟

The benefits are beyond measure or comprehension. This is an extremely large model that can pass law exams [^2], has potential in healthcare diagnosis [^3], and apparently has better bedside manner than many doctors [^4].

You can absolutely ask it to:

> Create a terraform module that creates two S3 buckets with bidirectional regional replication and global access enabled, that yields the bucket arn's and the replication rules as outputs.

> Write a micronaut application that serves the following OpenAPI document...

## Risks 😨

Well, although the risk are substantial with AI in general, chat interfaces actually have a diminished risk when compared to code completion. The ergonomics aren't as nice, but it is crystal clear what data is going to the mothership. So there really isn't much of a data leakage risk. However, you still risk the general biases and discrimination that come with AI.

### Legal Implications ⚖️

> Can you delete specific prompts?
>
> No, we are not able to delete specific prompts from your history. Please don't share any sensitive information in your conversations.
>
> -- https://help.openai.com/en/articles/6783457-what-is-chatgpt

But also:

> Subject to the Content Policy and Terms, you own the output you create with ChatGPT, including the right to reprint, sell, and merchandise – regardless of whether output was generated through a free or paid plan.

So essentially, you own what it gives you back, but it uses what you send to it for both generation and improvement.

Read more in their [Content Policy](https://labs.openai.com/policies/content-policy) and [Terms of use](https://openai.com/policies/terms-of-use).

[^1]: [ChatGPT reaches 100 million users two months after launch - The Guardian](https://www.theguardian.com/technology/2023/feb/02/chatgpt-100-million-users-open-ai-fastest-growing-app)
[^2]: [ChatGPT passes exams from law and business schools - CNN Business](https://edition.cnn.com/2023/01/26/tech/chatgpt-passes-exams/index.html)
[^3]: [ChatGPT for healthcare services: An emerging stage for an innovative perspective - ScienceDirect](https://www.sciencedirect.com/science/article/pii/S2772485923000224)
[^4]: [AI has better ‘bedside manner’ than some doctors, study finds - The Guardian](https://www.theguardian.com/technology/2023/apr/28/ai-has-better-bedside-manner-than-some-doctors-study-finds)
