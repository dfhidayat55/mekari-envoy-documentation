# Managing people

{% hint style="success" %}
**General Guide** — for everyone, no technical knowledge needed.
{% endhint %}

| | |
|---|---|
| **Who this is for** | Company admins |
| **Where to find it** | **Settings** → **Users**, **Groups** and **Organizations** (under **Workspace**) |
| **Last checked** | 24 October 2026 |

## What it is

These three pages are where an admin decides who can use Envoy in your company and what they can do.

**Users** lists everyone who can sign in to your company in Envoy, plus anyone you have invited who hasn't signed in yet. Here you invite people, change their role and remove them. **Groups** are named sets of people, used to limit who can connect a connector, who an agent is shared with, and who can use a knowledge base collection (its **Who can use this** setting, see [Knowledge base](../guides/knowledge-base.md)). **Organizations** shows the companies you belong to and lets you rename yours.

Only admins see these pages. Members and viewers don't.

## Before you start

* You need the admin role in your company.
* Have the person's work email address ready. It must be exactly the address they sign in to Envoy with (today that is their work Google account, through **Sign in with Google**). If they sign in with a different address, Envoy shows **Access Not Granted** and doesn't let them in.

## How to use it

### Invite someone

1. Go to **Settings** → **Users** and click **Invite user**.
2. Enter their **Work email**.
3. Choose a **Role**. A short description of what that role can do appears under the field.
4. Click **Send invite**.
5. Envoy confirms that the person can now join. Send them a link to Envoy yourself so they can sign in.

{% hint style="info" %}
If the person already has an Envoy account, they are added straight away. Otherwise they appear on the list as **Not signed in yet**, with the date they were invited and when the invite expires.
{% endhint %}

### Find someone on the list

1. Type in **Search name or email**.
2. Use **All roles** to show only one role.
3. Use the membership filter: **All**, **Members** (signed in) or **Invited** (not signed in yet).
4. Read the columns **User**, **Role**, **Groups** and **Joined date**.

### Change someone's role

1. Find the person on **Users**.
2. Pick a new role in their **Role** column.
3. Envoy confirms the change, for example "Ani is now a member."

{% hint style="info" %}
Your own role is shown but locked: another admin has to change it.
{% endhint %}

### Remove someone or cancel an invite

1. Click the actions button (three dots) at the end of the person's row.
2. Click **Remove** for a member, or **Revoke invite** for someone who hasn't signed in yet.
3. For a member, choose what happens to the work they own: **Transfer their work to another member** (then pick someone in **Transfer to**), or **Leave their work in place**.
4. Click **Remove** (or **Revoke invite**) to confirm.

{% hint style="info" %}
With **Transfer their work to another member**, their agents, knowledge, skills and tasks move to that person and the tasks keep running. With **Leave their work in place**, their tasks are stopped and deleted; their agents, knowledge and skills stay as they are.
{% endhint %}

### Create a group

1. Go to **Settings** → **Groups** and click **New group**.
2. Enter a **Group name** (for example "Finance team" or "Consultants") and, if you like, a **Description**.
3. Click **Create group**.

### Manage a group

1. On **Groups**, click the actions button on the group's row.
2. Click **Manage members**, choose people under **Add a member**, remove anyone who shouldn't be there, and click **Done**.
3. Click **Rename** to change its name, or **Delete** to remove the group.

### Rename your organization

1. Go to **Settings** → **Organizations**. Use **Search...** if you belong to several.
2. Click the actions button on the organization's row, then **Edit**.
3. Change the **Name** in **Edit organization** and click **Save changes**.

{% hint style="info" %}
The **Organization ID** is shown for reference and can't be changed.
{% endhint %}

## Your options

| Option | What it does |
|---|---|
| **admin** | Full access. Manages the organization, its users, and every setting. |
| **member** | Works day-to-day: uses the assistant, agents, skills, and documents. This is the default for a new invite. |
| **viewer** | Read-only access. Cannot make changes or view credentials. |

## Good to know

* Envoy doesn't email invites yet. After you invite someone, send them a link to Envoy yourself.
* An invite expires after 30 days. Once it has expired you can invite the same address again.
* An address can have only one pending invite at a time.
* Your company must always keep at least one admin, so the last admin can't be made a member or viewer, or removed.
* You can't change your own role or remove yourself. To leave, switch organization or sign out.
* A removed person loses access at once and is signed out of your organization. The apps they connected in your company (for example their Google or Microsoft account) are disconnected. Their chats stay private to them. Their access to other companies isn't affected.
* Deleting a group takes everyone out of it. The people themselves stay in your company.
* Only people who already belong to your company can be added to a group. Group names must be unique and 1–80 characters long; organization names can be up to 80 characters.
* Only Envoy's platform owners can create or archive organizations. Archiving signs everyone out of that organization but keeps its data. As an admin you can rename yours.

## Ideas to try

* Invite a new teammate as a **member**, then add them to the right group so they can use the team's agent.
* Create a "Consultants" group and use it to limit who can use a sensitive connector or knowledge base.
* Filter **Users** by **Invited** to chase people who haven't signed in yet.

## If something goes wrong

| What you see | What to do |
|---|---|
| "They are already in this organization." | The person is already a member. Find them on the list and change their role if needed. |
| "They already have a pending invite." | Wait for them to sign in, or click **Revoke invite** on their row and invite them again. |
| "Enter a valid work email address." | Check the address for typos. |
| "This company must keep at least one admin." | Make someone else an admin first, then change or remove this person. |
| "You cannot remove yourself. Switch organization or sign out instead." | Ask another admin to remove you, or switch organization or sign out. |
| "Choose another member of this organization to receive their work." | The person you picked in **Transfer to** is no longer a member. Pick someone else, or choose **Leave their work in place**. |
| "A group with that name already exists." | Pick a different group name. |
| "Only people who already belong to this company can be added." | Invite them on **Users** first. Add them to the group after they have joined. |
| "Couldn't load people." | Click **Retry**. |

## Related guides

* [Getting started](../guides/getting-started.md)
* [Agents](../guides/agents.md)
* [Connectors (connect your apps)](../guides/connectors.md)
* [Knowledge base](../guides/knowledge-base.md)
* [Company AI controls & Connector access](../for-admins/company-ai-controls-and-connector-access.md)
