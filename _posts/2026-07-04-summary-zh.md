---
layout: default
title: "Horizon Summary: 2026-07-04 (ZH)"
date: 2026-07-04
lang: zh
---

> 从 26 条内容中筛选出 13 条重要资讯。

---

1. [Leaking YouTube creators' private videos](#item-1) ⭐️ 9.0/10
2. [Contrastive Decoding Diffing (CDD): recovering verbatim finetuning data from logits alone, no weight access needed(R)](#item-2) ⭐️ 9.0/10
3. [Báo cáo về khả năng rò rỉ phiên làm việc hoặc bộ nhớ đệm trong Claude Code](#item-3) ⭐️ 8.0/10
4. [Các nhà vật lý thiên văn đau đầu trước những 'chấm đỏ nhỏ' bí ẩn từ kính thiên văn Webb](#item-4) ⭐️ 8.0/10
5. [Các mô hình Anthropic mới hơn cho thấy sự suy giảm về độ tin cậy khi sử dụng công cụ](#item-5) ⭐️ 8.0/10
6. [Current AI ra mắt Bản đồ khoảng trống AI mã nguồn mở](#item-6) ⭐️ 8.0/10
7. [Cải thiện hiệu suất của tác nhân lập trình AI thông qua khả năng tự đánh giá](#item-7) ⭐️ 8.0/10
8. [Phương pháp USAF cho phép tinh chỉnh thưa các mô hình MoE hiệu quả trên GPU phổ thông](#item-8) ⭐️ 8.0/10
9. [BaryGraph: Kiến trúc đồ thị tri thức coi các mối quan hệ là tài liệu nhúng hạng nhất](#item-9) ⭐️ 8.0/10
10. [Command and Conquer: Generals được chuyển đổi gốc sang macOS, iPhone và iPad](#item-10) ⭐️ 7.0/10
11. [Google Books (or similar) all book scans – $200k bounty (2025)](#item-11) ⭐️ 7.0/10
12. [Hướng dẫn toàn diện về cách hiểu các chỉ số giám sát hệ thống Linux](#item-12) ⭐️ 7.0/10
13. [Nhà sáng tạo khóa học độc lập báo cáo doanh thu sụt giảm đáng kể do AI](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Leaking YouTube creators' private videos](https://javoriuski.com/post/youtube) ⭐️ 9.0/10

A security researcher details a vulnerability that allowed attackers to leak private YouTube video metadata, sparking a deep discussion on platform security and corporate engineering culture.

hackernews · javxfps · 7月4日 16:45 · [社区讨论](https://news.ycombinator.com/item?id=48786781)

**标签**: `#security`, `#vulnerability`, `#youtube`, `#web-privacy`, `#infosec`

---

<a id="item-2"></a>
## [Contrastive Decoding Diffing (CDD): recovering verbatim finetuning data from logits alone, no weight access needed(R)](https://www.reddit.com/r/MachineLearning/comments/1umn2dk/contrastive_decoding_diffing_cdd_recovering/) ⭐️ 9.0/10

Contrastive Decoding Diffing (CDD) is a novel grey-box attack that enables the verbatim recovery of finetuning data from LLMs by contrasting base and finetuned model logits.

reddit · r/MachineLearning · /u/CebulkaZapiekana · 7月3日 19:01

**标签**: `#LLM Security`, `#Data Privacy`, `#Machine Learning Research`, `#Model Extraction`, `#Contrastive Decoding`

---

<a id="item-3"></a>
## [Báo cáo về khả năng rò rỉ phiên làm việc hoặc bộ nhớ đệm trong Claude Code](https://github.com/anthropics/claude-code/issues/74066) ⭐️ 8.0/10

Một báo cáo trên GitHub đã nêu lên lo ngại về khả năng rò rỉ dữ liệu giữa các phiên làm việc khác nhau của Claude Code. Đội ngũ phát triển Claude Code hiện đang điều tra báo cáo này và cho rằng đây có khả năng là một hiện tượng ảo giác của mô hình thay vì lỗi bảo mật hệ thống. Sự việc này làm nổi bật thách thức quan trọng trong việc đảm bảo sự cô lập giữa các người dùng trong hạ tầng AI, nơi người dùng thường khó phân biệt giữa vi phạm bảo mật thực sự và ảo giác của mô hình. Điều này nhấn mạnh tầm quan trọng của việc kiểm định bảo mật nghiêm ngặt đối với các công cụ AI tác nhân xử lý dữ liệu mã nguồn nhạy cảm. Báo cáo cho thấy các ảo giác do ngữ cảnh gây ra, đặc biệt khi xử lý các tập dữ liệu đầu vào lớn hoặc các tệp tin từ phiên làm việc trước, có thể khiến mô hình tạo ra thông tin nghe có vẻ hợp lý nhưng không chính xác. Các nhà quan sát kỹ thuật lưu ý rằng mặc dù rò rỉ ở cấp độ hạ tầng là hiếm gặp, đây vẫn là mối quan tâm lớn đối với các nền tảng LLM đa người dùng.

hackernews · chatmasta · 7月4日 14:03 · [社区讨论](https://news.ycombinator.com/item?id=48785485)

**背景**: Claude Code là một công cụ lập trình tác nhân được thiết kế để tương tác với cơ sở mã nguồn cục bộ, quản lý tác vụ và thực thi lệnh trong môi trường của nhà phát triển. Ảo giác LLM xảy ra khi các mô hình tạo ra kết quả tự tin nhưng sai lệch về thực tế hoặc không liên quan, thường do các câu lệnh mơ hồ hoặc ngữ cảnh quá tải. Kiến trúc đa người dùng (multi-tenancy) trong AI đề cập đến việc một phiên bản phần mềm phục vụ nhiều người dùng, đòi hỏi sự cô lập nghiêm ngặt để ngăn chặn rò rỉ dữ liệu giữa họ.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.claude.com/">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://tianpan.co/blog/2026-04-17-multi-tenant-llm-noisy-neighbor-isolation">The Multi - Tenant LLM Problem: Noisy Neighbors, Isolation, and...</a></li>

</ul>
</details>

**社区讨论**: Cộng đồng đang chia rẽ, với một số người dùng báo cáo trải nghiệm tương tự về các phản hồi bị 'tráo đổi' trong các dịch vụ LLM khác, trong khi những người khác cho rằng đây là các ảo giác điển hình do cửa sổ ngữ cảnh lớn gây ra. Các nhà phát triển từ đội ngũ Claude Code đã tích cực tham gia, yêu cầu bằng chứng trong khi vẫn khẳng định rằng báo cáo hiện tại có vẻ là một ảo giác.

**标签**: `#LLM Security`, `#Data Privacy`, `#Claude Code`, `#Infrastructure`, `#AI Safety`

---

<a id="item-4"></a>
## [Các nhà vật lý thiên văn đau đầu trước những 'chấm đỏ nhỏ' bí ẩn từ kính thiên văn Webb](https://www.quantamagazine.org/astrophysicists-puzzle-over-webbs-new-universe-20260702/) ⭐️ 8.0/10

Các nhà vật lý thiên văn đang nghiên cứu một loại thiên thể mới được gọi là 'chấm đỏ nhỏ' do kính thiên văn James Webb phát hiện. Những vật thể nhỏ gọn, có màu đỏ này dường như đang thách thức các mô hình hiện tại về cách các thiên hà hình thành trong vũ trụ sơ khai. Những vật thể này cho thấy quá trình hình thành thiên hà sơ khai có thể đã diễn ra nhanh hơn hoặc khác biệt so với suy nghĩ trước đây. Việc hiểu rõ chúng có thể buộc chúng ta phải sửa đổi đáng kể các mô hình vũ trụ học hiện tại, bao gồm cả lý thuyết Lambda-CDM tiêu chuẩn. Các bằng chứng gần đây cho thấy những chấm đỏ này có thể là các lỗ đen được bao bọc trong lớp khí dày, có khả năng đại diện cho một loại vật thể mới gọi là 'sao lỗ đen'. Các nhà nghiên cứu đang cẩn thận lọc bỏ dữ liệu nhiễu từ các sao lùn nâu gần đó để đảm bảo tính chính xác của các quan sát này.

hackernews · jnord · 7月4日 09:08 · [社区讨论](https://news.ycombinator.com/item?id=48783948)

**背景**: Mô hình Lambda-CDM là khung lý thuyết tiêu chuẩn trong vũ trụ học, mô tả một vũ trụ nơi các thiên hà phát triển dần dần thông qua việc sáp nhập các cấu trúc nhỏ hơn trong hàng tỷ năm. Kính thiên văn James Webb (JWST) gần đây đã thách thức điều này bằng cách quan sát các thiên hà trưởng thành và sáng một cách đáng ngạc nhiên tồn tại ngay sau vụ nổ Big Bang. Những 'chấm đỏ nhỏ' này là các vật thể nhỏ gọn, có độ dịch chuyển đỏ cao, không hoàn toàn khớp với các phân loại truyền thống về sao hoặc thiên hà.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Little_red_dot_(astronomical_object)">Little red dot (astronomical object) - Wikipedia</a></li>
<li><a href="https://www.space.com/astronomy/black-holes/james-webb-space-telescope-finds-evidence-the-mysterious-little-red-dots-are-black-hole-stars">James Webb Space Telescope finds evidence the mysterious 'little red dots' are black hole stars | Space</a></li>
<li><a href="https://arxiv.org/html/2412.03534v1">Galaxy Formation in the Early Universe - arXiv.org</a></li>

</ul>
</details>

**社区讨论**: Cộng đồng đang tranh luận sôi nổi về bản chất của các vật thể này, với một số người dùng lưu ý rằng các nhà nghiên cứu đã tính đến khả năng nhiễu từ các sao lùn nâu. Những người khác tỏ ra thích thú với giả thuyết rằng các chấm đỏ này có thể là 'sao lỗ đen', nơi áp suất khí mô phỏng hoạt động của các ngôi sao.

**标签**: `#astrophysics`, `#JWST`, `#cosmology`, `#space-science`, `#scientific-research`

---

<a id="item-5"></a>
## [Các mô hình Anthropic mới hơn cho thấy sự suy giảm về độ tin cậy khi sử dụng công cụ](https://simonwillison.net/2026/Jul/4/better-models-worse-tools/#atom-everything) ⭐️ 8.0/10

Armin Ronacher báo cáo rằng các mô hình Anthropic mới hơn như Opus 4.8 và Sonnet 5 ngày càng không tuân thủ nghiêm ngặt các lược đồ sử dụng công cụ bằng cách tự ý thêm các trường không cần thiết. Hành vi này khiến các công cụ lập trình tùy chỉnh như Pi từ chối các lệnh gọi công cụ mà lẽ ra các mô hình cũ hơn có thể xử lý chính xác. Sự suy giảm này làm phức tạp hóa việc phát triển các tác nhân AI đáng tin cậy, vì các nhà phát triển không còn có thể mặc định rằng các mô hình mới hơn, mạnh mẽ hơn sẽ duy trì sự tuân thủ nghiêm ngặt đối với các lược đồ công cụ tùy chỉnh. Điều này làm nổi bật một sự đánh đổi tiềm ẩn khi các mô hình được tối ưu hóa cho các công cụ nội bộ cụ thể có thể trở nên kém linh hoạt hơn đối với các tích hợp của bên thứ ba. Vấn đề dường như bắt nguồn từ quá trình đào tạo học tăng cường (Reinforcement Learning) khiến các mô hình bị thiên lệch đối với các công cụ chỉnh sửa cụ thể được sử dụng trong Claude Code. Do đó, các nhà phát triển bên thứ ba có thể cần phải triển khai nhiều biến thể công cụ để đáp ứng các đặc điểm hành vi riêng biệt của các phiên bản mô hình khác nhau.

rss · Simon Willison · 7月4日 22:53

**背景**: Các mô hình ngôn ngữ lớn (LLM) sử dụng tính năng 'gọi công cụ' hoặc 'gọi hàm' để tương tác với phần mềm bên ngoài bằng cách xuất dữ liệu có cấu trúc, thường là JSON, khớp với một lược đồ đã xác định trước. Khi một mô hình không tuân thủ lược đồ này—bằng cách thêm các trường thừa hoặc sử dụng sai kiểu dữ liệu—phần mềm nhận sẽ không thể thực thi tác vụ được yêu cầu, dẫn đến lỗi cho tác nhân AI.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aivineet.com/tool-calling-reliability-llm-agents-schemas-validation-retries/">Tool calling reliability : schemas, validation, retries</a></li>

</ul>
</details>

**标签**: `#LLM`, `#AI Agents`, `#Tool Use`, `#Software Engineering`, `#Anthropic`

---

<a id="item-6"></a>
## [Current AI ra mắt Bản đồ khoảng trống AI mã nguồn mở](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

Current AI đã phát hành Gap Map v0.1, một chỉ mục toàn diện phân loại 421 sản phẩm AI mã nguồn mở quan trọng, bao gồm các mô hình, công cụ và tập dữ liệu, trên 14 danh mục khác nhau. Dự án cũng cung cấp quyền truy cập mở vào dữ liệu cơ bản thông qua GitHub, bao gồm hàng nghìn tệp YAML và các tập lệnh nghiên cứu. Chỉ mục này cung cấp một cái nhìn tổng quan có cấu trúc rất cần thiết về hệ sinh thái AI mã nguồn mở vốn đang bị phân mảnh mạnh mẽ, giúp các nhà nghiên cứu và nhà phát triển điều hướng hệ sinh thái hiệu quả hơn. Bằng cách chuẩn hóa cách theo dõi các công cụ này, dự án thúc đẩy sự minh bạch và hợp tác tốt hơn trong cộng đồng AI toàn cầu. Phiên bản v0.1 bao gồm 266 công cụ phần mềm, 85 mô hình, 50 tập dữ liệu và 20 dự án phần cứng từ 228 tổ chức. Dữ liệu được cấp phép theo giấy phép MIT và có thể được khám phá bằng các công cụ như Datasette Lite để phân tích sâu hơn về các kho lưu trữ được theo dõi.

rss · Simon Willison · 7月3日 22:04

**背景**: Hệ sinh thái AI mã nguồn mở bao gồm một loạt các mô hình, khung làm việc và tập dữ liệu cho phép các nhà phát triển xây dựng ứng dụng AI mà không cần dựa hoàn toàn vào các mô hình độc quyền, đóng kín. Khi số lượng các thành phần này tăng lên nhanh chóng, việc lập chỉ mục chúng trở nên cần thiết để xác định các khoảng trống công nghệ và đảm bảo nguồn lực được cộng đồng sử dụng hiệu quả.

**社区讨论**: Cộng đồng đã bày tỏ sự hào hứng về tính sẵn có của dữ liệu cơ bản, đặc biệt là khả năng sử dụng các công cụ như Datasette để truy vấn và khám phá danh sách khổng lồ các kho lưu trữ được theo dõi.

**标签**: `#AI`, `#Open Source`, `#Data Indexing`, `#Ecosystem Analysis`

---

<a id="item-7"></a>
## [Cải thiện hiệu suất của tác nhân lập trình AI thông qua khả năng tự đánh giá](https://simonwillison.net/2026/Jul/3/judgement/#atom-everything) ⭐️ 8.0/10

Simon Willison nhấn mạnh chiến lược trao quyền cho các tác nhân lập trình AI như Fable để chúng tự đưa ra quyết định về việc kiểm thử và lựa chọn mô hình thay vì tuân theo các chỉ dẫn cứng nhắc. Bằng cách ủy quyền các tác vụ cho các mô hình nhỏ hơn, hiệu suất thấp hơn thông qua các tác nhân phụ, người dùng có thể cải thiện đáng kể hiệu quả chi phí. Sự chuyển dịch sang quyền tự chủ dựa trên mô hình cho phép các nhà phát triển tối ưu hóa việc sử dụng token và duy trì năng suất cao mà không làm giảm chất lượng. Điều này đại diện cho một xu hướng rộng lớn hơn trong ngành, nơi các tác nhân đóng vai trò là những người điều phối thông minh thay vì chỉ là các công cụ dòng lệnh đơn giản. Người dùng có thể triển khai phương pháp này bằng cách thêm tệp bộ nhớ vào dự án của họ để hướng dẫn tác nhân tạo ra các tác nhân phụ với các mô hình thay thế, chẳng hạn như sử dụng Sonnet cho việc triển khai phức tạp và Haiku cho các chỉnh sửa đơn giản. Cách tiếp cận này giữ cho khả năng đánh giá và tổng hợp cấp cao nằm trong vòng lặp của tác nhân chính.

rss · Simon Willison · 7月3日 18:51

**背景**: Claude Code là một công cụ tác nhân của Anthropic hoạt động trong thiết bị đầu cuối để hiểu cơ sở mã và thực hiện các tác vụ phát triển. Fable là một tác nhân lập trình AI tiên tiến được thiết kế cho các tác vụ dài hạn, có khả năng quản lý các vòng đời phần mềm phức tạp với quyền tự chủ cao hơn.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.anthropic.com/en/docs/agents-and-tools/claude-code/overview">Claude Code overview - Anthropic</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#Prompt Engineering`, `#Claude Code`, `#Software Development`, `#LLMs`

---

<a id="item-8"></a>
## [Phương pháp USAF cho phép tinh chỉnh thưa các mô hình MoE hiệu quả trên GPU phổ thông](https://www.reddit.com/r/MachineLearning/comments/1unl62q/if_your_gpu_can_run_inference_it_should_be_able/) ⭐️ 8.0/10

Phương pháp USAF cho phép người dùng tinh chỉnh các mô hình Mixture-of-Experts (MoE) trên phần cứng phổ thông bằng cách chỉ huấn luyện các trọng số chuyên gia và bộ định tuyến. Cách tiếp cận này loại bỏ nhu cầu sử dụng thêm các adapter, giúp thực hiện các tác vụ như tinh chỉnh mô hình Qwen3-30B-A3B trên GPU 12GB. Đột phá này làm giảm đáng kể rào cản phần cứng khi tinh chỉnh các mô hình MoE lớn, giúp việc tùy chỉnh AI nâng cao trở nên dễ tiếp cận hơn đối với các nhà phát triển cá nhân và nhà nghiên cứu có nguồn lực hạn chế. Nó phổ cập hóa khả năng thích ứng các mô hình mạnh mẽ mà không cần đến các cụm máy tính cấp doanh nghiệp. Dự án được phát hành mã nguồn mở theo giấy phép Apache 2.0 và tập trung vào việc tinh chỉnh thưa bằng cách cập nhật các trọng số chuyên gia cụ thể thay vì toàn bộ tham số mô hình. Nó được thiết kế đặc biệt để hoạt động trên phần cứng vốn đã có khả năng chạy suy luận cho các mô hình lớn này.

reddit · r/MachineLearning · /u/tsuyu122 · 7月4日 21:56

**背景**: Các mô hình Mixture-of-Experts (MoE) là kiến trúc mạng thần kinh sử dụng nhiều mạng con chuyên biệt, hay còn gọi là 'chuyên gia', để xử lý dữ liệu, với một mạng định tuyến quyết định chuyên gia nào sẽ được kích hoạt cho một đầu vào nhất định. Tinh chỉnh thưa là kỹ thuật chỉ cập nhật một tập hợp con các tham số của mô hình, giúp tiết kiệm tài nguyên tính toán hơn so với tinh chỉnh toàn bộ. Điều này cho phép người dùng thích ứng các mô hình lớn với các tác vụ cụ thể mà không cần bộ nhớ và sức mạnh tính toán khổng lồ thường thấy khi cập nhật toàn bộ tham số.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.baeldung.com/cs/mixture-of-experts">The Mixture-of-Experts ML Approach - Baeldung</a></li>
<li><a href="https://www.ibm.com/think/topics/fine-tuning">What is Fine-Tuning? | IBM</a></li>

</ul>
</details>

**社区讨论**: Cộng đồng đã phản hồi tích cực, ca ngợi tính khả thi về mặt kỹ thuật của phương pháp này và tiềm năng phổ cập hóa việc huấn luyện mô hình. Các cuộc thảo luận nhấn mạnh sự quan tâm đến việc cách tiếp cận này có thể được áp dụng cho các kiến trúc MoE khác như thế nào.

**标签**: `#Machine Learning`, `#LLM`, `#MoE`, `#Fine-tuning`, `#Open Source`

---

<a id="item-9"></a>
## [BaryGraph: Kiến trúc đồ thị tri thức coi các mối quan hệ là tài liệu nhúng hạng nhất](https://www.reddit.com/r/MachineLearning/comments/1un3lsf/barygraph_knowledge_graph_where_every/) ⭐️ 8.0/10

BaryGraph giới thiệu một kiến trúc mới, trong đó các mối quan hệ, được gọi là 'BaryEdge', được coi là các tài liệu nhúng độc lập thay vì chỉ là siêu dữ liệu. Bằng cách xếp chồng đệ quy các cạnh này thành các bộ ba 'MetaBary', hệ thống làm nổi bật các kết nối cấu trúc giữa các khái niệm vốn nằm xa nhau trong không gian vectơ tiêu chuẩn. Cách tiếp cận này khắc phục hạn chế lớn của các hệ thống RAG tiêu chuẩn, vốn thường không nắm bắt được các mối quan hệ cấu trúc liên miền không rõ ràng. Nó cho phép truy xuất ngữ nghĩa sâu hơn bằng cách xác định các mô hình mà tìm kiếm vectơ dựa trên độ tương đồng cosine truyền thống không thể phát hiện. Hệ thống sử dụng MongoDB với tìm kiếm vectơ và nomic-embed-text để xử lý 6,6 triệu tài liệu, đạt được các chỉ số tương quan cấu trúc cao hơn đáng kể so với độ tương đồng cosine thô. Nó cũng bao gồm một máy chủ MCP để cho phép các trợ lý AI truy vấn trực tiếp đồ thị.

reddit · r/MachineLearning · /u/adseipsum · 7月4日 08:24

**背景**: Đồ thị tri thức là các cấu trúc biểu diễn thông tin dưới dạng mạng lưới các nút và cạnh, trong đó các nút đại diện cho thực thể và các cạnh đại diện cho mối quan hệ. RAG (Truy xuất tăng cường thế hệ) tiêu chuẩn thường dựa trên các nhúng vectơ phẳng, ánh xạ văn bản thành các điểm trong không gian; tuy nhiên, phương pháp này gặp khó khăn trong việc xác định các kết nối logic phức tạp, đa bước giữa các chủ đề khác biệt. Model Context Protocol (MCP) là một tiêu chuẩn mở cho phép các mô hình AI tương tác an toàn với các nguồn dữ liệu và công cụ bên ngoài.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://modelcontextprotocol.io/examples">Example Servers - Model Context Protocol</a></li>

</ul>
</details>

**社区讨论**: Cộng đồng đã thể hiện sự quan tâm đáng kể đến tính mới về kiến trúc khi coi các mối quan hệ là các tài liệu có thể truy xuất. Các cuộc thảo luận tập trung vào việc triển khai kỹ thuật các bộ ba MetaBary và tiềm năng của phương pháp này trong việc tăng cường khả năng suy luận liên miền trong các ứng dụng AI.

**标签**: `#Knowledge Graphs`, `#RAG`, `#Vector Databases`, `#Embeddings`, `#Information Retrieval`

---

<a id="item-10"></a>
## [Command and Conquer: Generals được chuyển đổi gốc sang macOS, iPhone và iPad](https://github.com/ammaarreshi/Generals-Mac-iOS-iPad/tree/main) ⭐️ 7.0/10

Một dự án cộng đồng đã chuyển đổi thành công trò chơi chiến thuật thời gian thực kinh điển Command and Conquer: Generals sang các nền tảng của Apple bằng cách tận dụng công cụ chuyển đổi mã hỗ trợ bởi AI và các nhánh mã nguồn mở hiện có. Việc triển khai này cho phép chơi game gốc trên các thiết bị macOS, iPhone và iPad. Dự án này làm nổi bật tiềm năng ngày càng lớn của các công cụ hỗ trợ bởi AI trong việc hiện đại hóa phần mềm và công cụ trò chơi cũ cho phần cứng đương đại. Nó cho thấy cách các nhà phát triển có thể thu hẹp khoảng cách giữa các tựa game kinh điển và hệ sinh thái di động hiện đại với hiệu suất cao hơn. Bản chuyển đổi được xây dựng dựa trên nhánh fbraz3/GeneralsX, vốn tận dụng bản phát hành mã nguồn GPL v3 của EA, đồng thời bổ sung các bản sửa lỗi công cụ và tối ưu hóa đầu vào cho giao diện cảm ứng. Người dùng bắt buộc phải sở hữu trò chơi trên Steam để cài đặt và chạy ứng dụng thành công.

hackernews · asronline · 7月4日 19:41 · [社区讨论](https://news.ycombinator.com/item?id=48788283)

**背景**: Command and Conquer: Generals là một trò chơi chiến thuật thời gian thực 3D phổ biến được EA phát hành lần đầu vào năm 2003. Việc chuyển đổi các trò chơi cũ sang các nền tảng hiện đại như iOS thường đòi hỏi những thay đổi đáng kể để xử lý các phương thức nhập liệu khác nhau, chẳng hạn như điều khiển cảm ứng và sự khác biệt về kiến trúc giữa bộ vi xử lý x86 và ARM.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/videos/play/wwdc2026/357/">Speedrun your game port with agentic coding - WWDC26 - Videos ...</a></li>

</ul>
</details>

**社区讨论**: Các thành viên cộng đồng ca ngợi dự án là một ứng dụng thực tế của AI trong lập trình, mặc dù một số người lưu ý rằng tài liệu do AI tạo ra có thể mang lại cảm giác thiếu tự nhiên. Những người khác thảo luận về khả năng áp dụng các kỹ thuật chuyển đổi này cho các tựa game kinh điển khác như Emperor: Battle for Dune và nhận xét về sự xuất hiện của các thuật ngữ lạ do AI tạo ra trong văn bản kỹ thuật.

**标签**: `#Game Development`, `#Retro Gaming`, `#AI-Assisted Coding`, `#macOS`, `#iOS`

---

<a id="item-11"></a>
## [Google Books (or similar) all book scans – $200k bounty (2025)](https://software.annas-archive.gl/AnnaArchivist/annas-archive/-/work_items/234) ⭐️ 7.0/10

Anna's Archive has initiated a $200,000 bounty to incentivize the digitization and preservation of rare and hard-to-find book collections.

hackernews · Cider9986 · 7月4日 16:51 · [社区讨论](https://news.ycombinator.com/item?id=48786838)

**标签**: `#digital-archiving`, `#open-access`, `#information-preservation`, `#data-curation`

---

<a id="item-12"></a>
## [Hướng dẫn toàn diện về cách hiểu các chỉ số giám sát hệ thống Linux](https://peteris.rocks/blog/htop/) ⭐️ 7.0/10

Hướng dẫn này cung cấp phân tích chi tiết về các chỉ số hiển thị trong các công cụ giám sát Linux như top và htop, giải thích cách diễn giải dữ liệu CPU, bộ nhớ và tiến trình. Tài liệu này làm rõ những điểm gây nhầm lẫn phổ biến liên quan đến các chỉ số hiệu suất hệ thống. Việc hiểu các chỉ số này là rất cần thiết để các quản trị viên hệ thống và lập trình viên chẩn đoán chính xác các điểm nghẽn hiệu suất và quản lý việc phân bổ tài nguyên. Điều này giúp người dùng tránh hiểu sai dữ liệu, chẳng hạn như nhầm lẫn giữa bộ nhớ ảo và mức sử dụng RAM thực tế. Hướng dẫn nhấn mạnh rằng Resident Set Size (RSS) là chỉ số đáng tin cậy hơn về mức sử dụng bộ nhớ so với kích thước bộ nhớ ảo. Tài liệu cũng bao gồm cách diễn giải các trạng thái tiến trình và mức tải trung bình để cung cấp cái nhìn toàn diện về tình trạng hệ thống.

hackernews · theanonymousone · 7月4日 12:00 · [社区讨论](https://news.ycombinator.com/item?id=48784777)

**背景**: Các công cụ như top và htop là những tiện ích dòng lệnh tiêu chuẩn được sử dụng trong Linux để giám sát các tiến trình hệ thống và mức sử dụng tài nguyên theo thời gian thực. Chúng hiển thị thông tin quan trọng như tải CPU, mức tiêu thụ bộ nhớ và trạng thái của từng tiến trình. Việc hiểu các kết quả đầu ra này là nền tảng cho quản trị hệ thống và khắc phục sự cố Linux hiệu quả.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Resident_set_size">Resident set size - Wikipedia</a></li>
<li><a href="https://www.baeldung.com/linux/resident-set-vs-virtual-memory-size">Difference Between Resident Set Size and Virtual Memory Size | Baeldung on Linux</a></li>
<li><a href="https://www.digitalocean.com/community/tutorials/load-average-in-linux">What is Load Average in Linux? - DigitalOcean</a></li>

</ul>
</details>

**社区讨论**: Cộng đồng đề xuất các lựa chọn thay thế hiện đại như btop để có giao diện giàu thông tin hơn. Người dùng cũng chia sẻ các mẹo thực tế, chẳng hạn như bật chế độ xem cây tiến trình và tắt các luồng người dùng trong htop để giảm bớt sự lộn xộn.

**标签**: `#linux`, `#system-administration`, `#htop`, `#performance-monitoring`, `#cli`

---

<a id="item-13"></a>
## [Nhà sáng tạo khóa học độc lập báo cáo doanh thu sụt giảm đáng kể do AI](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 7.0/10

Nhà giáo dục độc lập Josh W. Comeau báo cáo rằng doanh số các khóa học gần đây của anh đã giảm xuống chỉ còn khoảng một phần ba so với mức thông thường. Anh cho rằng sự sụt giảm này xuất phát từ tâm lý lo ngại của các lập trình viên về an ninh việc làm và xu hướng chuyển sang sử dụng các mô hình ngôn ngữ lớn (LLM) để học tập cá nhân hóa. Xu hướng này làm nổi bật một thách thức kinh tế ngày càng lớn đối với các nhà sáng tạo độc lập, khi nội dung giáo dục của họ đang bị các mô hình AI thu thập mà không có sự đền bù. Nó cũng phản ánh sự bất ổn rộng lớn hơn trong ngành công nghệ liên quan đến tương lai của việc tiếp thu kỹ năng lập trình trong kỷ nguyên AI. Comeau lưu ý rằng anh và các nhà sáng tạo khác đang chứng kiến doanh thu giảm hơn 50%. Anh bày tỏ lo ngại rằng các LLM đang thực sự 'hút' nội dung của họ để cung cấp dịch vụ gia sư tự động, điều này làm giảm động lực để học viên mua các khóa học do con người biên soạn.

rss · Simon Willison · 7月3日 21:25

**背景**: Sự trỗi dậy của các LLM đã giới thiệu những công cụ mạnh mẽ cho việc gia sư cá nhân hóa, có khả năng thích ứng với nhu cầu của từng học viên trong thời gian thực. Đồng thời, ngành công nghiệp phần mềm đang trải qua sự thay đổi trong lộ trình nghề nghiệp, khi các lập trình viên ngày càng phụ thuộc vào AI cho các tác vụ lập trình, điều này đã làm dấy lên các cuộc tranh luận về sự cần thiết của việc xây dựng kỹ năng truyền thống.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2604.26962">DeepTutor: Towards Agentic Personalized Tutoring</a></li>
<li><a href="https://stackoverflow.blog/2025/12/26/ai-vs-gen-z/">AI vs Gen Z: How AI has changed the career pathway for junior developers - Stack Overflow</a></li>
<li><a href="https://brainhub.eu/library/software-developer-age-of-ai">Is There a Future for Software Engineers? The Impact of AI [2025]</a></li>

</ul>
</details>

**社区讨论**: Cuộc thảo luận phản ánh mối lo ngại rộng rãi giữa các nhà sáng tạo về tính bền vững của 'nền kinh tế sáng tạo' khi tài sản trí tuệ của họ bị sử dụng để huấn luyện chính những công cụ thay thế dịch vụ của họ. Nhiều người thừa nhận sự căng thẳng giữa tính tiện lợi của việc học qua AI và sự mất mát các nguồn tài nguyên giáo dục chất lượng cao do con người biên soạn.

**标签**: `#AI`, `#Developer Education`, `#Creator Economy`, `#LLMs`, `#Tech Industry`

---