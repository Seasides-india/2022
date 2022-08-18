---
key: unicorn_private_database
title: How We Got Into A Unicorn’s Private Codebase
id: PmoMEVHO3imfUIMXsPai12
language: English
format: hands-on
tags:
  - research
level: beginner
speakers:
  - arshit_jain
videoId: 
<!--presentation: https://www.blockchainvillage.net/ -->
draft: false
---

<!-- <a align="center" class="btn primary" target="_blank" rel="noopener" href="https://forms.gle/x7tbBKrf3eoVJ7UJ9">Register</a>  -->

**How We Got Into A Unicorn’s Private Codebase**

**Abstract**:

Reading a **$120 million worthy unicorn startup's private codebase** on a fine Sunday afternoon while sipping on coffee would be an exciting experience, wouldn't it? It’s not a very uncommon phenomenon. Only last year, Twitch was added to the long line of organizations whose source code has been made public inadvertently. Twitch's source code, which includes 6,000 internal Git repositories and 3,000,000 documents with a combined unzipped size of 200GB, was exposed to the 4chan forum.

Here's how wtechtalk_threathuntinge got access to **159 private codebases** of  **13 organizations** ranging from small-scale startups to leading unicorns. 
- First, we examined an unending number of GitHub tokens and secrets being hardcoded into mobile applications by decompiling multiple apps and found that the leading use case was hardcoding GitHub tokens in Git URLs to import packages.
- In that giant pool of tokens, we also discovered hardcoded client secrets and IDs for Oauth applications. With these OAuth tokens, someone can make an app of their own to impersonate a legitimate organization which they can use to steal sensitive data from customers of that organization. We could clone private repositories and gain full access to confidential source code.
- Moreover, with a hardcoded Personal Access Token (PAT), the attacker could masquerade as the person whose PAT has been leaked, therefore accessing private repositories, making commits issues, pulling requests as the person whose PAT has been revealed, and much more. Scary, right? 

It's not unusual for developers to hardcode sensitive information in their source code and then submit it to popular code-sharing platforms like GitHub. According to GitGuardian, 6 million hardcoded secrets will be discovered in 2021, with India being the leading source of leaks and an increase of 2 times compared to 2020. Considering that GitGuardian’s studies are limited to only public repositories hosted on GitHub or GitLab and not secrets being committed in private repositories or self-hosted git clients it is astounding that no directed research has been conducted to reveal the different use cases of these hardcoded tokens apart from version-control platforms. Hence, in our study, we directly explore the source code of millions of mobile apps and find out these instances of leaks directly. In this talk, we plan on investigating the causes, impacts, and techniques that can be used to prevent such leaks. Further, we'll be giving you a sneak peek into some of our interesting findings.

**Duration**: 30 mins


**About Trainer**
**Arshit Jain** is working as a senior security engineer in Cloudsek.His main responsibility includes handling the backend of BeVigil,the world first security search engine for mobile apps.His interest lies in automating anything and everything that requires manual efforts.He likes to travel,read books and play any sports in his free time.

<!--
<a align="center" class="btn primary" target="_blank" rel="noopener" href="https://docs.google.com/forms/d/1l0JWU9j-t_i0xJDF6NK7SPQoevcGx_ijkmsMoyvmxPk">Register</a>
-->
