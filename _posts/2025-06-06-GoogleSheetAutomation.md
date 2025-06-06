---
title: GoogleSheets Automation with Gemini 2.5 Pro
categories: [Projects with AI]
tags: [GoogleSheets, Google Workspace, Gmail, Automation, AppScript,Gemini 2.5 Pro ]
date: 2025-06-06 16:15:00 +0200
---

# My First AI Project
This week, I'd like to share a small project I recently developed and I'm really proud of!

It's not about how simple it is, but about how powerful AI can be in saving us time and improving our work and productivity. If more people took the time to explore these tools and try things hands-on, imagine how far we could go.

# Background - Remedy
Before we jump into the project itseld, let me give you a bit of context and why it came to life.

I work in a Consulting company, and I'm always trying to find ways to be more productive and effiecient using AI.

Recently, our team was overwhelmed by a large number of emails coming from a system called Remedy.

*Note: For those unfamiliar, Remedy is a ticketing tool used by companies to track incidents, tasks, or user requests. It can also notify external vendors about issues.*

Due to some internal changes, we were reciving duplicated tickets. The problem? We couldn't always tell which tickets needed our attention and which didn't. We tried working with the client on a solution but they couldn't change anything without us losing visibility of some tasks that we might have to handle.

# Solutions Discussed
Like anyone else, we first thought of traditional ways to solve the problem. 

Here’s what we considered:

* Send all the emails to Spam and have someone on the team manually check them from time to time.
* Remove ourselves from the notification group so we’d only receive emails assigned directly to us.
* 
Unfortunately, the second option wasn’t possible, as we risked missing tasks when someone from the internal client team was on holiday and had no backup.

And the first option? Too much hassle, too much time wasted.

So I started thinking—maybe AI could help us here.

# Google Sheets

Internally, we use Google Sheets to keep track of our project tasks. We recently created a new tab to track Remedy tickets.

Before this project, I had to manually go through each email and fill in the ticket details. It was repetitive, slow, and annoying.

Then I thought: *Can’t this be done faster? Automatically?*

Why? Because these emails always followed the same pattern. They usually started with:

"You have been assigned…"
"Your group has been assigned…"
"Has been assigned to you…"

Since we have access to Google Workspace tools, I decided to ask Gemini for help.

# Gemini
Here’s the first prompt I gave Gemini:

```text
I want to create some kind of google sheet tab that is connected to my email and I want ti to get filled ul with certain information of the subject of my email and the date it arrives
```

I didn't have a clear idea yet of the structure of my Google Sheet, but Gemini gave me a great answer:

> You can defintely create a Google Sheet that automatically populates with subject and arrival date of your emails! This is tipically done using **Google Apps Scripts**, a JavaScript-based platform that allows you to extend and automate Google Workspace applications like Gmail and Sheets

With just my second prompt, Gemini gave me a working script to test:

```text
Can you help me do it? I've created the table and I want to fill the columns Task and Start.

I want the column Task to be filled with a specific information of the Suvject and the Start to be filled with the date I received the email
```

After that, I just had to be more specific about the email patterns so Gemini could extract exactly the information I needed.

# End Result

Success! 

Right now we have a fully automated Google Sheet that shows only the tickets we need to handle. The rest? Still in our email, but no longer cloggin our main inbox. No more spam folder drama. 

Here's (blurred) picture of the final result on the Google Sheets.

![Google Sheets](/assets/GoogleSheets.jpeg)

And here's an example of the types of emails we were receiving:

![Email](/assets/Email.jpeg)

In case anyone anyone also wants to give it a try at making their work easier, I'll be also sharing the code. 

# Want to Try It?
If you're also looking for ways to make your job easier using AI, I’ll be sharing the code I used in this project on my github.

Stay tuned!