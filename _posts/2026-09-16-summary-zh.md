---
layout: default
title: "Horizon Summary: 2026-09-16 (ZH)"
date: 2026-09-16
lang: zh
---

> 从 35 条内容中筛选出 19 条重要资讯。

---

1. [Internet Archive triển khai các biện pháp bảo vệ lưu lượng truy cập mới cho Wayback Machine](#item-1) ⭐️ 9.0/10
2. [Google ra mắt các mô hình Gemini 3.8 Live và Extended Thinking](#item-2) ⭐️ 9.0/10
3. [Prior Labs ra mắt TabPFN-3.5, mô hình nền tảng dữ liệu bảng đạt chuẩn SOTA mới](#item-3) ⭐️ 9.0/10
4. [Giới thiệu các mô hình System One và khung suy luận Jev](#item-4) ⭐️ 8.0/10
5. [Show HN: Khung tranh e-ink nhận diện tiếng chim và vẽ minh họa theo phong cách thế kỷ 19](#item-5) ⭐️ 8.0/10
6. [Các nhà nghiên cứu bảo mật giành quyền quản trị GitHub của Baseten qua token bị rò rỉ](#item-6) ⭐️ 8.0/10
7. [Giải quyết tình trạng suy giảm chất lượng và độ bền sản phẩm](#item-7) ⭐️ 8.0/10
8. [Hệ thống tệp GEFS được giới thiệu dưới dạng bản xem trước trên OpenBSD](#item-8) ⭐️ 8.0/10
9. [Nghiên cứu mới lập luận rằng khả năng tự cải thiện đệ quy chưa sớm xảy ra](#item-9) ⭐️ 8.0/10
10. [Bảng mở rộng dịch thuật nhấp chuột MS MARCO: Cách tiếp cận DSSM 'bình dân'](#item-10) ⭐️ 8.0/10
11. [Lập trình viên tuyên bố xây dựng driver GPU Linux cho M4 Mac Mini bằng LLM](#item-11) ⭐️ 7.0/10
12. [Show HN: Capsule – Ứng dụng web tệp đơn lưu trữ dữ liệu vào SQLite](#item-12) ⭐️ 7.0/10
13. [Nghi vấn phá hoại gây gián đoạn nghiêm trọng mạng lưới đường sắt Hà Lan](#item-13) ⭐️ 7.0/10
14. [Công cụ quản lý gói uv phiên bản 0.12.14 đã được phát hành](#item-14) ⭐️ 6.0/10
15. [Rheinmetall công bố tài liệu kỹ thuật cho giao thức hệ thống vũ khí OnboardAPI](#item-15) ⭐️ 6.0/10
16. [Đánh giá mức độ hoàn thiện của công trình nghiên cứu cho hội thảo Machine Learning](#item-16) ⭐️ 6.0/10
17. [Các chiến lược xử lý thống kê tập dữ liệu không thể tái lập trong nghiên cứu học thuật](#item-17) ⭐️ 6.0/10
18. [Tìm kích thước lô tự động cho Accelerate với FSDP2](#item-18) ⭐️ 6.0/10
19. [Lựa chọn giữa ngành Khoa học máy tính và Kỹ thuật điện cho bằng Tiến sĩ AI](#item-19) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Internet Archive triển khai các biện pháp bảo vệ lưu lượng truy cập mới cho Wayback Machine](https://blog.archive.org/2026/09/15/an-update-on-wayback-machine-access/) ⭐️ 9.0/10

Internet Archive đang áp dụng các biện pháp quản lý lưu lượng truy cập mới cho Wayback Machine để giảm thiểu gián đoạn dịch vụ do hoạt động cào dữ liệu tự động với lưu lượng lớn gây ra. Các biện pháp bảo vệ này được thiết kế để duy trì sự ổn định của dịch vụ trước các bot cố gắng vượt qua hạn chế truy cập của các trang web gốc. Là một thư viện kỹ thuật số phi lợi nhuận quan trọng, Wayback Machine đang phải đối mặt với áp lực lớn từ việc thu thập dữ liệu phục vụ AI, điều này đe dọa sứ mệnh cung cấp quyền truy cập mở vào nội dung web lịch sử. Việc bảo vệ cơ sở hạ tầng này là rất cần thiết để đảm bảo tính bền vững lâu dài của kho lưu trữ kỹ thuật số công cộng. Người dùng có thể gặp phải tình trạng giới hạn tốc độ hoặc lỗi truy cập, chẳng hạn như mã trạng thái 429, khi tổ chức này nỗ lực lọc bỏ lưu lượng truy cập tự động độc hại. Các biện pháp này nhằm ưu tiên người dùng là con người đồng thời ngăn chặn việc lạm dụng kho lưu trữ bởi các hoạt động cào dữ liệu quy mô lớn.

hackernews · ChrisArchitect · 9月15日 17:52 · [社区讨论](https://news.ycombinator.com/item?id=49716176)

**背景**: Wayback Machine là một kho lưu trữ kỹ thuật số đã bảo tồn hàng tỷ trang web từ năm 1996, đóng vai trò là nguồn tài nguyên quan trọng cho các nhà nghiên cứu và công chúng. Cào dữ liệu web liên quan đến việc sử dụng các bot tự động để trích xuất lượng lớn thông tin từ các trang web, điều này có thể làm quá tải máy chủ và gây gián đoạn dịch vụ cho người dùng hợp pháp. Sự bùng nổ gần đây trong phát triển AI đã làm tăng quy mô của hoạt động cào dữ liệu này, gây áp lực chưa từng có lên cơ sở hạ tầng công cộng.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://web.archive.org/">Wayback Machine</a></li>
<li><a href="https://waybackmachine.app/">Wayback Machine - Explore Internet History</a></li>
<li><a href="https://datashift.dev/resources/web-scraping-for-enterprises">Web Scraping for Enterprises: The Strategic Guide 2026 | DataShift</a></li>

</ul>
</details>

**社区讨论**: Cộng đồng phần lớn ủng hộ các nỗ lực của Internet Archive, coi tổ chức này là người hùng vì đã duy trì quyền truy cập mở bất chấp áp lực lớn. Tuy nhiên, người dùng cũng bày tỏ sự thất vọng về các thiệt hại ngoài ý muốn, chẳng hạn như việc truy cập hợp pháp bị chặn, và lo ngại rằng cuộc chạy đua vũ trang AI đang gây ra những tổn hại không thể khắc phục đối với các tài nguyên web mở.

**标签**: `#Internet Archive`, `#Web Scraping`, `#Digital Preservation`, `#Infrastructure`, `#AI Ethics`

---

<a id="item-2"></a>
## [Google ra mắt các mô hình Gemini 3.8 Live và Extended Thinking](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/) ⭐️ 9.0/10

Google đã giới thiệu Gemini 3.8 Live với khả năng đàm thoại thời gian thực được cải tiến, cùng với chế độ 'Extended Thinking' được thiết kế cho các tác vụ suy luận phức tạp. Những cập nhật này nhằm mang lại các tương tác bằng giọng nói tự nhiên hơn và hiệu suất phân tích sâu sắc hơn cho người dùng. Bản phát hành này đại diện cho một bước tiến quan trọng trong việc giúp các trợ lý AI có khả năng xử lý các suy luận phức tạp, đồng thời duy trì giao tiếp bằng giọng nói có độ trễ thấp giống như con người. Điều này giúp Google cạnh tranh tốt hơn trong thị trường ứng dụng AI thời gian thực đang phát triển nhanh chóng. Chế độ Extended Thinking cho phép mô hình dành nhiều tài nguyên tính toán hơn cho việc suy luận trước khi phản hồi, trong khi Gemini 3.8 Live cải thiện khả năng xử lý giọng nói, bao gồm việc xử lý tốt hơn các giọng địa phương đặc trưng và giảm độ trễ.

hackernews · leumon · 9月15日 17:38 · [社区讨论](https://news.ycombinator.com/item?id=49715947)

**背景**: Gemini là dòng mô hình AI đa phương thức hàng đầu của Google, có khả năng xử lý văn bản, mã nguồn, âm thanh và video. Các tính năng 'Live' đề cập đến khả năng tương tác bằng giọng nói thời gian thực với độ trễ thấp, trong khi 'Extended Thinking' đề cập đến các cơ chế suy luận theo chuỗi cho phép mô hình tạm dừng và suy nghĩ về các vấn đề phức tạp trước khi đưa ra câu trả lời.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.google.dev/gemini-api/docs/thinking">Gemini thinking - Interactions API | Google AI for Developers</a></li>
<li><a href="https://www.androidheadlines.com/2026/06/google-gemini-extended-thinking-mode-levels-rollout.html">Google Launches Gemini Extended Thinking Mode for All Users</a></li>

</ul>
</details>

**社区讨论**: Người dùng nhìn chung rất ấn tượng với khả năng xử lý giọng địa phương của mô hình và tính hữu ích của nó trong việc học ngôn ngữ, mặc dù một số người vẫn hoài nghi về khả năng cạnh tranh so với các mô hình của đối thủ như OpenAI. Người dùng cũng đánh giá cao việc các tính năng này đã khả dụng hơn trên các tài khoản Google Workspace.

**标签**: `#AI`, `#Gemini`, `#Google`, `#LLM`, `#Conversational AI`

---

<a id="item-3"></a>
## [Prior Labs ra mắt TabPFN-3.5, mô hình nền tảng dữ liệu bảng đạt chuẩn SOTA mới](https://www.reddit.com/r/MachineLearning/comments/1wh4xhy/tabpfn35_is_released_as_the_next_sota_tabular/) ⭐️ 9.0/10

Prior Labs vừa ra mắt TabPFN-3.5, một mô hình nền tảng dữ liệu bảng mới đạt hiệu suất dẫn đầu trên các bảng xếp hạng TabArena và BeyondArena. Bản phát hành này bao gồm các biến thể chuyên biệt như TabPFN-3.5-Fast giúp tăng tốc độ và TabPFN-3.5-Thinking giúp cải thiện độ chính xác. Sự kiện này đánh dấu bước tiến quan trọng trong học máy trên dữ liệu bảng nhờ khả năng xử lý các tập dữ liệu có số chiều và độ đa dạng cao với điểm Elo vượt trội. Nó cung cấp một công cụ mạnh mẽ, sẵn sàng sử dụng cho phân tích dữ liệu phức tạp mà không cần huấn luyện lại nhiều. TabPFN-3.5 hỗ trợ các tập dữ liệu lên tới 1 triệu hàng và 20.000 đặc trưng, vượt xa các mô hình cơ sở trước đó. Biến thể 'Thinking' cho phép người dùng đánh đổi thêm tài nguyên tính toán để đạt được độ chính xác dự báo cao hơn.

reddit · r/MachineLearning · /u/tuanacelik · 9月15日 16:18

**背景**: TabPFN là mô hình dựa trên kiến trúc Transformer được thiết kế cho học trong ngữ cảnh (in-context learning), cho phép thực hiện dự báo trên dữ liệu bảng mà không cần cập nhật tham số theo cách truyền thống. TabArena đóng vai trò là một hệ thống đánh giá trực tuyến, liên tục kiểm tra và xếp hạng các mô hình học máy trên dữ liệu bảng dựa trên hiệu suất của chúng qua nhiều tập dữ liệu khác nhau.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TabPFN">TabPFN</a></li>
<li><a href="https://arxiv.org/abs/2506.16791">TabArena : A Living Benchmark for Machine Learning on Tabular Data</a></li>
<li><a href="https://github.com/PriorLabs/TabPFN">GitHub - PriorLabs/ TabPFN : TabPFN : Foundation Model for Tabular...</a></li>

</ul>
</details>

**社区讨论**: Cộng đồng đã thể hiện sự quan tâm lớn đối với khả năng xử lý dữ liệu bảng quy mô lớn của mô hình và những cải thiện đáng kể về điểm Elo so với các phiên bản trước. Các cuộc thảo luận nhấn mạnh tính hữu dụng thực tế của biến thể 'Thinking' đối với những người dùng ưu tiên độ chính xác trong các ứng dụng quan trọng.

**标签**: `#machine-learning`, `#tabular-data`, `#foundation-models`, `#ai-research`, `#sota`

---

<a id="item-4"></a>
## [Giới thiệu các mô hình System One và khung suy luận Jev](https://typesafe.ai/blog/introducing-system-one-models-and-jev) ⭐️ 8.0/10

Jev là một khung suy luận mới ưu tiên đầu ra có cấu trúc, an toàn về kiểu dữ liệu và tốc độ cao thay vì tạo văn bản đa năng như các LLM truyền thống. Nó giới thiệu các mô hình 'System One' được thiết kế đặc biệt cho các tác vụ hạn chế như phân loại và chấm điểm. Cách tiếp cận này mang lại sự cải thiện hiệu suất đáng kể cho các ứng dụng thực tế cần dữ liệu có cấu trúc đáng tin cậy thay vì văn bản tự do. Nó thu hẹp khoảng cách giữa các mô hình mã hóa truyền thống và AI tạo sinh hiện đại bằng cách áp đặt các lược đồ đầu ra nghiêm ngặt. Khung này tập trung vào các loại đầu vào cụ thể như 'Choice', 'Score' hoặc 'Null' để đảm bảo đầu ra có thể dự đoán được. Nó sử dụng học tăng cường từ dữ liệu tương phản (RLCD) để tối ưu hóa các mô hình chuyên biệt này cho các tác vụ đòi hỏi độ chính xác cao.

hackernews · albelfio · 9月15日 19:25 · [社区讨论](https://news.ycombinator.com/item?id=49717558)

**背景**: Các LLM truyền thống được thiết kế để tạo văn bản tự do, điều này có thể gây kém hiệu quả và khó dự đoán đối với các ứng dụng phần mềm yêu cầu dữ liệu có cấu trúc. Suy luận an toàn về kiểu dữ liệu đảm bảo rằng đầu ra của mô hình tuân thủ nghiêm ngặt các cấu trúc dữ liệu đã xác định trước, giúp ngăn ngừa lỗi thời gian chạy trong các hệ thống hạ nguồn.

**社区讨论**: Cộng đồng rất quan tâm đến lợi ích về hiệu suất nhưng tranh luận liệu việc so sánh tốc độ với các LLM đa năng có công bằng hay không. Người dùng cũng lưu ý những điểm tương đồng với các mô hình thiết kế theo hợp đồng (design-by-contract) hiện có và đặt câu hỏi về sự khác biệt giữa công nghệ này với các mô hình chỉ sử dụng bộ mã hóa truyền thống.

**标签**: `#LLM`, `#Inference`, `#Type-Safety`, `#Software Engineering`, `#AI Infrastructure`

---

<a id="item-5"></a>
## [Show HN: Khung tranh e-ink nhận diện tiếng chim và vẽ minh họa theo phong cách thế kỷ 19](https://github.com/arnegiacomo/fugleramme) ⭐️ 8.0/10

Dự án sử dụng mạng thần kinh BirdNET để nhận diện các loài chim địa phương thông qua âm thanh và tạo ra các hình minh họa theo phong cách thế kỷ 19 trên màn hình e-ink theo thời gian thực. Nó kết nối hiệu quả giữa xử lý âm thanh kỹ thuật số và nghệ thuật vật lý đầy thẩm mỹ. Dự án này cho thấy cách AI có thể được tích hợp vào phần cứng hàng ngày để tạo ra những trải nghiệm người dùng đầy 'phép màu' và hữu hình. Nó làm nổi bật xu hướng ngày càng tăng trong việc sử dụng các mạng thần kinh chuyên biệt để theo dõi thiên nhiên và thể hiện sự sáng tạo. Hệ thống dựa vào BirdNET, một bộ phân loại mạng thần kinh truyền thống thay vì LLM, để thực hiện nhận diện loài chim chính xác. Thiết lập phần cứng được thiết kế để tiêu thụ điện năng thấp, tạo nên một tác phẩm bền vững và lâu dài.

hackernews · arnemunthekaas · 9月15日 12:31 · [社区讨论](https://news.ycombinator.com/item?id=49711544)

**背景**: BirdNET là một mô hình học sâu chuyên dụng được huấn luyện để nhận diện hàng ngàn loài chim từ các bản ghi âm. Màn hình e-ink rất phổ biến trong các dự án của cộng đồng maker vì chúng chỉ tiêu thụ điện năng khi cập nhật hình ảnh, cho phép thời lượng pin cực dài. Những công nghệ này thường được kết hợp với các vi điều khiển như ESP32 để tạo ra các thiết bị IoT kết nối, tiêu thụ điện năng thấp.

**社区讨论**: Cộng đồng đánh giá rất cao dự án vì sự kết hợp sáng tạo giữa công nghệ và nghệ thuật, nhiều người dùng cảm thấy nó rất truyền cảm hứng. Những người tham gia cũng thảo luận về hiệu suất kỹ thuật của màn hình e-ink và bộ phân loại BirdNET làm nền tảng.

**标签**: `#hardware`, `#ai`, `#e-ink`, `#maker`, `#iot`

---

<a id="item-6"></a>
## [Các nhà nghiên cứu bảo mật giành quyền quản trị GitHub của Baseten qua token bị rò rỉ](https://www.strix.ai/blog/baseten-harbor-github-pat-takeover) ⭐️ 8.0/10

Một công ty nghiên cứu bảo mật đã sử dụng tác nhân tự động để phát hiện Personal Access Token (PAT) của GitHub bị rò rỉ trong lịch sử xây dựng Docker công khai. Token này đã cấp cho các nhà nghiên cứu quyền quản trị đối với các kho lưu trữ sản phẩm của Baseten chỉ trong vòng 25 phút. Sự cố này làm nổi bật những rủi ro nghiêm trọng khi để lộ thông tin xác thực nhạy cảm trong các tệp tin xây dựng container và cho thấy khả năng ngày càng tăng của các tác nhân AI trong việc xác định các lỗ hổng bảo mật quan trọng. Đây là lời nhắc nhở mạnh mẽ cho các tổ chức về việc cần kiểm tra các quy trình CI/CD để tránh rò rỉ bí mật. Token bị rò rỉ cung cấp quyền hạn rộng rãi, bao gồm quyền quản trị và quyền đẩy mã nguồn vào các kho lưu trữ sản phẩm cốt lõi và cơ sở hạ tầng GitOps. Các nhà nghiên cứu đã tiết lộ lỗ hổng này một cách có trách nhiệm cho Baseten, đơn vị sau đó đã xoay vòng token và bảo mật dự án bị ảnh hưởng.

hackernews · bearsyankees · 9月15日 18:11 · [社区讨论](https://news.ycombinator.com/item?id=49716476)

**背景**: Personal Access Token (PAT) của GitHub đóng vai trò như mật khẩu thay thế để xác thực với các API của GitHub, và nếu bị rò rỉ, chúng có thể cấp quyền truy cập trái phép vào các kho lưu trữ riêng tư. Các hình ảnh Docker thường vô tình bao gồm các tệp nhạy cảm nếu ngữ cảnh xây dựng không được làm sạch đúng cách, khiến các bí mật bị lộ trong các lớp hình ảnh công khai.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens">Managing your personal access tokens - GitHub Docs</a></li>
<li><a href="https://nhimg.org/massive-docker-hub-leak-10000-images-expose-secrets-and-auth-keys">Massive Docker Hub Leak : 10,000+ Images Expose Secrets and Auth...</a></li>

</ul>
</details>

**社区讨论**: Cộng đồng đã khen ngợi phản ứng nhanh chóng của Baseten nhưng tranh luận về đạo đức khi sử dụng một công ty thực tế làm nghiên cứu điển hình cho tiếp thị. Một số người dùng bày tỏ sự không thoải mái với tính chất quyết liệt của việc công khai này, trong khi những người khác coi đó là một bài học quý giá về rủi ro của các cuộc tấn công bảo mật tự động.

**标签**: `#cybersecurity`, `#devsecops`, `#vulnerability-disclosure`, `#ai-security`, `#github-security`

---

<a id="item-7"></a>
## [Giải quyết tình trạng suy giảm chất lượng và độ bền sản phẩm](https://www.forbrukerradet.no/short-life/) ⭐️ 8.0/10

Cuộc thảo luận làm nổi bật cách các động lực thị trường và nhu cầu của người tiêu dùng về giá rẻ thúc đẩy chu kỳ lỗi thời có kế hoạch và giảm tuổi thọ sản phẩm. Nó xem xét cách các thương hiệu thường thỏa hiệp về chất lượng để duy trì mức giá trong bối cảnh chi phí sản xuất tăng cao. Xu hướng này ảnh hưởng đến quyền lợi người tiêu dùng và tính bền vững của môi trường, vì các sản phẩm bị thay thế thường xuyên hơn. Hiểu được những động lực này là điều cần thiết đối với người tiêu dùng đang tìm kiếm giá trị và các nhà hoạch định chính sách đang giải quyết vấn đề minh bạch thị trường. Phân tích chỉ ra hiện tượng 'bán rẻ thương hiệu', nơi các công ty khai thác danh tiếng đã gây dựng để bán hàng kém chất lượng hơn, cùng với khó khăn mà người tiêu dùng gặp phải khi so sánh chất lượng với giá cả. Sự thiếu minh bạch về kỹ thuật khiến người mua bình thường khó phân biệt giữa vật liệu bền và các sản phẩm thay thế rẻ tiền hơn.

hackernews · ingve · 9月15日 10:00 · [社区讨论](https://news.ycombinator.com/item?id=49710109)

**背景**: Lỗi thời có kế hoạch là một chiến lược kinh doanh trong đó các sản phẩm được thiết kế với thời hạn sử dụng hạn chế để chúng trở nên lỗi thời hoặc không còn chức năng sau một khoảng thời gian nhất định. Thực tiễn này buộc người tiêu dùng phải mua sản phẩm thay thế thường xuyên hơn, điều này thường gắn liền với áp lực kinh tế rộng lớn hơn của lạm phát và chuỗi cung ứng toàn cầu hóa.

**社区讨论**: Cộng đồng cho rằng chất lượng suy giảm là một hình thức lạm phát ẩn và lưu ý rằng người tiêu dùng thường ưu tiên giá rẻ hơn độ bền. Nhiều người bình luận cho rằng thật không công bằng khi mong đợi người mua phải là chuyên gia về vật liệu, vì các công ty cố tình làm cho chất lượng trở nên khó xác minh.

**标签**: `#economics`, `#consumer-rights`, `#manufacturing`, `#market-analysis`, `#sustainability`

---

<a id="item-8"></a>
## [Hệ thống tệp GEFS được giới thiệu dưới dạng bản xem trước trên OpenBSD](https://marc.info/?l=openbsd-tech&m=178948744271633&w=2) ⭐️ 8.0/10

Một bản xem trước của hệ thống tệp GEFS, vốn được phát triển cho hệ điều hành 9front, đã được chuyển đổi sang nền tảng OpenBSD. Việc triển khai này mang đến các tính năng toàn vẹn dữ liệu nâng cao cho hệ sinh thái OpenBSD. GEFS cung cấp khả năng bảo vệ dữ liệu mạnh mẽ thông qua cơ chế băm ở cấp độ khối, đây là một sự bổ sung quan trọng cho những người dùng ưu tiên độ tin cậy của lưu trữ. Sự xuất hiện của nó mang đến cho người dùng OpenBSD một giải pháp thay thế hiện đại để quản lý tính toàn vẹn của dữ liệu. Hệ thống tệp này sử dụng các con trỏ khối chứa mã băm của dữ liệu mà chúng trỏ tới, cho phép phát hiện và báo cáo tình trạng hỏng hóc từ phương tiện lưu trữ bên dưới. Nó đã được sử dụng thành công trong môi trường thực tế bởi cộng đồng 9front.

hackernews · sippingabonedry · 9月15日 17:12 · [社区讨论](https://news.ycombinator.com/item?id=49715590)

**背景**: GEFS là một hệ thống tệp được thiết kế với trọng tâm là tính toàn vẹn và nhất quán của dữ liệu, có nguồn gốc từ dự án 9front bắt nguồn từ Plan 9. OpenBSD là một hệ điều hành giống Unix nổi tiếng với sự chú trọng vào bảo mật, tính chính xác và chất lượng mã nguồn. Các hệ thống tệp như GEFS rất quan trọng đối với lưu trữ hiện đại vì chúng giúp ngăn chặn tình trạng hỏng dữ liệu âm thầm.

**社区讨论**: Cộng đồng có phản hồi khá tích cực, trong đó người dùng nhấn mạnh độ tin cậy đã được kiểm chứng của hệ thống tệp này trên 9front. Một số người tham gia bày tỏ sự quan tâm đến việc so sánh GEFS với các hệ thống tệp khác như HAMMER2 từ DragonFlyBSD.

**标签**: `#OpenBSD`, `#Filesystems`, `#GEFS`, `#Storage`, `#Systems Programming`

---

<a id="item-9"></a>
## [Nghiên cứu mới lập luận rằng khả năng tự cải thiện đệ quy chưa sớm xảy ra](https://www.reddit.com/r/MachineLearning/comments/1wgazy4/rsi_is_not_happening_r/) ⭐️ 8.0/10

Một nghiên cứu gần đây chứng minh rằng các tác nhân LLM hiện tại không thể thực hiện các nhiệm vụ nghiên cứu học máy mở ở mức độ tương đương với các nhà nghiên cứu con người. Các tác giả lập luận rằng vì những tác nhân này không thể hoàn thành thành công các dự án nghiên cứu phức tạp, triển vọng về khả năng tự cải thiện đệ quy (RSI) hiện chưa thể xảy ra trong tương lai gần. Phát hiện này thách thức giả định rằng các tác nhân AI sẽ tất yếu gây ra sự bùng nổ trí tuệ bằng cách tự động hóa quá trình nghiên cứu và phát triển của chính chúng. Nó cung cấp một cái nhìn thực tế cho các cuộc tranh luận về an toàn AI liên quan đến mốc thời gian và tính khả thi của siêu trí tuệ. Các nhà nghiên cứu đã đánh giá các tác nhân như Codex và OpenClaw bằng cách giao cho chúng các bài báo chưa xuất bản tại NeurIPS, với kết quả được chấm điểm bởi chính các tác giả gốc. Nghiên cứu nhấn mạnh rằng RSI đòi hỏi nhiều hơn là chỉ tăng tốc độ nghiên cứu; nó đòi hỏi khả năng thực hiện khám phá khoa học tự chủ ở cấp độ cao.

reddit · r/MachineLearning · /u/we_are_mammals · 9月14日 18:03

**背景**: Tự cải thiện đệ quy (RSI) là một khái niệm lý thuyết trong đó một hệ thống AI tự cải thiện mã nguồn hoặc kiến trúc của chính nó để trở nên thông minh hơn, có khả năng dẫn đến một 'sự bùng nổ trí tuệ'. Thuật ngữ này được I.J. Good đưa ra vào năm 1965 để mô tả một kịch bản giả định nơi máy móc vượt qua khả năng nhận thức của con người. Nghiên cứu hiện tại về các tác nhân AI thường tập trung vào khả năng đóng vai trò là nhà nghiên cứu tự chủ, nhưng nghiên cứu này cho thấy chúng vẫn thiếu các khả năng suy luận cần thiết cho sự tiến bộ tự định hướng thực sự.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement</a></li>
<li><a href="https://arxiv.org/abs/2505.19955">[2505.19955] MLR-Bench: Evaluating AI Agents on Open - Ended ...</a></li>

</ul>
</details>

**社区讨论**: Cuộc thảo luận trong cộng đồng khá phân cực, với một số người dùng chỉ trích phương pháp luận của bài báo hoặc định nghĩa về RSI, trong khi những người khác bày tỏ sự thất vọng vì thiếu sự tham gia thảo luận có ý nghĩa về các kết quả nghiên cứu. Có sự hoài nghi đáng kể về việc liệu các tiêu chuẩn đánh giá hiện tại có phản ánh chính xác tiềm năng cho các khả năng của tác nhân trong tương lai hay không.

**标签**: `#AI Safety`, `#Recursive Self-Improvement`, `#LLM Agents`, `#Machine Learning Research`, `#AGI`

---

<a id="item-10"></a>
## [Bảng mở rộng dịch thuật nhấp chuột MS MARCO: Cách tiếp cận DSSM 'bình dân'](https://www.reddit.com/r/MachineLearning/comments/1wg3g03/ms_marco_clicktranslation_expansion_tables_poor/) ⭐️ 8.0/10

Tác giả đã giới thiệu một kỹ thuật mở rộng tài liệu dựa trên đếm, sử dụng thống kê đồng xuất hiện chéo từ MS MARCO để làm phong phú chỉ mục đảo ngược. Phương pháp này hoạt động như một giải pháp thay thế hiệu quả về mặt tính toán cho các mô hình thần kinh phức tạp bằng cách chèn các thuật ngữ truy vấn liên quan hàng đầu trực tiếp vào các bài đăng tài liệu. Cách tiếp cận này cung cấp một phương pháp thực tế để cải thiện hiệu suất cơ sở BM25 trong các công cụ tìm kiếm mà không cần chi phí tính toán nặng nề của các mạng thần kinh sâu. Nó mang đến cho các nhà phát triển một giải pháp nhẹ nhàng tại thời điểm lập chỉ mục để cải thiện khả năng khớp ngữ nghĩa trong các hệ thống tìm kiếm toàn văn. Phương pháp này tính toán mối liên hệ giữa các đơn vị phía tài liệu và đơn vị phía truy vấn thông qua các cặp được giám sát, cho phép mở rộng tài liệu trong quá trình lập chỉ mục. Không giống như mô hình DSSM, phương pháp này bị giới hạn ở các phụ thuộc tuyến tính nhưng vẫn rất hiệu quả để tăng cường khả năng truy xuất cơ sở.

reddit · r/MachineLearning · /u/SpiritedTrip · 9月14日 13:28

**背景**: BM25 là một hàm xếp hạng được sử dụng rộng rãi để ước tính mức độ liên quan của các tài liệu đối với một truy vấn tìm kiếm dựa trên tần suất thuật ngữ. DSSM là một kiến trúc mạng thần kinh được thiết kế để ánh xạ các truy vấn và tài liệu vào một không gian ngữ nghĩa chung nhằm cải thiện độ chính xác khi truy xuất. Mở rộng tài liệu là một kỹ thuật được sử dụng để thêm các thuật ngữ có liên quan vào tài liệu nhằm tăng khả năng khớp với truy vấn của người dùng.

**标签**: `#Information Retrieval`, `#Search Engines`, `#NLP`, `#BM25`, `#Machine Learning`

---

<a id="item-11"></a>
## [Lập trình viên tuyên bố xây dựng driver GPU Linux cho M4 Mac Mini bằng LLM](https://codyho.dev/blog/gpu-driver/) ⭐️ 7.0/10

Một cá nhân được cho là đã phát triển thành công driver GPU Linux cho M4 Mac Mini chỉ trong một tháng bằng cách tận dụng LLM để dịch ngược phần cứng. Thành tựu này đã gây ra nhiều tranh cãi lớn do nền tảng chuyên môn của tác giả và việc sử dụng AI trong quá trình phát triển. Sự kiện này làm nổi bật tiềm năng của AI trong việc tăng tốc các tác vụ dịch ngược phức tạp, đồng thời đặt ra những câu hỏi quan trọng về nguồn gốc pháp lý, quyền sở hữu trí tuệ và đạo đức khi đưa mã nguồn do AI tạo ra vào các dự án mã nguồn mở. Dự án này đối mặt với những rào cản lớn để được đưa vào nhân Linux, đặc biệt là do chính sách nghiêm ngặt không sử dụng AI của dự án Asahi Linux và những lo ngại về việc tác giả có thể đã tiếp cận các bí mật thương mại của Apple.

hackernews · ADevWithAnIdea · 9月15日 19:30 · [社区讨论](https://news.ycombinator.com/item?id=49717638)

**背景**: Asahi Linux là một dự án cộng đồng tập trung vào việc chuyển đổi nhân Linux sang phần cứng Apple Silicon, vốn thiếu tài liệu chính thức từ Apple. Vì kiến trúc GPU của Apple là độc quyền và không có tài liệu công khai, các nhà phát triển thường mất nhiều năm để dịch ngược phần cứng theo cách thủ công nhằm tạo ra các driver hoạt động được. Việc sử dụng AI trong bối cảnh này gây tranh cãi gay gắt vì nó có thể vô tình kết hợp các bí mật thương mại được bảo hộ hoặc vi phạm các hướng dẫn đóng góp nghiêm ngặt của các dự án mã nguồn mở uy tín.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://asahilinux.org/">Asahi Linux</a></li>
<li><a href="https://en.wikipedia.org/wiki/Asahi_linux_project">Asahi linux project</a></li>

</ul>
</details>

**社区讨论**: Cộng đồng đang chia rẽ sâu sắc; một số người ca ngợi tốc độ của thành tựu kỹ thuật này, trong khi những người khác bày tỏ lo ngại mạnh mẽ về quá khứ của tác giả với tư cách là cựu kỹ sư Apple và những rủi ro pháp lý tiềm ẩn khi sử dụng mã do AI tạo ra. Nhiều người cho rằng mã nguồn này đã bị 'nhiễm bẩn' và không thể được chấp nhận bởi dự án Asahi Linux chính thức do các chính sách và tiêu chuẩn đạo đức nghiêm ngặt của họ.

**标签**: `#Linux`, `#GPU`, `#Apple Silicon`, `#Reverse Engineering`, `#LLM`

---

<a id="item-12"></a>
## [Show HN: Capsule – Ứng dụng web tệp đơn lưu trữ dữ liệu vào SQLite](https://withcapsule.app/) ⭐️ 7.0/10

Capsule là một công cụ mới được xây dựng bằng Rust và Tauri 2.0, cho phép đóng gói các ứng dụng web HTML cùng dữ liệu liên quan như hình ảnh hoặc tài liệu vào một tệp SQLite duy nhất và có tính di động cao. Công cụ này cung cấp một phương thức độc đáo để quản lý và chia sẻ các ứng dụng web ưu tiên cục bộ mà không cần phải lưu trữ trên máy chủ bên ngoài. Dự án này đơn giản hóa việc phân phối các công cụ nhỏ, được tạo bởi AI hoặc các công cụ cá nhân bằng cách đóng gói logic ứng dụng và dữ liệu người dùng lại với nhau. Nó giải quyết những khó khăn trong việc lưu trữ và quản lý trạng thái cho các tiện ích web đơn giản. Ứng dụng sử dụng UUID và dấu thời gian duy nhất cho mỗi mục dữ liệu để hỗ trợ việc hợp nhất, đồng thời áp dụng mô hình bảo mật nghiêm ngặt, trong đó các tài liệu mặc định không có quyền truy cập trực tiếp vào hệ thống tệp. Nó cũng hỗ trợ xuất dữ liệu sang các định dạng CSV hoặc JSON.

hackernews · bashtian · 9月15日 13:31 · [社区讨论](https://news.ycombinator.com/item?id=49712278)

**背景**: Phần mềm ưu tiên cục bộ (local-first) là một mô hình thiết kế trong đó dữ liệu được lưu trữ chủ yếu trên thiết bị của người dùng thay vì máy chủ từ xa, đảm bảo quyền riêng tư và khả năng hoạt động ngoại tuyến. Tauri là một khung làm việc để xây dựng các ứng dụng máy tính để bàn nhỏ, nhanh và an toàn bằng cách sử dụng các công nghệ web như HTML, CSS và JavaScript.

**社区讨论**: Cộng đồng có nhiều ý kiến trái chiều, một số người dùng khen ngợi sự đổi mới này trong khi những người khác cho rằng các API trình duyệt hiện đại như File System Access API đã làm cho việc đóng gói như vậy trở nên không cần thiết. Những người phản biện cũng đặt ra lo ngại về tính thực tiễn của việc chia sẻ các tệp đóng gói đối với các ứng dụng yêu cầu cập nhật trạng thái thường xuyên.

**标签**: `#web-development`, `#sqlite`, `#tauri`, `#local-first`, `#rust`

---

<a id="item-13"></a>
## [Nghi vấn phá hoại gây gián đoạn nghiêm trọng mạng lưới đường sắt Hà Lan](https://www.bbc.com/news/articles/c8ly49w9g1edo) ⭐️ 7.0/10

Mạng lưới đường sắt Hà Lan đã gặp phải sự gián đoạn dịch vụ nghiêm trọng do các hành vi nghi là phá hoại. Các cơ quan chức năng hiện đang điều tra các vụ việc để xác định nguyên nhân và tìm ra thủ phạm. Sự kiện này làm nổi bật tính dễ bị tổn thương của cơ sở hạ tầng quốc gia quan trọng trước các hành vi can thiệp có chủ đích. Nó làm dấy lên những lo ngại về an ninh của hệ thống giao thông và khả năng bị gián đoạn có phối hợp. Các chuyên gia lưu ý rằng hệ thống đường sắt được thiết kế để 'an toàn khi gặp lỗi' (fail-safe), điều này khiến chúng vốn dĩ rất dễ bị ép vào trạng thái dừng hoạt động. Mặc dù cơ chế này giúp ngăn ngừa va chạm, nhưng nó tạo ra một lỗ hổng lớn khi những kẻ xấu có thể dễ dàng làm tê liệt giao thông trên diện rộng.

hackernews · choult · 9月15日 10:22 · [社区讨论](https://news.ycombinator.com/item?id=49710253)

**背景**: Nguyên tắc thiết kế 'an toàn khi gặp lỗi' trong kỹ thuật đảm bảo rằng nếu hệ thống gặp sự cố, nó sẽ mặc định chuyển sang trạng thái ngăn ngừa thiệt hại, chẳng hạn như dừng tất cả các đoàn tàu. Vụ việc này xảy ra trùng với 'Prinsjesdag', một sự kiện thường niên tại Hà Lan nơi quốc vương đọc diễn văn nêu rõ chính sách của chính phủ, thường thu hút các cuộc biểu tình của công chúng.

**社区讨论**: Cộng đồng đang thảo luận về vụ việc trong bối cảnh các vụ phá hoại đường sắt tương tự gần đây ở Pháp và những căng thẳng địa chính trị rộng lớn hơn. Nhiều người bình luận chỉ ra rằng bản chất 'an toàn khi gặp lỗi' của cơ sở hạ tầng đường sắt khiến nó trở thành mục tiêu gây gián đoạn tốn ít công sức nhưng có tác động lớn.

**标签**: `#infrastructure`, `#cybersecurity`, `#transportation`, `#geopolitics`, `#systems-engineering`

---

<a id="item-14"></a>
## [Công cụ quản lý gói uv phiên bản 0.12.14 đã được phát hành](https://github.com/astral-sh/uv/releases/tag/0.12.14) ⭐️ 6.0/10

Trình quản lý gói uv phiên bản 0.12.14 giới thiệu khả năng tiếp tục tải xuống bị gián đoạn thông qua các yêu cầu HTTP Range và cải thiện chẩn đoán lỗi với các gợi ý nhất quán. Phiên bản này cũng tinh chỉnh mã thoát để phân biệt rõ hơn giữa các lỗi dự kiến và lỗi vận hành nội bộ. Những cải tiến này giúp tăng năng suất cho nhà phát triển bằng cách cung cấp phản hồi rõ ràng hơn khi cài đặt gói thất bại và tăng độ tin cậy trong môi trường mạng không ổn định. Bản cập nhật này đảm bảo uv tiếp tục là một công cụ mạnh mẽ và dễ sử dụng để quản lý các phụ thuộc Python. Bản phát hành bao gồm các tối ưu hóa hiệu suất cho việc giải quyết phụ thuộc từ wheelhouse cục bộ và các chỉ mục gói lớn, cùng với các bản sửa lỗi cho hỗ trợ đường dẫn dài trên Windows và phát hiện trình thông dịch Python trên Unix. Tính năng xem trước mới, `batch-export`, cho phép người dùng xuất nhiều lựa chọn phụ thuộc từ một lockfile dùng chung trong một lần gọi lệnh.

github · astral-releases-bot[bot] · 9月15日 02:19

**背景**: uv là trình quản lý gói Python hiệu năng cao được viết bằng Rust, được thiết kế để thay thế các công cụ như pip và pip-tools. Các yêu cầu HTTP Range cho phép máy khách chỉ tải xuống các phần cụ thể của tệp, điều này rất cần thiết để tiếp tục quá trình tải xuống bị gián đoạn mà không cần bắt đầu lại từ đầu. Lockfile được sử dụng để cố định các phụ thuộc vào các phiên bản cụ thể, đảm bảo các bản dựng có thể tái lập trên các môi trường khác nhau.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HTTP_Range_request">HTTP Range request</a></li>
<li><a href="https://dev.to/shalvah/understanding-lockfiles-1m10">Understanding Lockfiles - DEV Community</a></li>

</ul>
</details>

**标签**: `#python`, `#package-management`, `#uv`, `#developer-tools`

---

<a id="item-15"></a>
## [Rheinmetall công bố tài liệu kỹ thuật cho giao thức hệ thống vũ khí OnboardAPI](https://rheinmetall.github.io/onboardapi-documentation/9.10.0/index.html) ⭐️ 6.0/10

Rheinmetall đã công bố tài liệu kỹ thuật cho OnboardAPI, một giao thức được sử dụng trong các hệ thống vũ khí kết nối của họ. Việc phát hành này cung cấp quyền truy cập công khai vào các thông số kỹ thuật của giao diện thay vì mã nguồn thực tế. Việc phát hành này mang đến cái nhìn hiếm hoi về các tiêu chuẩn quản lý giao diện phần cứng cấp quân sự hiện đại. Nó nhấn mạnh sự phụ thuộc của ngành công nghiệp vào các giao thức truyền thông đã được thiết lập cho các hệ thống quốc phòng phân tán và phức tạp. OnboardAPI được xây dựng dựa trên tiêu chuẩn Data Distribution Service (DDS). Các nhà phê bình lưu ý rằng mặc dù tài liệu mang tính thông tin, nhưng kiến trúc DDS cơ bản thường bị coi là quá nặng nề và phức tạp đối với một số ứng dụng hệ thống nhúng.

hackernews · summarity · 9月15日 21:07 · [社区讨论](https://news.ycombinator.com/item?id=49718928)

**背景**: DDS là một giao thức trung gian được thiết kế để trao đổi dữ liệu thời gian thực trong các hệ thống phân tán, thường được sử dụng trong quốc phòng và tự động hóa công nghiệp. Nó tạo điều kiện thuận lợi cho việc giao tiếp giữa các thành phần khác nhau bằng cách quản lý luồng dữ liệu và chất lượng dịch vụ. Tuy nhiên, việc triển khai nó có thể tiêu tốn nhiều tài nguyên, dẫn đến các cuộc tranh luận về tính phù hợp của nó đối với các môi trường nhúng bị hạn chế.

**社区讨论**: Cộng đồng tỏ ra hoài nghi, lưu ý rằng đây chỉ là tài liệu chứ không phải mã nguồn mở. Nhiều người dùng bày tỏ sự thất vọng về việc phụ thuộc vào DDS, so sánh hệ thống này với ROS2 dành cho phần cứng quân sự và đặt câu hỏi về tính hữu dụng thực tế của tài liệu này.

**标签**: `#DDS`, `#MilitaryTech`, `#Protocols`, `#EmbeddedSystems`, `#OpenSource`

---

<a id="item-16"></a>
## [Đánh giá mức độ hoàn thiện của công trình nghiên cứu cho hội thảo Machine Learning](https://www.reddit.com/r/MachineLearning/comments/1wgv7hi/how_much_work_in_progress_can_a_workshop/) ⭐️ 6.0/10

Một nhà nghiên cứu đang tìm kiếm lời khuyên từ cộng đồng về việc liệu một thuật toán sơ bộ chỉ giải quyết được một phần vấn đề có đủ điều kiện để nộp cho hội thảo hay không. Đề xuất này bao gồm việc trình bày các kết quả hiện tại cùng với lộ trình lý thuyết cho các phần mở rộng trong tương lai. Việc hiểu rõ ngưỡng yêu cầu cho các bài nộp hội thảo là rất quan trọng đối với các nhà nghiên cứu trẻ, những người cần cân bằng giữa việc công bố kết quả học thuật và bản chất đang phát triển của nghiên cứu. Các hội thảo thường là nơi nhận phản hồi sớm, khiến sự phân biệt này trở nên thiết yếu cho sự phát triển chuyên môn. Các bài nộp hội thảo thường ưu tiên thảo luận và phản hồi hơn là các yêu cầu khắt khe về tính mới như ở các hội nghị chính. Tuy nhiên, tác giả cần đảm bảo rằng công trình được trình bày cung cấp đủ nội dung để tạo ra sự tương tác có ý nghĩa với các đồng nghiệp.

reddit · r/MachineLearning · /u/strammerrammer · 9月15日 09:13

**背景**: Trong lĩnh vực học thuật về machine learning, các hội thảo là những sự kiện chuyên biệt được tổ chức song song với các hội nghị lớn như NeurIPS hoặc ICML. Khác với các bài nộp chính thức đòi hỏi kết quả hoàn thiện và có tính mới cao, các hội thảo được thiết kế để thúc đẩy sự hợp tác và thảo luận về các ý tưởng mới nổi hoặc các nghiên cứu đang trong quá trình thực hiện.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dryfta.com/how-to-set-abstract-submission-criteria-for-conferences/">How to Set Abstract Submission Criteria for Conferences</a></li>
<li><a href="https://dfrws.org/submission-criteria/">Submission Criteria DFRWS APAC/EU/USA - DFRWS</a></li>

</ul>
</details>

**社区讨论**: Cộng đồng nhìn chung khuyến khích việc nộp các công trình đang thực hiện cho các hội thảo, nhấn mạnh rằng những nơi này được thiết kế đặc biệt để nhận phản hồi sớm và kết nối thay vì là các ấn phẩm đã hoàn thiện và có tầm ảnh hưởng lớn.

**标签**: `#machine learning`, `#academic research`, `#workshop submission`, `#career advice`

---

<a id="item-17"></a>
## [Các chiến lược xử lý thống kê tập dữ liệu không thể tái lập trong nghiên cứu học thuật](https://www.reddit.com/r/MachineLearning/comments/1wgutx6/d_how_do_you_get_preprocessed_dataset_of_a_paper_d/) ⭐️ 6.0/10

Một chủ đề thảo luận trên Reddit cung cấp lời khuyên thực tế cho các nhà nghiên cứu đang gặp khó khăn trong việc tái lập các thống kê tập dữ liệu khi tác giả không chia sẻ dữ liệu đã tiền xử lý hoặc không phản hồi. Chủ đề này khám phá các phương pháp ghi lại sự khác biệt và quản lý việc liên lạc với tác giả cũng như các tạp chí. Cuộc thảo luận này làm nổi bật một vấn đề nhức nhối trong 'cuộc khủng hoảng khả năng tái lập' trong lĩnh vực machine learning, nơi các quy trình tiền xử lý không minh bạch gây cản trở việc kiểm chứng khoa học. Việc giải quyết những vấn đề này là rất cần thiết để duy trì tính toàn vẹn và độ tin cậy của nghiên cứu học thuật. Chủ đề gợi ý rằng các nhà nghiên cứu nên ghi lại rõ ràng mọi sự khác biệt thay vì cố gắng ép buộc dữ liệu khớp với quy mô đã báo cáo, vì việc lấy mẫu tùy ý có thể tạo ra những sai lệch mới. Nó cũng cung cấp hướng dẫn về thời điểm và cách thức liên hệ với biên tập viên tạp chí liên quan đến các tác giả không phản hồi.

reddit · r/MachineLearning · /u/Individual-Safety906 · 9月15日 08:50

**背景**: Cuộc khủng hoảng khả năng tái lập trong machine learning đề cập đến khó khăn trong việc sao chép các kết quả đã công bố do thiếu mã nguồn, quy trình xử lý dữ liệu không minh bạch hoặc thiếu tài liệu hướng dẫn. Các quy trình tiền xử lý dữ liệu rất cần thiết để chuyển đổi dữ liệu thô thành định dạng phù hợp cho việc huấn luyện mô hình, và sự không nhất quán trong các bước này thường dẫn đến các thống kê tập dữ liệu cuối cùng khác nhau.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/analytics-vidhya/how-reproducibility-crisis-is-eating-away-the-credibility-of-machine-learning-technology-a4db017f85e4?responsesOpen=true">How Reproducibility Crisis is Eating Away the Credibility of Machine ...</a></li>
<li><a href="https://hbiostat.org/papers/kap23lea.pdf">Leakage and the reproducibility crisis in machine - learning -based...</a></li>
<li><a href="https://diogoribeiro7.github.io/data-science/data_preprocessing_pipelines/">Building Data Preprocessing Pipelines for Reliable Models</a></li>

</ul>
</details>

**社区讨论**: Cộng đồng thường khuyên nên minh bạch bằng cách ghi lại chính xác các bước đã thực hiện và những khác biệt thu được. Nhiều người dùng gợi ý rằng nếu tác giả vẫn không phản hồi, các nhà nghiên cứu nên công bố kết quả của riêng họ kèm theo lưu ý rằng họ không thể tái lập các thống kê ban đầu.

**标签**: `#machine-learning`, `#reproducibility`, `#academic-research`, `#data-science`

---

<a id="item-18"></a>
## [Tìm kích thước lô tự động cho Accelerate với FSDP2](https://www.reddit.com/r/MachineLearning/comments/1wg9u62/how_to_automatically_find_the_batch_size_when/) ⭐️ 6.0/10

Một nhà phát triển đang tìm kiếm phương pháp để tự động phát hiện kích thước lô (batch size) và khôi phục lỗi CUDA OOM khi sử dụng Hugging Face Accelerate với FSDP2 trong môi trường đa GPU. Hiện tại, tính năng này được hỗ trợ cho huấn luyện đơn GPU nhưng vẫn thiếu quy trình triển khai rõ ràng cho các thiết lập phân tán. Quản lý bộ nhớ hiệu quả là yếu tố then chốt để huấn luyện các mô hình lớn, và việc thiếu khả năng tự động khôi phục lỗi OOM trong huấn luyện phân tán buộc các nhà phát triển phải điều chỉnh kích thước lô thủ công, gây tốn thời gian và dễ sai sót. Giải quyết vấn đề này sẽ giúp tối ưu hóa quy trình tinh chỉnh các mô hình ngôn ngữ lớn trên phần cứng hạn chế. Người dùng đang đặt câu hỏi liệu Accelerate có thể khởi động lại các tiến trình phân tán với kích thước lô nhỏ hơn khi gặp lỗi CUDA OOM hay không, hay việc này đòi hỏi phải triển khai tùy chỉnh bên ngoài. FSDP2 là một kiến trúc mới hơn, gây ra các phức tạp trong việc quản lý trạng thái giữa các tiến trình phân tán, khiến việc khởi động lại đơn giản trở nên khó khăn.

reddit · r/MachineLearning · /u/zdeneklapes · 9月14日 17:24

**背景**: Hugging Face Accelerate là một thư viện giúp đơn giản hóa việc chạy huấn luyện PyTorch trên nhiều cấu hình phần cứng khác nhau. FSDP2 (Fully Sharded Data Parallel) là một kỹ thuật huấn luyện tiết kiệm bộ nhớ bằng cách phân mảnh các tham số mô hình, gradient và trạng thái bộ tối ưu hóa trên nhiều GPU. Lỗi CUDA OOM (hết bộ nhớ) xảy ra khi yêu cầu bộ nhớ của mô hình vượt quá dung lượng VRAM khả dụng trên GPU.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pyemma.github.io/FSDP2-Code-Walk/">FSDP 2 Under the Hood - A Deep Dive into PyTorch 's Fully Sharded...</a></li>
<li><a href="https://discuss.pytorch.org/t/is-it-safe-to-recover-from-cuda-oom/12754">Is it safe to recover from CUDA OOM ? - PyTorch Forums</a></li>
<li><a href="https://github.com/hyf020908/distributed-llm-lab">GitHub - hyf020908/ distributed -llm-lab: A systems engineering toolkit...</a></li>

</ul>
</details>

**社区讨论**: Cuộc thảo luận nhấn mạnh khó khăn kỹ thuật trong việc đồng bộ hóa các điều chỉnh kích thước lô trên nhiều tiến trình phân tán, vì tất cả các tiến trình thường phải duy trì cùng một kích thước lô để tránh làm lệch quá trình huấn luyện.

**标签**: `#Machine Learning`, `#Hugging Face`, `#FSDP2`, `#Distributed Training`, `#CUDA`

---

<a id="item-19"></a>
## [Lựa chọn giữa ngành Khoa học máy tính và Kỹ thuật điện cho bằng Tiến sĩ AI](https://www.reddit.com/r/MachineLearning/comments/1wfte3b/phd_branding_question_r/) ⭐️ 6.0/10

Một nghiên cứu sinh tương lai đang cân nhắc việc chọn khoa Khoa học máy tính (CS) hay Kỹ thuật điện (EE) để tối ưu hóa cơ hội nghề nghiệp cho vị trí nhà khoa học nghiên cứu tại các tập đoàn công nghệ lớn. Quyết định này làm nổi bật tầm quan trọng chiến lược của thương hiệu học thuật trong thị trường việc làm AI đầy cạnh tranh, nơi các nhà tuyển dụng thường sử dụng hệ thống lọc hồ sơ tự động. Nghiên cứu của sinh viên này tập trung vào Graph ML và xử lý tín hiệu đồ thị, vốn là những lĩnh vực nằm ở điểm giao thoa giữa ngành CS và EE.

reddit · r/MachineLearning · /u/legoWolf13 · 9月14日 04:26

**背景**: Tại nhiều trường đại học, các chủ đề nghiên cứu như mạng thần kinh đồ thị và xử lý tín hiệu mang tính liên ngành, cho phép sinh viên lựa chọn khoa trực thuộc. Việc chọn khoa có thể ảnh hưởng đến cách hồ sơ được phân loại bởi hệ thống theo dõi ứng viên (ATS) và cách các nhà tuyển dụng nhìn nhận trọng tâm kỹ thuật của ứng viên.

**社区讨论**: Cuộc thảo luận trong cộng đồng tập trung vào việc liệu tên khoa có quan trọng hơn kết quả nghiên cứu thực tế hay không, với nhiều ý kiến cho rằng chất lượng công bố khoa học và khả năng kết nối quan trọng hơn tên bằng cấp.

**标签**: `#PhD`, `#Career Advice`, `#Machine Learning`, `#Graph Neural Networks`, `#Industry Research`

---