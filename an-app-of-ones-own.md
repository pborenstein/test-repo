---
title: "An app of one's own"
source: "https://www.contraption.co/app-of-ones-own/"
author: ""
published: "2025-05-16"
created: "2025-07-04"
description: "Personal software for life automation"
tags: []
date: "2025-07-04"
siphon: "pborenstein/test-repo"
---

Personal software for life automation

[Philip I. Thomas](https://www.philipithomas.com/)

![Sunset iJenner, CA](https://www.contraption.co/content/images/2025/05/jenner.jpg)

When I was in third grade, my dream was to have a PalmPilot. My teacher had one, and the idea of having digital assistant in my pocket seemed like science fiction to me. Decades later, the iPhone has transformed life, yet leaves a lot to be desired in terms of autonomy and intelligence.

I have built many apps for other people. Recently, I began building one just for myself. I call it Junk Drawer, a home for my personal data, scripts, and workflows. My app has become a way to apply AI in fun ways in my life, and I think more people should make a small, private app of their own.

With the rise of vibe coding, building software has become easier, and more people are experimenting. Instead of buying software products just for one feature - like a [link shortener](https://www.youtube.com/watch?v=HuIFFTiodIA&ref=contraption.co) — you can just build it yourself.

Building software for others requires a lot of overhead: user accounts, integrations, and configuration screens. As a codebase matures, you layer on email notifications, error monitoring, and scheduled actions such as “send a summary every Monday.”

My first instinct was to spin up a separate app for each tool I wanted — but I soon found it easier to bundle everything into one project. By housing all my personal tools in a single [Rails](https://www.contraption.co/rails-versus-nextjs/) app, I reuse the same configuration, login, [recurring jobs](https://guides.rubyonrails.org/active_job_basics.html?ref=contraption.co), and notifications instead of rebuilding them each time. And, I can keep the choices weird - like sending notifications over [Signal](https://signal.org/?ref=contraption.co) instead of email. That’s where an app of one’s own shines: it can be a smorgasbord of features.

Here are some features already in Junk Drawer:

- When someone joins my mailing list, the app uses AI to research and tell me about them.
- When I publish here, it uses AI to analyzs the essay and recommend how to share it on LinkedIn text for a LinkedIn post to share the article. (I may add an automatic BlueSky feed, too.)
- On the first day of the month, it sends a reminder to post my [newsletter](https://www.philipithomas.com/posts/how-to-replace-social-media-with-a-personal-newsletter?ref=contraption.co) on [my website](https://www.philipithomas.com/?ref=contraption.co).
- It embeds [Blazer](https://github.com/ankane/blazer?ref=contraption.co) dashboards for data from Postcard, Booklet, and Ghost on my Toolbox server.
- A homepage built with [98.css](https://jdan.github.io/98.css/?ref=contraption.co) links to every app running on the server.

Planned additions include indexing two decades of Gmail in [Chroma](https://trychroma.com/?ref=contraption.co) for better search, integrating [Maybe Finance](https://github.com/maybe-finance/maybe?ref=contraption.co) for spending insights, and automating accounting tasks.

Today, the two most useful enablers for a personal app are APIs and AI. APIs expose your scattered data—emails, credit-card transactions, calendars. [Zapier](https://zapier.com/?ref=contraption.co) used to bridge those gaps, but your own app can do it more directly (and for free).

AI’s capabilities still outpace most products that claim to use it. The essay [“AI Horseless Carriages”](https://koomen.dev/essays/horseless-carriages/?ref=contraption.co) argues that the best patterns remain undiscovered. ChatGPT is powerful, yet many apps over-simplify their AI features. A personal app can close that gap: draft email replies, build a daily schedule with background research on each meeting, or flag unusual credit-card charges — all based on your preferred prompts.

Companies could adopt a separate “vibes” app as well. Production systems guard customer data behind code reviews, staging, and alerts. An isolated internal app— disconnected from customer information — could handle informal tasks such as Doordash lunch orders, looking up who's on-call, or searching internal docs - enabling employees to prototype freely.

Building an app for myself has been rewarding. I can take an idea, code it, and deploy it to [my server](https://www.contraption.co/a-mini-data-center/) in minutes. Each feature can be a sandbox for experimenting with AI on my real-world data.

Since childhood I have wanted a digital assistant in my pocket. AI is enabling a new frontier of customization. But, to really build the automations you want on your own data, try building an app for yourself.