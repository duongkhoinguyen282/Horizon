---
layout: default
title: "Horizon Summary: 2026-07-02 (EN)"
date: 2026-07-02
lang: en
---

> From 29 items, 13 important content pieces were selected

---

1. [Podman v6.0.0 Released with Architectural and Networking Improvements](#item-1) ⭐️ 9.0/10
2. [Virginia Enacts Ban on the Sale of Geolocation Data](#item-2) ⭐️ 8.0/10
3. [Linux 6.9 Regression Fails to Wipe LUKS Encryption Keys During Suspend](#item-3) ⭐️ 8.0/10
4. [A Practical Guide to Requesting Assistance from Strangers](#item-4) ⭐️ 8.0/10
5. [Immich 3.0 Release and Community Reflections](#item-5) ⭐️ 8.0/10
6. [Using DSPy to evaluate and improve Datasette Agent's SQL system prompts](#item-6) ⭐️ 8.0/10
7. [Understand to participate: Maintaining developer agency in the age of AI agents](#item-7) ⭐️ 8.0/10
8. [Exapunks: A Deep Dive into Low-Level Programming Through Puzzle Gaming](#item-8) ⭐️ 7.0/10
9. [PeerTube: A Decentralized and Federated Video Hosting Platform](#item-9) ⭐️ 7.0/10
10. [Simon Willison Releases llm-coding-agent 0.1a0](#item-10) ⭐️ 7.0/10
11. [Anthropic Restores Access to Claude Fable 5 and Mythos 5 Models](#item-11) ⭐️ 7.0/10
12. [Resources for Strengthening Mathematical Foundations in Machine Learning Research](#item-12) ⭐️ 7.0/10
13. [The Ethical Implications of 'Paper Fishing' and Gift Authorship in Academia](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Podman v6.0.0 Released with Architectural and Networking Improvements](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 9.0/10

Podman v6.0.0 introduces significant architectural refinements and enhanced networking capabilities, further solidifying its role as a robust, daemonless container engine. This release focuses on improving performance and stability for both rootless and rootful container deployments. As a major version release, Podman v6.0.0 represents a significant milestone in the container ecosystem, offering a more secure and efficient alternative to traditional daemon-based engines like Docker. It provides developers with better integration options and improved performance for complex containerized workflows. The update includes refined networking stacks and deeper integration with system-level tools, ensuring better compatibility with existing container-compose files. Users can expect improved performance in rootless mode, leveraging advanced networking backends.

hackernews · soheilpro · Jul 2, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48762098)

**Background**: Podman is an open-source, daemonless container engine designed to be a drop-in replacement for Docker. Unlike Docker, which relies on a central background daemon to manage containers, Podman uses a fork/exec model that allows containers to run as child processes of the user. This architecture enhances security by reducing the attack surface and allows for easier integration with system management tools like Systemd.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.redhat.com/blog/2018/11/20/buildah-podman-containers-without-daemons">Containers without daemons: Podman and Buildah available in RHEL 7.6 and RHEL 8 | Red Hat Developer</a></li>
<li><a href="https://docs.podman.io/en/stable/markdown/podman-network.1.html">podman-network — Podman documentation</a></li>

</ul>
</details>

**Discussion**: The community is generally positive, praising the daemonless architecture and ease of migration from Docker, though some users express concerns about minor compatibility differences. Discussions also highlight the utility of Quadlet for system integration and compare Podman's performance against alternatives like OrbStack on macOS.

**Tags**: `#Podman`, `#Containers`, `#DevOps`, `#Linux`, `#Docker`

---

<a id="item-2"></a>
## [Virginia Enacts Ban on the Sale of Geolocation Data](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

Virginia has officially implemented a law prohibiting the sale of precise geolocation data, which went into effect on July 1. This legislation marks a significant update to the state's existing Consumer Data Protection Act. This law provides critical protections against the unauthorized monetization of sensitive location tracking, which has previously been used for controversial purposes like targeted advertising based on visits to sensitive locations. It represents a growing trend of state-level intervention to curb data privacy abuses. The legislation amends the Virginia Consumer Data Protection Act to restrict the sale of precise geolocation data, with enforcement handled by the state's Attorney General. Penalties for non-compliance can reach up to $7,500 per violation.

hackernews · toomuchtodo · Jul 2, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48767347)

**Background**: Geolocation data is typically collected by smartphones through GPS, Wi-Fi signals, and cellular network pings. While often used to provide location-based services, this data is frequently scrubbed of direct identifiers and sold to third-party brokers for advertising or behavioral analysis. Virginia's Consumer Data Protection Act (VCDPA) serves as the primary framework for these privacy regulations.

<details><summary>References</summary>
<ul>
<li><a href="https://lis.virginia.gov/bill-details/20261/SB338/text/CHAP0820">CHAP0820 - 2026 Regular Session | LIS - lis.virginia.gov</a></li>
<li><a href="https://privacylawmap.com/states/virginia">Virginia VCDPA Privacy Law Compliance Guide 2026 | Consumer ...</a></li>
<li><a href="https://www.techtarget.com/searchmobilecomputing/definition/What-is-geolocation">What is geolocation? Explaining how geolocation data works</a></li>

</ul>
</details>

**Discussion**: The community expressed strong support for the ban, citing concerns over the misuse of location data for sensitive tracking, such as visits to medical clinics. However, users also raised questions regarding jurisdictional enforcement and the potential for companies to bypass these rules if they operate outside of Virginia.

**Tags**: `#privacy`, `#data-protection`, `#legislation`, `#geolocation`, `#cybersecurity`

---

<a id="item-3"></a>
## [Linux 6.9 Regression Fails to Wipe LUKS Encryption Keys During Suspend](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

A regression introduced in Linux kernel 6.9 prevents the system from properly wiping LUKS disk-encryption keys from memory during a suspend operation. This failure leaves sensitive encryption keys exposed in RAM while the system is in a suspended state. This bug poses a significant security risk for users who rely on memory wiping to protect their data against physical access or cold-boot attacks. It highlights how silent regressions in core kernel functionality can undermine established security practices. The issue specifically affects the `cryptsetup luksSuspend` operation, which is often used to secure data before a system enters a low-power state. Community members noted that this functionality is not universally supported across all distributions, potentially limiting the scope of the impact.

hackernews · IngoBlechschmid · Jul 2, 15:25 · [Discussion](https://news.ycombinator.com/item?id=48763035)

**Background**: LUKS (Linux Unified Key Setup) is the standard for disk encryption in Linux, ensuring that data on a drive remains inaccessible without the correct passphrase. Suspend-to-RAM allows a computer to enter a low-power state while keeping data in memory, whereas hibernation writes the contents of RAM to the disk and powers off the machine entirely.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Linux_Unified_Key_Setup">Linux Unified Key Setup - Wikipedia</a></li>
<li><a href="https://wiki.archlinux.org/title/Power_management/Suspend_and_hibernate">Power management/ Suspend and hibernate - ArchWiki</a></li>

</ul>
</details>

**Discussion**: The community debated whether this is a critical kernel bug or an issue with specific distribution implementations like Debian. Some users argued that the title is sensationalist, while others emphasized that security regressions are often difficult to detect because the system appears to function normally.

**Tags**: `#linux-kernel`, `#security`, `#luks`, `#encryption`, `#regression`

---

<a id="item-4"></a>
## [A Practical Guide to Requesting Assistance from Strangers](https://pradyuprasad.com/writings/how-to-ask-for-help/) ⭐️ 8.0/10

Pradyun Gedupudi provides a structured guide on how to effectively reach out to strangers for help by emphasizing clarity, demonstrating prior effort, and respecting the recipient's time. The guide outlines actionable steps to increase the likelihood of receiving a positive response. Mastering professional communication is essential for career growth and networking, especially when seeking mentorship or advice from experts. This guide helps individuals avoid common pitfalls that lead to ignored requests. The author highlights the importance of 'proof of work,' suggesting that showing you have attempted to solve the problem independently is the most effective way to earn someone's time. It also advises keeping initial communications concise to reduce the cognitive load on the recipient.

hackernews · FigurativeVoid · Jul 2, 13:19 · [Discussion](https://news.ycombinator.com/item?id=48761118)

**Background**: In professional and technical communities, cold outreach is a common method for networking or troubleshooting. However, many people struggle with crafting requests that are respectful and likely to succeed. This guide addresses the soft skills required to bridge the gap between strangers in a professional context.

**Discussion**: The community highly values the advice, noting that proof of work must go beyond surface-level efforts to be effective. Commenters also suggest that one's perception of how busy a recipient is can often be inaccurate, so it is better to focus on the quality of the request rather than overthinking the recipient's schedule.

**Tags**: `#professional-development`, `#networking`, `#communication`, `#career-advice`, `#soft-skills`

---

<a id="item-5"></a>
## [Immich 3.0 Release and Community Reflections](https://github.com/immich-app/immich/discussions/29439) ⭐️ 8.0/10

The Immich community is discussing the release of version 3.0, which continues to solidify the platform's position as a leading self-hosted alternative to major cloud photo services. Immich is significant because it allows users to regain control over their personal media data while offering a user experience comparable to Google Photos or Apple Photos. It addresses the growing demand for privacy-focused, high-performance self-hosted software. While highly praised for its interface and features, users continue to report challenges with mobile synchronization reliability. Some users are also comparing Immich to encrypted alternatives like Ente for enhanced security.

hackernews · hashier · Jul 2, 14:13 · [Discussion](https://news.ycombinator.com/item?id=48761944)

**Background**: Immich is an open-source, self-hosted photo and video management solution that provides features like facial recognition, smart search, and automatic mobile uploads. It is designed to run on a user's own hardware, ensuring that media files remain private and under the user's complete control. This approach is popular among privacy enthusiasts who want to avoid the data harvesting practices of large tech companies.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/immich-app/immich">GitHub - immich-app/immich: High performance self - hosted photo ...</a></li>
<li><a href="https://aicybr.com/blog/immich-complete-self-hosting-guide">Immich Complete Self-Hosting Guide: From Installation to ...</a></li>
<li><a href="https://use-apify.com/blog/google-photos-alternatives-2026">5 Self - Hosted Google Photos Alternatives (2026) | Use Apify</a></li>

</ul>
</details>

**Discussion**: The community sentiment is largely positive, with many users praising Immich as a 'no-brainer' replacement for cloud services. However, some users expressed concerns regarding the stability of mobile sync and highlighted the benefits of end-to-end encrypted alternatives like Ente.

**Tags**: `#self-hosting`, `#open-source`, `#photography`, `#data-privacy`, `#immich`

---

<a id="item-6"></a>
## [Using DSPy to evaluate and improve Datasette Agent's SQL system prompts](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 8.0/10

Simon Willison is utilizing the DSPy framework to systematically evaluate and optimize the system prompts used by Datasette Agent for generating SQL queries. The process involves automated testing to identify and fix inefficiencies in how the agent interacts with database schemas. This approach shifts prompt engineering from manual guesswork to a data-driven, programmatic workflow, significantly improving the reliability of LLM-based SQL agents. It demonstrates how developers can use modern frameworks to reduce error-retry loops and enhance query accuracy. The research identified that providing only table names in the schema listing led to excessive guessing and error-retry loops. The suggested fix is to include column names directly in the prompt or adjust the agent's instructions regarding schema exploration.

rss · Simon Willison · Jul 2, 18:25

**Background**: DSPy is a Python framework that enables developers to build LLM applications using modular, declarative programming instead of manual prompt engineering. Datasette Agent is an AI assistant designed to help users explore and query data within Datasette by automatically generating and executing SQL queries.

<details><summary>References</summary>
<ul>
<li><a href="https://agent.datasette.io/">Datasette Agent : an AI assistant for Datasette to help explore and...</a></li>
<li><a href="https://simonwillison.net/2026/May/21/datasette-agent/">Datasette Agent | Simon Willison’s Weblog</a></li>

</ul>
</details>

**Tags**: `#DSPy`, `#LLM`, `#Prompt Engineering`, `#Datasette`, `#SQL`

---

<a id="item-7"></a>
## [Understand to participate: Maintaining developer agency in the age of AI agents](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 8.0/10

Geoffrey Litt argues that developers must maintain a deep conceptual understanding of their codebase to remain active participants in the creative process alongside AI coding agents. He emphasizes that failing to do so leads to cognitive debt, which limits a developer's ability to evolve projects effectively. As AI agents take on more complex coding tasks, developers risk losing their mental model of the system, which is essential for creative problem-solving and long-term project maintenance. This perspective highlights the critical balance between leveraging automation and retaining human technical expertise. The concept of 'cognitive debt' refers to the erosion of shared understanding within a team or individual regarding how a software system functions. Developers are encouraged to actively learn what the agent is doing to ensure they remain fluent in the project's logic.

rss · Simon Willison · Jul 2, 17:07

**Background**: AI coding agents are advanced tools capable of modifying files, creating directories, and handling complex refactoring tasks in modern IDEs. Cognitive debt is a growing concern in software engineering, representing the gap between the actual system complexity and a developer's mental model of that system. As these agents automate more work, the risk of developers becoming passive observers rather than active architects increases.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.22106">From Technical Debt to Cognitive and Intent Debt: Rethinking ...</a></li>
<li><a href="https://getdx.com/blog/cognitive-debt-the-hidden-risk-in-ai-driven-software-development/">Cognitive debt: The hidden risk in AI-driven software development</a></li>

</ul>
</details>

**Tags**: `#AI Engineering`, `#Software Development`, `#Human-AI Collaboration`, `#Cognitive Debt`

---

<a id="item-8"></a>
## [Exapunks: A Deep Dive into Low-Level Programming Through Puzzle Gaming](https://www.zachtronics.com/exapunks/) ⭐️ 7.0/10

Exapunks is a puzzle game from Zachtronics that tasks players with writing assembly-like code to hack virtual computer systems. It gamifies the experience of low-level programming by requiring players to manage data and navigate networks. The game is highly regarded for its ability to demystify assembly language and systems architecture for non-experts. It serves as an engaging educational tool that fosters problem-solving skills and logical thinking within the engineering community. Players must balance code efficiency with system constraints, often learning that iterative optimization is more effective than premature optimization. The game provides a sandbox environment that makes complex concepts like memory management and network protocols accessible.

hackernews · yu3zhou4 · Jul 2, 18:41 · [Discussion](https://news.ycombinator.com/item?id=48765663)

**Background**: Zachtronics is a renowned independent game studio known for its 'zach-like' genre, which emphasizes engineering, logic, and system optimization. These games often require players to build automated solutions using restricted instruction sets, mimicking real-world constraints found in embedded systems and low-level programming.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zachtronics">Zachtronics - Wikipedia</a></li>
<li><a href="https://softwareengineeringdaily.com/2025/12/18/designing-innovative-puzzle-games-with-zachtronics-with-zach-barth/">Designing Innovative Puzzle Games with Zach Barth</a></li>

</ul>
</details>

**Discussion**: The community highly praises Exapunks for its career-shaping influence and ability to make assembly language approachable. Users also recommend exploring the developer's other titles and note that playing with friends adds a fun, competitive layer to the puzzle-solving experience.

**Tags**: `#gaming`, `#programming`, `#assembly`, `#education`, `#zachtronics`

---

<a id="item-9"></a>
## [PeerTube: A Decentralized and Federated Video Hosting Platform](https://github.com/Chocobozzz/PeerTube) ⭐️ 7.0/10

PeerTube is an open-source, federated video hosting platform that utilizes P2P technology to distribute bandwidth load among viewers. It allows users to host their own instances or join existing ones to share video content without relying on a central authority. It offers a resilient alternative to centralized platforms like YouTube by preventing single points of failure and promoting user sovereignty. This model is crucial for creators and communities seeking to avoid algorithmic control and platform censorship. The platform leverages WebTorrent for P2P video distribution, which significantly reduces the server-side bandwidth requirements for popular videos. However, it currently lacks robust monetization features and centralized discovery tools found on mainstream platforms.

hackernews · doener · Jul 2, 11:17 · [Discussion](https://news.ycombinator.com/item?id=48759634)

**Background**: PeerTube is part of the Fediverse, a collection of interconnected, decentralized social networks that communicate via the ActivityPub protocol. Unlike traditional platforms, it does not rely on a single company to store data or manage content. Instead, it operates as a network of independent servers that can interact with each other.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PeerTube">PeerTube - Wikipedia</a></li>
<li><a href="https://fediverse.party/">- Fediverse.Party - explore federated networks</a></li>
<li><a href="https://valebyte.com/en/blog/peertube-on-vps-installation-configuration-and-maintenance/">PeerTube on VPS: installation, configuration, and maintenance</a></li>

</ul>
</details>

**Discussion**: The community acknowledges PeerTube's technical potential for privacy and open-source advocacy but highlights significant barriers to mainstream adoption, specifically the lack of monetization for creators and limited content discovery. Some users find it useful for niche projects, while others argue it currently serves more as a distribution tool than a full-featured social platform.

**Tags**: `#decentralization`, `#fediverse`, `#video-hosting`, `#open-source`, `#web-infrastructure`

---

<a id="item-10"></a>
## [Simon Willison Releases llm-coding-agent 0.1a0](https://simonwillison.net/2026/Jul/2/llm-coding-agent/#atom-everything) ⭐️ 7.0/10

Simon Willison has released an alpha version of llm-coding-agent, a new Python library that extends his existing LLM framework to support autonomous file manipulation and command execution. The tool allows developers to perform tasks like editing files and running shell commands through natural language prompts. This release provides a transparent, practical example of how to build agentic workflows using established LLM libraries. It serves as a valuable resource for developers interested in the mechanics of AI-driven coding assistants and iterative tool development. The agent includes specific tools for reading, searching, and editing files, as well as executing shell commands with timeout protections. It can be installed via uvx and supports both a command-line interface and a Python API for programmatic control.

rss · Simon Willison · Jul 2, 19:33

**Background**: An agentic coding assistant is an AI system capable of autonomously interacting with a developer's environment to perform coding tasks. These systems typically use LLMs to reason about file structures, write code, and execute tests, often requiring careful sandboxing to ensure security. Simon Willison's 'llm' library is a popular open-source tool designed to simplify interactions with various LLM providers.

**Tags**: `#LLM`, `#AI Agents`, `#Python`, `#Developer Tools`, `#Automation`

---

<a id="item-11"></a>
## [Anthropic Restores Access to Claude Fable 5 and Mythos 5 Models](https://simonwillison.net/2026/Jun/30/anthropic/#atom-everything) ⭐️ 7.0/10

Anthropic announced that the U.S. Department of Commerce has lifted export controls on its advanced Claude Fable 5 and Mythos 5 AI models. The company began restoring global access to these models on July 1, 2026. This decision marks a significant shift in AI policy, allowing users worldwide to regain access to some of the most powerful frontier LLMs currently available. It highlights the growing tension between national security export controls and the global demand for advanced generative AI technology. Claude Fable 5 and Mythos 5 are designed for long-running, autonomous projects, featuring enhanced capabilities in software engineering and life sciences research. The models were previously restricted due to regulatory concerns regarding their potential dual-use applications.

rss · Simon Willison · Jun 30, 23:58

**Background**: Export controls are legal mechanisms used by governments to restrict the transfer of sensitive technologies to foreign entities for national security reasons. In the context of AI, these controls often target frontier models that possess advanced capabilities in areas like cybersecurity or biological research. Anthropic had been forced to temporarily pull these models from international markets following the initial imposition of these regulations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/07/01/anthropic-redeploys-claude-fable-5-on-july-1-after-us-export-controls-lift-adds-new-cybersecurity-classifier/">Anthropic Redeploys Claude Fable 5 on July 1 After US Export ...</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#anthropic`, `#export-controls`, `#generative-ai`, `#llms`, `#ai-policy`

---

<a id="item-12"></a>
## [Resources for Strengthening Mathematical Foundations in Machine Learning Research](https://www.reddit.com/r/MachineLearning/comments/1ulmy9g/booksresources_to_improve_mathematical/) ⭐️ 7.0/10

A PhD student has initiated a discussion to curate high-quality resources for mastering linear algebra, probability theory, and functional analysis to support advanced machine learning research. The request seeks alternatives to overly dense textbooks like Rudin's, focusing on practical, digestible materials for researchers. Strengthening mathematical foundations is critical for ML researchers to move beyond 'learning-as-you-go' and achieve a deeper understanding of complex algorithms. This discussion provides a community-vetted roadmap for bridging the gap between applied coding and theoretical rigor. The discussion highlights specific resources such as 'Linear Algebra Done Right', 'A Primer on RKHS', and Pat Kidger's 'Just-Know-Stuff' list. It emphasizes that the primary challenge is not finding materials, but the discipline required to work through them while managing academic duties.

reddit · r/MachineLearning · /u/mvreich · Jul 2, 16:24

**Background**: Functional analysis, particularly Reproducing Kernel Hilbert Spaces (RKHS), is essential for understanding modern statistical learning theory and kernel methods. Pattern Recognition and Machine Learning (PRML) by Christopher Bishop is a foundational text that bridges engineering and computer science perspectives in machine learning. These topics are often considered prerequisites for advanced research in high-dimensional data analysis.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Reproducing_kernel_Hilbert_space">Reproducing kernel Hilbert space - Wikipedia</a></li>
<li><a href="https://www.mdpi.com/2413-4155/4/4/40">A Concise Tutorial on Functional Analysis for Applications to Signal Processing</a></li>
<li><a href="https://link.springer.com/book/9780387310732">Pattern Recognition and Machine Learning | Springer Nature Link</a></li>

</ul>
</details>

**Discussion**: The community generally supports the proactive approach of revisiting fundamentals, often suggesting a mix of classic textbooks and modern, application-focused video series like 'The Bright Side of Mathematics'. Participants emphasize that consistent practice and working through proofs are more valuable than passive reading.

**Tags**: `#Machine Learning`, `#Mathematics`, `#Academic Research`, `#Education`

---

<a id="item-13"></a>
## [The Ethical Implications of 'Paper Fishing' and Gift Authorship in Academia](https://www.reddit.com/r/MachineLearning/comments/1ulgunh/what_do_you_think_about_paper_fishing_d/) ⭐️ 6.0/10

A recent discussion highlights the prevalence of 'paper fishing,' where researchers secure co-authorship on projects they did not contribute to, often to satisfy institutional productivity requirements. This practice undermines the integrity of academic research, misrepresents individual contributions, and creates systemic incentives that reward superficial output over genuine scientific advancement. Gift authorship occurs when individuals are added to papers without meeting standard authorship criteria, such as intellectual contribution or drafting the manuscript, often to maintain funding or progress reports.

reddit · r/MachineLearning · /u/impressivestatus21 · Jul 2, 12:26

**Background**: Academic authorship is intended to credit those who have made significant intellectual contributions and who take responsibility for the work. 'Gift' or 'honorary' authorship is widely considered a form of research misconduct, as it misleads the scientific community about who actually performed the research.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nature.com/nature-index/news/gift-ghost-authorship-what-researchers-need-to-know">The gift of paper authorship | News | Nature Index</a></li>
<li><a href="https://en.wikipedia.org/wiki/Academic_authorship">Academic authorship - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community generally condemns the practice as unethical and unprofessional, though many acknowledge that systemic pressures and toxic lab cultures often force researchers into these situations to survive.

**Tags**: `#academia`, `#research-ethics`, `#machine-learning`, `#career-development`, `#authorship`

---