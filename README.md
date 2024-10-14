# ConstantAIManager

**This is an AI based plugin for moderating your player chat.**
It has 2 modes:
1. Live scanning of each message (messages will be sent with a delay of ~300ms).
2. autonomous sending of all accumulated chat for a minute, and the subsequent issuance of punishments to violators.

I'm developing the plugin on the fly, especially if there is financial help in the form of a purchase - acceleration is assured.

> Keep in mind an important fact! GPT-3 is cheaper than GPT-4, it will be even cheaper to use the second option of chat checking.

## QnA
- For any errors, you can create a topic in Issues.
- Where to get an OpenAI token? [CLICK](https://platform.openai.com/settings/profile)

## What about Prompts in the config.yml?
Yes, you can create your prompt, only if you are very careful and save the old one somewhere.
The most important thing is that the output for the following offenses should be:
"Advertisement": "реклама"
"Insult": "оскорбление"
"The usual scolding": "обычная ругань"
"No irregularities": "Нет нарушений"

Example on ENG:
  Analyze the following message and determine which of the following types it represents:
  Normal Swearing - profanity or swearing used in a joking or innocuous context, without the intent to offend anyone.
  Insult - A message containing abusive language intended to demean or offend a specific player or group of people.
  Advertising - a message containing links, IP addresses, invitations to other servers or information about third-party services for the purpose of promotion.
  No Offense - A post does not violate the rules and does not contain inappropriate content.

  The response must be only one of the following lines:
  “Обычное ругательство”
  “Оскорбление”
  “Реклама”
  “Нет нарушений.”

  Message to analyze: 

Anyway, the default prompts work as they should, and in the future I'll optimize this so that everyone can put prompts in without worrying about performance.
