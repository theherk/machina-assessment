# 🤖 machina-assessment

There are many AI / LLM tools emerging, and the landscape is changing daily. My goal is to assess them for both personal and professional reasons. This is just my tiny perspective into tools I am working with, and some considerations about them.

I vacillate heavily between "Wow! This is amazing!" and "Kill it with fire!". I'm part tech geek, part Luddite on the topic.

In any event, these analyses should be done in the open, and I welcome your contribution or correction to these reports.

## Goals

- 🔍 Identify tools useful for programming.
- 💲 Assess their value.
- 📚 Evaluate how to use them.
- ⚠ Consider the risk associated.

It would be excellent, to have extra data when available or possible with traffic analysis to verify the data being sent out is as expected. But there are only so many hours in the day. 🤷

## Types of AI Covered

Broadly speaking there are two types of AI-related tools considered here:

- Those that make suggestions in your editor.
- Those that you have a dialog with via separate chat.

Some are both, and both are very much like having a pair programmer that is just flat out better than you. And if you are still stuck thinking they aren't capable or hallucinate too much, your information is out-of-date. These new models are better than most of the scrubs I've ever worked with; better than me by an embarrassing amount. You can think you're Kasparov all you want, but when Deep Blue comes you're still a world champ getting lapped by the machine.

> When I was defeated by Deep Blue in 1997, I became convinced that my mistake was not taking machine intelligence seriously enough.
>
> -- Garry Kasparov

There are of course other types of tools, and tools useful in other applications; e.g. healthcare. Some tools provide very nice API's too, but we aren't going to touch any of that here; just the pair programming tools.

## Tools Covered

- [Bard](./bard.md)
- [ChatGPT](./chatgpt.md)
- [Codeium](./codeium.md)
- [CodeWhisperer](./codewhisperer.md)
- [Copilot](./copilot.md)
- [Raycast](./raycast.md)

## Risks 😨

Since Codeium is both an autocomplete tool and a chat interface there are more varied risks. But is offers a fully self-hosted model, so those can be mitigated entirely if needed.

### Data Leakage 📤

Each of the suggestion tools comes with some degree of risk, as they must send code to the API to retrieve a suggestion, but they have varying degrees of openness about how they select data for harvesting, so we'll take this one in each report.

### Legal Implications ⚖️

The legal implications are also very specific to the tool, so we'll rely on specific takes in each report. But in general, one must consider what code is going upstream, client data, and corporate espionage.

### Licensure 📃

The risk of licensure remains relevant. It is essential to ensure that any generated code is free from copyrights or licensing encumbrances. Basically, the jury is out on how code suggestions claimed by other parties will impact licensure, but I find most of these concerns to be completely dubious. I haven't seen any well-articulated risks that suggestions will cause license encumbrances.

### Ethical Issues 🤔

- Bias in the training data or algorithms that could lead to unfair or discriminatory outcomes.
- Lack of transparency in how the AI makes its suggestions, making it difficult for developers to understand or verify the code.
- Dependence on the AI code assistant, which could lead to a reduction in critical thinking or creativity skills among developers.
- Intellectual property concerns if the AI code assistant is used to generate code that infringes on existing patents or copyrights.
- Potential for misuse or abuse if the AI code assistant is used for malicious purposes, such as creating malware or hacking tools.

I highly recommend [Why Does AI Lie, and What Can We Do About It?](https://youtu.be/w65p_IIp6JY) or any videos from Computerphile on the topic, like [AI "Stop Button" Problem - Computerphile](https://youtu.be/3TYT1QfdfsM), or scholarly papers on the topic.

## General Disposition

The risks of using autocomplete AI models is very unclear. With chat interfaces, it is very easy to know what data goes out, because you put it in the box. But with autocomplete models, you have to either self-host where possible or accept that some portion of your code will be sent to the mothership with varying degrees of knowledge about what is sent.

> You haven't proved it's safe. You've just proved you can't figure out how it's dangerous.
>
> -- Rob Miles

But all of this brought me to one conclusion. If you think your code is sacrosanct, you are a dinosaur. This is **not** an "all hail deus ex machina" or even "hail corporate", it is just the unfortunate truth that can only be entertaining in the most dire, macabre way. I don't want to be glib, but your source code almost certainly doesn't matter. Why is somebody going to care to steal your codebase, if they can just generate one into existance? They won't. So you can either saddle this horse up and take a ride on Dot Com Boom 2: Electric Boogaloo, or... well it's Chicxulub for you.

Remember, your user data is precious, and should be protected. This is for both moral and compliance reasons, but your program code is functionally moist garbage that can be replaced by old world monkeys beating discipline into a keyboard.

> The development of full artificial intelligence could spell the end of the human race.
>
> -- Stephen Hawking

But chin up buttercup, we aren't there... yet.

---

Look the ethics implications are real. You'd better believe you can get these models to write a function `estimate_iq(gender, skin_color)`, and have it recommend code that actually decrements IQ for women and minorities, while giving me a nice, albeit undeserved, raise. I've seen it. And you must also be aware that **you are unaware of your biases**. So, you have to be conscientious of this and mitigate the risk. You need to review everything with your rose-tinted goggles set aside. This is going to hurt people, but if done with our eyes open maybe this won't cause the fall of mankind within the decade.

> I made a lot of money. I’m not proud of that, but I’m not ashamed of it either.
>
> -- Michael Corleone “The Godfather: Part II” (1974)

> *Note* I must strongly resist the urge to use the spelling "proompt" throughout.
