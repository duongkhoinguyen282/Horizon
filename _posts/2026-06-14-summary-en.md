---
layout: default
title: "Horizon Summary: 2026-06-14 (EN)"
date: 2026-06-14
lang: en
---

> From 24 items, 15 important content pieces were selected

---

1. [US Government Orders Anthropic to Suspend Fable 5 and Mythos 5 Access](#item-1) ⭐️ 10.0/10
2. [Formal Methods and the Future of Programming](#item-2) ⭐️ 9.0/10
3. [Publishing WASM wheels to PyPI for use with Pyodide](#item-3) ⭐️ 9.0/10
4. [Coherent Context Can Silently Shift LLMs Into Different Internal Regimes](#item-4) ⭐️ 9.0/10
5. [Rio de Janeiro's 'Homegrown' LLM Allegedly a Weighted Merge of Existing Models](#item-5) ⭐️ 8.0/10
6. [Open-Source Knowledge Graph Pipeline Improves LLM Multi-Hop Reasoning](#item-6) ⭐️ 8.0/10
7. [The Verifier Tax: Horizon-Dependent Safety–Success Tradeoffs in Tool-Using LLM Agents](#item-7) ⭐️ 8.0/10
8. [Show HN: Kage – Shadow any website to a single binary for offline viewing](#item-8) ⭐️ 7.0/10
9. [Indexing 669 GB of GoPro footage using local ML on M1 Max](#item-9) ⭐️ 7.0/10
10. [Caddy compatibility for zeroserve: 3x throughput and 70% lower latency](#item-10) ⭐️ 7.0/10
11. [Mapping SQLite result columns back to their source table and column](#item-11) ⭐️ 7.0/10
12. [OpenAI WebRTC Audio Session Playground Adds GPT-Realtime-2 and Document Context](#item-12) ⭐️ 7.0/10
13. [Derivative-Free Neural Network Optimization Achieves Competitive Results on MNIST](#item-13) ⭐️ 7.0/10
14. [Simon Willison releases luau-wasm 0.1a0 for Pyodide](#item-14) ⭐️ 6.0/10
15. [Developer Launches Free Bilingual Machine Learning Notebook Course](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [US Government Orders Anthropic to Suspend Fable 5 and Mythos 5 Access](https://simonwillison.net/2026/Jun/13/us-government-directive-to-suspend-access/#atom-everything) ⭐️ 10.0/10

The US government has issued an emergency directive requiring Anthropic to block all foreign nationals from accessing its Fable 5 and Mythos 5 AI models. Anthropic has complied by disabling these models for all users to ensure full adherence to the national security order. This action marks a significant escalation in geopolitical intervention regarding AI, signaling that the US government is now actively enforcing strict export controls on frontier model access based on national security concerns. The government cited concerns over a potential jailbreak method, though Anthropic argues the capability is already widely available in other models like GPT-5.5. The restriction specifically targets foreign nationals, forcing a broad service outage to maintain compliance.

rss · Simon Willison · Jun 13, 01:01

**Background**: Jailbreaking in AI refers to techniques used to bypass safety guardrails, allowing models to perform restricted tasks. Recent US export controls, such as those introduced in early 2025, have increasingly focused on restricting the global diffusion of advanced AI model weights and capabilities to prevent misuse by foreign entities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sidley.com/en/insights/newsupdates/2025/01/new-us-export-controls-on-advanced-computing-items-and-artificial-intelligence-model-weights">New U.S. Export Controls on Advanced Computing Items and Artificial ...</a></li>
<li><a href="https://www.stblaw.com/about-us/publications/view/2025/01/15/bis-announces-worldwide-export-controls-on-advanced-chips-and-ai-models">BIS Announces Worldwide Export Controls on Advanced Chips and AI Models</a></li>
<li><a href="https://medium.com/aiguys/jailbreaking-generative-ai-how-hackers-unleash-llms-and-what-it-means-for-ai-safety-fe49d511a2a8">Jailbreaking Generative AI - How Hackers Unleash LLMs and What It...</a></li>

</ul>
</details>

**Discussion**: The community is expressing shock at the abrupt nature of the order and questioning the technical justification, given that similar capabilities exist in other models. Many are concerned about the precedent this sets for government control over private AI research and deployment.

**Tags**: `#AI Policy`, `#National Security`, `#Export Controls`, `#Anthropic`, `#AI Safety`

---

<a id="item-2"></a>
## [Formal Methods and the Future of Programming](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 9.0/10

Jane Street is exploring the integration of formal methods and highly expressive type systems to improve software correctness. This approach aims to leverage mathematical verification to ensure code reliability in an era increasingly dominated by AI-generated software. As AI tools generate massive amounts of code, traditional manual review becomes unsustainable, making automated verification essential for maintaining system integrity. This shift highlights a growing industry focus on using type systems and formal proofs to catch bugs that testing alone might miss. The approach emphasizes using expressive types to encode program invariants directly into the code, effectively turning the compiler into a verification tool. This reduces the need for extensive runtime testing and helps prevent common logic errors in complex systems.

hackernews · eatonphil · Jun 14, 12:35 · [Discussion](https://news.ycombinator.com/item?id=48526633)

**Background**: Formal methods are mathematically based techniques used to describe and verify system properties, ensuring that software behaves exactly as specified. Expressive type systems allow developers to define complex constraints within the code, which the compiler checks during the build process. These practices are increasingly relevant as developers seek ways to manage the risks associated with AI-assisted coding.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Type_system">Type system - Wikipedia</a></li>
<li><a href="https://ceur-ws.org/Vol-4076/paper9.pdf">How Important are Formal Methods and Formal Logic for Software ...</a></li>

</ul>
</details>

**Discussion**: The community discussion reflects a mix of nostalgia for classical proof automation, enthusiasm for using modern type systems like Scala 3 to enforce correctness, and skepticism regarding whether formal specs are just a more complex form of testing. Participants also noted that AI-generated code necessitates a shift in human effort toward verification rather than just writing new code.

**Tags**: `#formal-methods`, `#software-engineering`, `#type-systems`, `#verification`, `#programming-paradigms`

---

<a id="item-3"></a>
## [Publishing WASM wheels to PyPI for use with Pyodide](https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/#atom-everything) ⭐️ 9.0/10

Pyodide 314.0 now allows developers to publish WebAssembly-compatible Python wheels directly to PyPI, enabling them to be installed at runtime. This update aligns with the PyEmscripten platform defined in PEP 783. This change removes the significant bottleneck of manual package maintenance by the Pyodide team, allowing maintainers to distribute their own WASM-compatible packages just like native Python wheels. It represents a major step forward for the portability of Python extensions in the browser. Packages must target the PyEmscripten platform and can be built using standard tools like cibuildwheel. The new support was enabled by a PR to PyPI that landed on April 21st.

rss · Simon Willison · Jun 13, 23:55

**Background**: Pyodide is a technology that brings the Python runtime to the web browser by compiling it to WebAssembly (WASM). Previously, distributing Python packages with C or Rust extensions for Pyodide was difficult because the Pyodide maintainers had to manually build and host them in a custom repository. PEP 783 introduces a standardized way to package these files, making them compatible with standard Python distribution channels like PyPI.

<details><summary>References</summary>
<ul>
<li><a href="https://peps.python.org/pep-0783/">PEP 783 – Emscripten Packaging | peps .python.org</a></li>
<li><a href="https://news.lavx.hu/article/pypi-now-accepts-wasm-wheels-for-pyodide-via-pep-783-support">PyPI Now Accepts WASM Wheels for Pyodide via PEP 783 Support</a></li>

</ul>
</details>

**Discussion**: The community has expressed excitement about this release, as it significantly simplifies the workflow for developers who want to bring complex Python libraries to the browser. It is viewed as a long-awaited solution to a major maintenance burden.

**Tags**: `#Python`, `#WebAssembly`, `#Pyodide`, `#PyPI`, `#Packaging`

---

<a id="item-4"></a>
## [Coherent Context Can Silently Shift LLMs Into Different Internal Regimes](https://www.reddit.com/r/MachineLearning/comments/1u5xnxg/coherent_context_can_silently_shift_llms_into_a/) ⭐️ 9.0/10

Independent research reveals that coherent input text can shift an LLM's internal state into a different latent regime before the final output is generated. This shift allows the model to process information differently while still appearing to follow safety protocols on the surface. This finding suggests that current alignment techniques like RLHF, which primarily monitor final outputs, are insufficient because they fail to detect when a model's underlying reasoning process has been compromised. It highlights a critical vulnerability where safety filters can be bypassed by manipulating the model's internal state through context. The researcher utilized tools like Sparse Autoencoders (SAE) and residual stream trajectory analysis on the Gemma-3-12B-IT model to observe these shifts. The study demonstrates that dense, coherent discourse can change how a model interprets rules and constraints without requiring explicit jailbreak prompts.

reddit · r/MachineLearning · /u/PresentSituation8736 · Jun 14, 21:42

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks by analyzing their internal components, such as the residual stream, to understand how they process information. RLHF is a common alignment method used to train models to follow human preferences, but it is often criticized for being a surface-level patch that does not address the underlying latent representations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.neelnanda.io/mechanistic-interpretability/glossary">A Comprehensive Mechanistic Interpretability Explainer & Glossary — Neel Nanda</a></li>
<li><a href="https://medium.com/@zepingyu/123-cb62513f5d50">Exploring the Residual Stream of Transformers for Mechanistic Interpretability — Explained | by Zeping Yu | Medium</a></li>
<li><a href="https://apxml.com/courses/llm-alignment-safety/chapter-2-reinforcement-learning-human-feedback-rlhf/limitations-extensions-rlhf">Limitations and Extensions of RLHF</a></li>

</ul>
</details>

**Discussion**: The research has sparked significant interest within the machine learning community, with experts emphasizing the importance of mechanistic interpretability in identifying vulnerabilities that traditional safety filters miss. Many commenters are engaging with the researcher to provide technical feedback on the methodology and the implications for future AI safety research.

**Tags**: `#LLM Safety`, `#Mechanistic Interpretability`, `#AI Alignment`, `#Latent Space`, `#Machine Learning Research`

---

<a id="item-5"></a>
## [Rio de Janeiro's 'Homegrown' LLM Allegedly a Weighted Merge of Existing Models](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

Investigations suggest that the Rio-3.5-Open-397B model, presented as a novel fine-tune by the municipality of Rio de Janeiro, is actually a weighted merge of the Nex-N2 Pro and Qwen3.5-397B models. This finding challenges claims that the model was developed through independent training. This incident highlights critical issues regarding transparency, attribution, and provenance in the open-source AI community. It underscores the importance of verifying claims about model development to ensure ethical practices and proper credit for original contributors. Technical analysis indicates that the model's weight tensors are a consistent 0.6/0.4 blend of Nex and Qwen across all 60 layers. This mathematical interpolation suggests that no significant new training or distillation occurred, contradicting the 'homegrown' narrative.

hackernews · unrvl22 · Jun 14, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48528371)

**Background**: Model merging is a technique in the AI community that combines weights from multiple fine-tuned models to create a new, hybrid model without the need for additional training. Unlike fine-tuning, which involves updating model parameters on a specific dataset, merging mathematically blends existing knowledge. Provenance refers to the documented history and origin of a model, which is essential for establishing trust and accountability in AI development.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-model-merging-for-llms/">An Introduction to Model Merging for LLMs | NVIDIA Technical Blog</a></li>
<li><a href="https://huggingface.co/blog/mlabonne/merge-models">Merge Large Language Models with mergekit</a></li>
<li><a href="https://www.trantorinc.com/blog/digital-provenance-ai">Digital Provenance in AI : Verifying Origin, Integrity & Trust</a></li>

</ul>
</details>

**Discussion**: The community is debating the ethics of claiming credit for merged models, with many expressing skepticism about the transparency of the project. Some users noted that while the performance is robust, the lack of proper attribution to the original model creators is a significant ethical oversight.

**Tags**: `#LLM`, `#Model Merging`, `#AI Ethics`, `#Open Source`, `#Provenance`

---

<a id="item-6"></a>
## [Open-Source Knowledge Graph Pipeline Improves LLM Multi-Hop Reasoning](https://www.reddit.com/r/MachineLearning/comments/1u5yyyl/i_built_an_opensource_knowledge_graph_pipeline/) ⭐️ 8.0/10

The developer released an open-source full-stack pipeline that integrates knowledge graph construction, community detection, and hybrid retrieval to enhance LLM reasoning. It combines dense vector search, BM25, and graph traversal to overcome common RAG limitations. This project addresses the 'lost in the middle' and multi-hop reasoning failures in standard RAG systems, providing a practical solution for complex information retrieval tasks. It enables LLMs to synthesize answers from disconnected text chunks by mapping entity relationships. The pipeline uses spaCy for entity extraction, NetworkX for graph construction, and Reciprocal Rank Fusion (RRF) to merge results before final cross-encoder reranking. It effectively bridges gaps between text chunks by traversing 1st-degree neighbors in the graph.

reddit · r/MachineLearning · /u/Future_Caregiver_643 · Jun 14, 22:38

**Background**: Retrieval-Augmented Generation (RAG) is a technique that allows LLMs to access external data to improve accuracy. Standard RAG often struggles with multi-hop reasoning, where an answer requires connecting information across multiple documents. Knowledge graphs represent data as interconnected entities, helping systems understand relationships that vector search might miss.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval -augmented generation - Wikipedia</a></li>
<li><a href="https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.community.modularity_max.greedy_modularity_communities.html">greedy _ modularity _ communities — NetworkX 3.6.1 documentation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Okapi_BM25">Okapi BM25 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community responded positively, engaging in constructive technical discussions regarding the implementation details, potential edge cases in graph construction, and the efficiency of the hybrid retrieval approach.

**Tags**: `#RAG`, `#Knowledge Graphs`, `#LLM`, `#Information Retrieval`, `#Open Source`

---

<a id="item-7"></a>
## [The Verifier Tax: Horizon-Dependent Safety–Success Tradeoffs in Tool-Using LLM Agents](https://www.reddit.com/r/MachineLearning/comments/1u58mkq/the_verifier_tax_horizondependent_safetysuccess/) ⭐️ 8.0/10

Researchers introduced the 'Verifier Tax,' a phenomenon where increasing safety verification in LLM agents leads to a measurable decline in task completion rates as task horizons grow. They proposed a two-tier verification architecture using deterministic checks followed by LLM-based analysis to mitigate unsafe successes. This research highlights the critical tension between safety and utility in agentic AI, providing a formal framework for evaluating whether an agent's success is truly safe. It challenges developers to rethink how they measure performance beyond simple task completion metrics. The study utilizes the τ-bench framework to categorize outcomes into safe success, unsafe success, and failure. It demonstrates that while verification reduces unsafe actions, it imposes a 'tax' on overall task completion as the complexity and length of the task increase.

reddit · r/MachineLearning · /u/AccomplishedLeg1508 · Jun 14, 02:09

**Background**: LLM agents are AI systems designed to use external tools to perform multi-step tasks in real-world environments. Evaluating these agents is difficult because they may complete a task successfully while violating safety policies, a phenomenon known as 'unsafe success.' τ-bench is a benchmark designed to simulate complex, multi-turn interactions between users and agents in business domains.

<details><summary>References</summary>
<ul>
<li><a href="https://evalscope.readthedocs.io/en/latest/third_party/tau_bench.html">τ-bench - EvalScope - Read the Docs</a></li>
<li><a href="https://imerit.ai/solutions/generative-ai-data-solutions/agent-evaluation/">Agentic AI Evaluation: Reliable & Safe AI Agents | iMerit</a></li>

</ul>
</details>

**Discussion**: The community is actively debating how to classify 'unsafe success' in evaluation metrics, with some arguing it should be treated as a failure while others suggest it requires a distinct category to better understand agent behavior.

**Tags**: `#LLM Agents`, `#AI Safety`, `#Evaluation Metrics`, `#Tool Use`, `#Machine Learning Research`

---

<a id="item-8"></a>
## [Show HN: Kage – Shadow any website to a single binary for offline viewing](https://github.com/tamnd/kage) ⭐️ 7.0/10

Kage is a new command-line tool that captures website content and bundles it into a single executable binary, allowing users to view the site offline. It provides a unique approach to archiving by packaging the entire site structure into a standalone file. This tool offers a portable way to preserve web content, which is particularly useful for archiving documentation or wikis for access in environments without internet connectivity. It simplifies the distribution of archived web data by consolidating assets into a single binary. The tool currently requires a server-side process to view the archived content, which has led to user feedback requesting a more portable, browser-native solution. It is distinct from other archiving tools like SingleFile, which typically output a single HTML file.

hackernews · tamnd · Jun 14, 17:25 · [Discussion](https://news.ycombinator.com/item?id=48529990)

**Background**: Web archiving is the process of collecting portions of the World Wide Web to ensure the information is preserved for future researchers, historians, and the public. Common tools like SingleFile or HTTrack are frequently used to save web pages as static files or local mirrors. These tools help mitigate the risk of 'link rot' and ensure content remains accessible even if the original website goes offline.

**Discussion**: The community expressed interest in the project but questioned the necessity of a server-side component, suggesting that a static HTML output would be more convenient. Users also compared Kage to existing, more established tools like SingleFile and HTTrack, noting that those alternatives offer different trade-offs regarding portability and ease of use.

**Tags**: `#web-archiving`, `#cli-tools`, `#offline-access`, `#web-development`

---

<a id="item-9"></a>
## [Indexing 669 GB of GoPro footage using local ML on M1 Max](https://news.ycombinator.com/item?id=48528029) ⭐️ 7.0/10

A developer built a local machine learning pipeline to index over 600GB of cycling footage, enabling automated search and direct integration of highlights into DaVinci Resolve. The project processed 628 videos using an M1 Max computer to identify specific moments without relying on cloud services. This project demonstrates the growing accessibility of local AI for personal media management, allowing users to organize massive video libraries privately and efficiently. It highlights a trend where hobbyists can replicate professional-grade indexing workflows on consumer hardware. The pipeline analyzed 57,537 frames over approximately 67 hours of compute time to categorize scenes. While effective, the project highlights the trade-offs between local processing power and the time required for deep video analysis.

hackernews · iliashad · Jun 14, 15:13

**Background**: Local machine learning involves running AI models directly on a user's hardware rather than sending data to external cloud servers. This approach is increasingly popular for privacy-conscious users who want to manage large archives of personal media like GoPro footage or family photos. Modern Apple Silicon chips, such as the M1 Max, provide sufficient neural engine performance to handle these intensive tasks locally.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aitoolnet.com/edit-mind">Edit Mind - Local Video Indexer & AI Search - Aitoolnet</a></li>
<li><a href="https://www.livelink.ai/blog-posts/top-ai-tools-for-video-highlight-detection">Top 10 AI Tools for Video Highlight Detection in 2026</a></li>

</ul>
</details>

**Discussion**: The community discussed the project's practicality, noting that similar features are now appearing in professional software like DaVinci Resolve. Some users shared their own similar projects, while others debated the efficiency of processing large datasets locally versus using cloud-based alternatives.

**Tags**: `#machine-learning`, `#video-processing`, `#local-ai`, `#automation`, `#media-management`

---

<a id="item-10"></a>
## [Caddy compatibility for zeroserve: 3x throughput and 70% lower latency](https://su3.io/posts/zeroserve-caddy-compat) ⭐️ 7.0/10

The zeroserve web server has implemented Caddy-compatible configuration support, leveraging io_uring to achieve a 3x increase in throughput and a 70% reduction in latency. This update aims to bridge the gap between high-performance experimental servers and industry-standard configuration formats. This development highlights the potential of io_uring for extreme performance optimization in networking while demonstrating the ongoing challenge of balancing raw speed with the feature-rich ecosystems required for production environments. While the performance gains are significant, the current implementation lacks critical production features found in Caddy, such as automated ACME certificate management and plugin support. The server relies on io_uring, a Linux kernel interface that reduces syscall overhead by allowing asynchronous I/O operations.

hackernews · losfair · Jun 14, 13:43 · [Discussion](https://news.ycombinator.com/item?id=48527145)

**Background**: io_uring is a Linux kernel interface introduced in 2019 that allows for high-performance asynchronous I/O by reducing the overhead associated with traditional system calls. Zeroserve is a specialized, high-performance web server designed for zero-config deployments, often utilizing eBPF for efficient request handling. Caddy is a popular, enterprise-ready web server known for its ease of use and automatic HTTPS management via ACME.

<details><summary>References</summary>
<ul>
<li><a href="https://su3.io/posts/introducing-zeroserve">zeroserve : a zero -config web server you can script with eBPF</a></li>

</ul>
</details>

**Discussion**: The community expressed skepticism regarding the lack of essential features like ACME and plugins, with many arguing that performance alone does not justify replacing established servers like Nginx. Some users also raised security concerns regarding the use of io_uring in web server development.

**Tags**: `#web-servers`, `#io_uring`, `#performance-engineering`, `#networking`, `#caddy`

---

<a id="item-11"></a>
## [Mapping SQLite result columns back to their source table and column](https://simonwillison.net/2026/Jun/13/sqlite-column-provenance/#atom-everything) ⭐️ 7.0/10

Simon Willison is researching programmatic methods to identify the original table and column for each field in an arbitrary SQLite query result. This approach aims to improve data provenance in tools like Datasette by handling complex SQL syntax including joins and Common Table Expressions (CTEs). Accurate data provenance is essential for building intuitive database interfaces that allow users to understand exactly where their data originates. This research helps bridge the gap between raw SQL output and meaningful metadata, which is particularly useful for data exploration tools. The research explores three main techniques: using the APSW library, accessing the C-level sqlite3_column_table_name() function via Python's ctypes, and parsing the output of the EXPLAIN command. These methods are necessary because standard Python SQLite interfaces often do not expose column provenance metadata by default.

rss · Simon Willison · Jun 13, 23:05

**Background**: SQLite is a lightweight, file-based database engine that is widely used for local storage and data analysis tools. Common Table Expressions (CTEs) are temporary result sets that simplify complex queries by allowing developers to define virtual tables within a single SQL statement. Data provenance refers to the documentation of the origin and processing history of data, which is critical for debugging and data integrity.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/sql/t-sql/queries/with-common-table-expression-transact-sql?view=sql-server-ver17">WITH common _ table _ expression (Transact- SQL )... | Microsoft Learn</a></li>
<li><a href="https://www.codestudy.net/blog/is-there-an-sqlite-equivalent-to-mysql-s-describe-table/">Is There an SQLite Equivalent to... — codestudy.net</a></li>

</ul>
</details>

**Tags**: `#SQLite`, `#SQL`, `#Data Provenance`, `#Datasette`, `#Database Engineering`

---

<a id="item-12"></a>
## [OpenAI WebRTC Audio Session Playground Adds GPT-Realtime-2 and Document Context](https://simonwillison.net/2026/Jun/12/openai-webrtc/#atom-everything) ⭐️ 7.0/10

Simon Willison has updated his OpenAI WebRTC playground to support the GPT-Realtime-2 model and added a feature allowing users to paste document context for voice-based conversations. This enables users to discuss specific text content directly with the AI in real-time. This update provides developers with a practical way to test the advanced reasoning capabilities of GPT-Realtime-2 and experiment with context-aware voice interactions. It bridges the gap for those waiting for these features to appear in consumer-facing applications. The playground now includes a dedicated text area for document context, which the model uses to inform its responses during the WebRTC session. GPT-Realtime-2 is noted for bringing GPT-5-class reasoning to voice experiences with a knowledge cut-off of September 30, 2024.

rss · Simon Willison · Jun 12, 23:53

**Background**: WebRTC is a technology that enables real-time communication directly between browsers, which OpenAI utilizes for its low-latency voice API. GPT-Realtime-2 is a specialized model released by OpenAI to provide smarter, more responsive voice interactions compared to previous iterations. These tools are primarily aimed at developers building voice-enabled applications via the OpenAI API.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.openai.com/api/docs/guides/realtime-webrtc">Realtime API with WebRTC | OpenAI API</a></li>
<li><a href="https://www.linkedin.com/posts/openai-for-business_advancing-voice-intelligence-with-new-models-activity-7458206167966703616-5G4N">Introducing GPT - Realtime - 2 for Voice Experiences | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#WebRTC`, `#Voice AI`, `#LLM`, `#Developer Tools`

---

<a id="item-13"></a>
## [Derivative-Free Neural Network Optimization Achieves Competitive Results on MNIST](https://www.reddit.com/r/MachineLearning/comments/1u4fc16/derivativefree_neural_network_optimization_mnist/) ⭐️ 7.0/10

A derivative-free optimization method called MDP successfully trained a neural network on the MNIST dataset, outperforming the standard Adam optimizer in a 25,450-dimensional parameter space. The model achieved a test accuracy of 93.4% compared to Adam's 91.7% using the same architecture. This result challenges the reliance on gradient-based backpropagation, which is the industry standard for deep learning. Demonstrating that derivative-free methods can scale to high-dimensional spaces opens new possibilities for training models where gradients are unavailable or computationally expensive. The experiment utilized a 784-32-10 network architecture and reached convergence after 1,000,000 function evaluations without using population-based methods. The implementation is publicly available in the sgo-lab repository.

reddit · r/MachineLearning · /u/Mis4318 · Jun 13, 02:51

**Background**: Most deep learning models are trained using gradient descent, which calculates the slope of the loss function to update weights. Derivative-free optimization is an alternative approach that searches for optimal parameters by evaluating the function directly without calculating gradients. This is often used in black-box scenarios where the internal structure of the model is unknown or gradients are difficult to compute.

<details><summary>References</summary>
<ul>
<li><a href="https://optimization-online.org/wp-content/uploads/2026/01/Riemannian_optimization_with_finite-difference_gradient.pdf">Riemannian optimization with finite-difference gradient</a></li>
<li><a href="https://ora.ox.ac.uk/objects/uuid:c54b7c60-4d37-464e-a549-cab897ed9b90/files/dm613mz05z">Studies on Neural Networks</a></li>

</ul>
</details>

**Discussion**: The community is actively discussing the scalability of this approach, with some users expressing skepticism about how it will perform on deeper, more complex architectures compared to standard gradient-based methods.

**Tags**: `#Machine Learning`, `#Optimization`, `#Neural Networks`, `#Derivative-Free Optimization`, `#MNIST`

---

<a id="item-14"></a>
## [Simon Willison releases luau-wasm 0.1a0 for Pyodide](https://simonwillison.net/2026/Jun/13/luau-wasm/#atom-everything) ⭐️ 6.0/10

Simon Willison has released luau-wasm 0.1a0, a package that enables the use of the Luau scripting language within Pyodide environments. This release utilizes WebAssembly wheels to allow Python developers to integrate Luau directly in the browser. This tool simplifies the integration of high-performance scripting languages into browser-based Python applications. It expands the utility of Pyodide by allowing developers to leverage Luau's fast execution capabilities within a web context. The package is distributed as a WebAssembly wheel, making it compatible with Pyodide's package management system. It is currently in an alpha stage (0.1a0), indicating that it is an early release for testing and experimentation.

rss · Simon Willison · Jun 13, 23:14

**Background**: Luau is a fast, embeddable scripting language derived from Lua 5.1, originally developed by Roblox for their platform. Pyodide is a port of CPython to WebAssembly, which allows Python code to run directly in web browsers without needing a server-side backend.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Luau_(programming_language)">Luau ( programming language ) - Wikipedia</a></li>
<li><a href="https://github.com/pyodide/pyodide">GitHub - pyodide / pyodide : Pyodide is a Python distribution for the...</a></li>

</ul>
</details>

**Tags**: `#lua`, `#webassembly`, `#pyodide`, `#python`

---

<a id="item-15"></a>
## [Developer Launches Free Bilingual Machine Learning Notebook Course](https://www.reddit.com/r/MachineLearning/comments/1u4zbld/im_building_a_free_bilingual_machinelearning/) ⭐️ 6.0/10

A developer has released an open-source, bilingual machine learning tutorial repository in Jupyter Notebook format that provides parallel content in English and Persian. The curriculum covers essential topics ranging from data preprocessing and feature engineering to MLOps and time series analysis. This project increases accessibility to machine learning education for non-native English speakers by providing hands-on, localized resources. It serves as a practical, community-driven alternative to traditional, English-only academic materials. The course is designed for local execution in Jupyter Notebooks, focusing on a step-by-step workflow that includes datasets and exercises. The author is currently seeking community feedback on the curriculum structure and methods to enhance practical learning beyond simple code copying.

reddit · r/MachineLearning · /u/abolfazl1363 · Jun 13, 19:07

**Background**: Jupyter Notebooks are widely used in data science to combine live code, equations, and narrative text into a single document. Feature engineering is the process of transforming raw data into meaningful inputs to improve model performance, while MLOps focuses on the operational practices required to deploy and maintain machine learning models in production environments.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Feature_engineering">Feature engineering</a></li>
<li><a href="https://ml-ops.org/content/mlops-principles">MLOps Principles</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dimensionality_reduction">Dimensionality reduction</a></li>

</ul>
</details>

**Discussion**: The community has shown interest in the project, with discussions focusing on the pedagogical value of bilingual resources and suggestions for improving the practical exercises to ensure students gain a deeper understanding of the concepts.

**Tags**: `#machine-learning`, `#education`, `#jupyter-notebooks`, `#open-source`, `#data-science`

---