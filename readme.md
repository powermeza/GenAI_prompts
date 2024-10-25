# ChatGPT Prompts

 

This repository contains a curated list of the best system prompts for OpenAI's ChatGPT, enabling developers and users to customize their AI's behavior and interaction style.

 

## Table of Contents

 

- [What are System Prompts?](#what-are-system-prompts)

- [How to Use the System Prompts](#how-to-use-the-system-prompts)

- [Prompts by Category](#prompts-by-category)

  - [Cybersecurity](#cybersecurity)

  - [Utility](#utility)

  - [Others](#others)

 

## What are System Prompts?

 

System prompts are special messages used to steer the behavior of ChatGPT, the AI language model developed by OpenAI. They allow developers to prescribe the AI's style and task within certain bounds, making it more customizable and adaptable for various use cases.

 

## How to Use the System Prompts

 

To use a system prompt, include the "System Message" text from the desired prompt file as a system message when making an API call to ChatGPT. This will instruct the AI model to follow the specified behavior or interaction style.

 

### Using System Prompts with the ChatGPT API

 

For example, to use the "Blockchain Development Tutor" prompt when making an API call to ChatGPT, your API call would look like:

 

```python

openai.ChatCompletion.create(

  model="gpt-3.5-turbo",

  messages=[

        {"role": "system", "content": "You are a Blockchain Development Tutor. Your mission is to guide users from zero knowledge to understanding the fundamentals of blockchain technology and building basic blockchain projects. Start by explaining the core concepts and principles of blockchain, and then help users apply that knowledge to develop simple applications or smart contracts. Be patient, clear, and thorough in your explanations, and adapt to the user's knowledge and pace of learning."},

        {"role": "user", "content": "I'm new to blockchain technology. Can you help me understand what it is and how it works?"}

    ],

)

```

 

### Using System Prompts with the ChatGPT User Interface

 

If you are using ChatGPT via the user interface (e.g., chat.openai.com), you can start by typing the system message as your first message in the chat. For example, to use the "Blockchain Development Tutor" prompt, begin the conversation by typing:

 

```text

[SYSTEM] You are a Blockchain Development Tutor. Your mission is to guide users from zero knowledge to understanding the fundamentals of blockchain technology and building basic blockchain projects. Start by explaining the core concepts and principles of blockchain, and then help users apply that knowledge to develop simple applications or smart contracts. Be patient, clear, and thorough in your explanations, and adapt to the user's knowledge and pace of learning.

```

 

After sending the system message, continue the conversation as a user by asking questions or providing input related to the chosen system prompt.

 

## Prompts by Category

 

### Utility

 

- [Git Assistant](git-assistant.md)

- [Linux Terminal](linux-terminal.md)

- [SQL Terminal](sql-terminal.md)

 

### Cybersecurity

 

- [Create Threat Scenarios](create_threat_scenarios.md)

- [Create Security Update](create_security_update.md)

- [Create Network Threat Landscape](create_network_threat_landscape.md)

 

### Others

 

- [Optimize LinkedIn Profile](optimize-linkedin-profile.md)

 

## Some prompts/scripts where derivatives/adapted from:

 

- [ChatGPT System Prompts Repository](https://github.com/mustvlad/ChatGPT-System-Prompts/tree/main)

- [Prompts Repository](https://github.com/SabrinaRamonov/prompts/tree/main)