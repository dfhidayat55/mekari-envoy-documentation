# Company AI controls & Connector access

{% hint style="success" %}
**General Guide** — for everyone, no technical knowledge needed.
{% endhint %}

| | |
|---|---|
| **Who this is for** | Company admins |
| **Where to find it** | **Settings** → **Company AI controls** and **Connector access** (under **AI Command Center**). Who may connect an app is set on that app's page under **Connectors**. |
| **Last checked** | 24 October 2026 |

## What it is

These pages let an admin set limits that apply to everyone in the company.

**Company AI controls** decides whether people may use memory, whether Zero Data Retention is forced on everyone, whether people may turn conversation compaction off, and how long memory chat summaries may be kept. These can only make things stricter than what each person chooses for themselves. The same page holds the **Monthly AI budget**: a cap on how much AI the whole company can use each month.

**Connector access** turns connectors on or off for the whole company. A connector you turn off can't be connected by anyone, and agents stop using it. On each app's own page you can also choose who in the company may connect it.

## Before you start

* You need the admin role in your company. Members and viewers don't see these pages.
* For Zero Data Retention, at least one AI model provider that supports it must already be set up for your platform.

## How to use it

### Change a company AI control

1. Go to **Settings** → **Company AI controls**.
2. Turn **Allow memory**, **Enforce Zero Data Retention** or **Allow turning compaction off** on or off.
3. Read the question that appears under the switch, for example "Turn memory off for everyone? Every member's stored memory will be deleted."
4. Click **Confirm** to apply it, or cancel to leave it as it was.

### Limit how long chat summaries are kept

1. On **Company AI controls**, open **Keep memory chat summaries for at most**.
2. Choose **No company limit**, or 7, 14, 30, 60, 90, 180 or 365 days.
3. Click **Confirm**. Summaries older than the limit are deleted.

{% hint style="info" %}
People can choose a shorter period for themselves, never a longer one.
{% endhint %}

### Set a monthly AI budget

1. On **Company AI controls**, find the **Monthly AI budget** card.
2. Turn on **Limit AI usage**.
3. Enter an amount of AI use in **Tokens per month**, a spending cap in **Cost per month (USD)**, or both. Leave a box empty for no limit of that kind.
4. Click **Save budget**. You see **Saved.**, and a line shows how much has been used this month and the reset date.

{% hint style="info" %}
To lift the cap, turn **Limit AI usage** off and click **Save budget**. Your limits are kept for when you turn it back on.
{% endhint %}

### Turn a connector off for everyone

1. Go to **Settings** → **Connector access**.
2. Find the connector in its section and turn its switch off.
3. Read "Turn <name> off for everyone? Agents stop using it and nobody can connect it until it is turned back on." and click **Turn off**.

{% hint style="info" %}
The row then shows who turned it off and when. To turn it back on, switch it on again: it is available straight away, with no extra question.
{% endhint %}

### Choose who may connect an app

1. Click **Connectors** in the left rail and open the app's page.
2. In the side column, find **Who can enable this**.
3. Choose **Everyone in the company** (the default), **Specific roles** (Admins, Members) or **Specific groups**, and tick the roles or groups.
4. Click **Save access**. You see "Saved who can use this connector."

{% hint style="info" %}
Only the people you chose can connect the app, and each of them still signs in with their own account. Groups are set up on **Groups** ([Managing people](../for-admins/managing-people.md)).
{% endhint %}

## Your options

| Option | What it does |
|---|---|
| **Allow memory** | When off, nobody in the company can use memory, and every member's stored memory is deleted. |
| **Enforce Zero Data Retention** | Forces Zero Data Retention for every member: only AI model providers that don't keep your data are used, and everyone's memory is deleted. Turn it off and people choose for themselves again. |
| **Allow turning compaction off** | When off, members can't switch off conversation compaction (the way long chats are shortened so they keep working). |
| **Keep memory chat summaries for at most** | The longest anyone in the company may keep memory chat summaries. With **No company limit**, each person chooses between 30 and 180 days. |
| **Monthly AI budget** | Caps how much AI the whole company can use each calendar month. When it is used up, nobody in the company can ask the AI until 00:00 (Jakarta time) on the 1st of the next month, unless you raise the limit or turn it off. |
| Sections on **Connector access** | Connectors are grouped as **Connectors directory**, **Google Workspace** / **Microsoft 365** (Google products are switched one by one), **Custom connectors** (added in your organization) and **Shared connectors** (offered to every organization; turning one off affects only yours). |

## Good to know

* Company AI controls can only restrict. They never switch anything on for someone who turned it off.
* Turning **Allow memory** off, or **Enforce Zero Data Retention** on, deletes every member's stored memory. That can't be undone. Setting a summary limit deletes summaries older than the limit for everyone.
* The page shows who last changed these settings, and when.
* The monthly AI budget covers everything the company asks the AI: chats, tasks, agents in other products and the Slack and Google Chat bots. When it is used up, everyone's message box is locked with "Your company's monthly AI budget is used up. You can ask again on <date>."
* Only admins see how much of the budget has been used. Nobody gets an email or notification when it is nearly used up, so check the card now and then.
* The monthly AI budget is the same limit as the **Organization** budget on **Budgets**. Saving it here makes it a calendar-month budget.
* When a connector is turned off, people who open it see "Your organization's admin turned this connector off. Ask them to turn it back on in Connector access." The top of **Connector access** shows how many connectors are turned off.
* Each person still controls their own memory and data choices within your limits ([Your AI data & memory](../guides/your-ai-data-and-memory.md)).

## Ideas to try

* Before a sensitive project, turn on **Enforce Zero Data Retention** for the whole company.
* Set **Keep memory chat summaries for at most** to 30 days to match your data policy.
* Set a **Cost per month (USD)** cap that matches your AI spending plan, and check the usage line each week.
* Limit a new connector to a "Pilot" group with **Specific groups** before you open it to everyone.

## If something goes wrong

| What you see | What to do |
|---|---|
| "ZDR needs at least one ZDR-eligible model provider configured first." | Ask your platform owner to set up an AI model provider that supports Zero Data Retention, then try again. |
| "Another admin changed these settings. Reload to see the latest." | Reload the page, check the new values, and make your change again. |
| **Save budget** stays greyed out with **Set a token limit, a cost limit, or both.** | Enter a number in **Tokens per month**, **Cost per month (USD)**, or both, then save. |
| The card says "The budget is used up. Nobody in the company can ask the AI until <date>, unless you raise the limit or turn it off." | Raise a limit and click **Save budget**, or turn **Limit AI usage** off and save. Others can ask again after they reload Envoy. |
| A connector doesn't appear on **Connector access** | Sections with no connectors are hidden. Check the other sections, or ask whether it has been added for your company. |

## Related guides

* [Getting started](../guides/getting-started.md)
* [Connectors (connect your apps)](../guides/connectors.md)
* [Your AI data & memory](../guides/your-ai-data-and-memory.md)
* [Managing people](../for-admins/managing-people.md)
