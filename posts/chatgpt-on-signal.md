# What if you had ChatGPT on your phone?

## TL;DR

Simple integration of [ChatGPT](https://openai.com/blog/chatgpt) with [Signal](https://signal.org).
Set it up on your phone by following the instructions on the [project page](https://github.com/nichelia/chatbot)

## About

Have you ever wished you had access to OpenAI's ChatGPT on your phone, but found the process of authenticating, navigating to their website, and writing in a web interface to be inconvenient? As someone who uses ChatGPT daily, I found myself frustrated with the limitations of this amazing technology.

That's why I came up with a solution - integrating ChatGPT with the Signal messaging app. Now you can access the power of ChatGPT through a familiar chat interface, complete with speech-to-text, keyboard shortcuts, and autocomplete functionality.

But why use ChatGPT in the first place? As advancements in natural language processing continue, we're seeing the potential for chatbots and automated conversations to revolutionize the way we interact with technology. ChatGPT, specifically, has been shown to generate human-like responses that can be difficult to distinguish from those written by a person.

However, accessing ChatGPT through the OpenAI website has its limitations. Authenticated users experience frequent timeouts and overwhelmed servers, limiting the usability of the technology. My solution offers a more convenient way to access ChatGPT, albeit at a cost.

In this blog post, I'll delve into the technical details of how I integrated ChatGPT with the Signal messaging app and how you can get started using it yourself. Stay tuned for a closer look at this exciting project!

## What you will need

To get started with integrating ChatGPT with the Signal messaging app, you will need a few things:

1. A standby machine such as a laptop or desktop computer.
2. Docker Desktop installed on your machine.
3. An OpenAI developer account which you can create on their website.
4. The Signal messaging app on your phone with a registered phone number.

If these prerequisites seem daunting, don't worry. We'll walk through each step in more detail to ensure you have everything you need to get started.

## Why Signal

Signal is a free and open source messaging app for iOS, Android, and desktop that provides end-to-end encryption for its users. Simply put, it allows you to have private conversations without the worry of someone snooping on your messages. Some of the features include texting, voice and video calls, media sharing, and group messaging. Not only is Signal privacy-focused, but it is also user-focused with a clean, simple interface that's easy to navigate. How does it differ from its competitors like Facebook Messenger, iMessage, WhatsApp, and Viber? They lack in the element of privacy and security that Signal so highly prioritizes. Signal can be downloaded on the App Store and Play Store for phones and on laptops as well, making it an accessible and widely available messaging app for all.

## What is Docker Desktop

Docker Desktop is a tool that makes it easier to build, test, and run applications by packaging them into self-contained containers. In simpler terms, it allows developers to create a reproducible environment for their projects, ensuring that everything works reliably, regardless of the machine it's running on. In the context of our project, we use Docker Desktop to ensure that our implementation of ChatGPT is consistent across different devices and operating systems, making it easier to get up and running.

---
Cover photo: [Dall-E generated image \`A futuristic cyborg poster hanging in a neon lit subway station\`](https://openai.com/product/dall-e-2)