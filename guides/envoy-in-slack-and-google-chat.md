# Envoy in Slack & Google Chat

{% hint style="success" %}
**General Guide** — for everyone, no technical knowledge needed.
{% endhint %}

| | |
|---|---|
| **Who this is for** | Everyone whose company has added Envoy to Slack or Google Chat |
| **Where to find it** | In Slack or Google Chat: mention the bot (usually called **Envoy**) in a channel or space, or send it a direct message |
| **Last checked** | 24 October 2026 |

## What it is

Your company can add Envoy to Slack, to Google Chat, or to both. You ask your question where you already talk to your team, and the answer appears right there in the thread.

In Slack, the bot answers with one agent your admin picked. In Google Chat it answers as Airene, with your company's connectors, unless your admin picked an agent instead.

From Slack and Google Chat, Envoy can only look things up. It never changes data, and it never uses anyone's personal connections, such as their own Gmail.

## Before you start

* Your admin has set up the Slack bot or the Google Chat bot.
* You are a full member of your company's Slack workspace or Google Workspace organization. Guests and people from other organizations don't get answers.
* In Slack, the bot has to be in the channel. Invite it with /invite @bot-name.
* In Google Chat, the app has to be visible to you, and added to the space you want to use.

## How to use it

### Ask in a Slack channel

1. Type @ and the bot's name, then your question, and send it.
2. A short **Thinking…** note appears in that message's thread.
3. The answer is posted in the thread, and the note disappears.

{% hint style="info" %}
For a follow-up, reply in the same thread and mention the bot again. It only sees messages that mention it.
{% endhint %}

### Ask in a Google Chat space

1. If the app isn't in the space yet, click the space name, then **Apps & integrations**, and add it.
2. Type @ and the app's name, then your question, and send it.
3. A **Thinking…** note appears, then the answer arrives in that message's thread.

{% hint style="info" %}
Mention the app without a question and it replies with a short note on how to use it.
{% endhint %}

### Ask in a direct message

1. In Slack, open a direct message with the bot. In Google Chat, start a chat with the app.
2. Type your question. You don't need to mention it here.
3. The answer arrives in the same direct message.

{% hint style="info" %}
A direct message starts a fresh conversation each day, at midnight UTC (07:00 in Jakarta). Give the context again the next day.
{% endhint %}

### Keep a conversation going

1. Stay in one thread. Everything in a thread counts as one conversation, so the bot remembers what was asked earlier in it.
2. Start a new message outside the thread when you want a fresh conversation.

## Your options

| Option | What it does |
|---|---|
| Who answers | Set by your admin. In Slack it is always one chosen agent. In Google Chat it is Airene with your company's connectors, or one chosen agent. |

## Good to know

* It is read-only. If you ask it to change something, it tells you to do it in Envoy instead.
* It doesn't use anyone's personal connections (such as your own Gmail or personal sign-ins). It uses the company connectors of the agent that answers.
* Everyone who can reach the bot gets the same agent and the same knowledge. Don't expect it to know things that are only yours.
* Guests, people from other organizations in shared Slack channels, and anyone in a Google Chat space that is open to outside people get a polite refusal instead of an answer.
* Answers are kept short. A long answer arrives as several messages of up to about 3,900 characters each.
* Only the first 4,000 characters of your message are read.
* Each person can ask about 20 questions every 10 minutes. Past that, or when the bot is very busy, it replies "I'm answering a lot of questions right now. Please try again in a minute."
* It only sees messages that mention it or are sent to it directly. It doesn't read the rest of the channel or thread, and it can't read files you post.
* Conversations are saved in your company's Envoy workspace. They are never added to anyone's personal memory.
* The bot counts toward your company's monthly AI budget. When the budget is used up, it can't answer until the budget resets or an admin raises it ([Company AI controls & Connector access](../for-admins/company-ai-controls-and-connector-access.md)).

## Ideas to try

* In a team channel, ask: "@Envoy what is our refund policy?"
* In a direct message, ask: "Summarise the key points of our travel expense rules."
* In a thread about a customer issue, ask a follow-up: "@Envoy and what if the order is older than 30 days?"

## If something goes wrong

| What you see | What to do |
|---|---|
| Nothing happens after you post in a channel | Make sure you mentioned the bot and that it is in the channel (/invite @bot-name). If it still doesn't answer, your admin may have paused it. |
| "Sorry, I can only help full members of this workspace." | You are a guest or from another organization in Slack. This is on purpose. |
| "Sorry, I can only help people in this organization, in spaces that are not open to people outside it." | Ask in a space that doesn't allow outside people, or in a direct message. |
| "App not responding" in Google Chat, or you can't find the app | Tell your admin. The app's setup or visibility needs checking. |
| "Sorry, I couldn't answer that just now. Please try again in a moment." | Wait a moment and ask again. If it keeps happening, your company's monthly AI budget may be used up; ask your admin ([Company AI controls & Connector access](../for-admins/company-ai-controls-and-connector-access.md)). |
| It doesn't remember yesterday's direct message | That's expected: direct messages start fresh each day. Repeat the context. |

## Related guides

* [Getting started](../guides/getting-started.md)
* [Chatting with Airene](../guides/chatting-with-airene.md)
* [Agents](../guides/agents.md)
* [Connectors (connect your apps)](../guides/connectors.md)
* [Company AI controls & Connector access](../for-admins/company-ai-controls-and-connector-access.md)
