# Track Decision Memo - Phase 2

**Họ tên:** Trần Văn Khoa  
**MSSV:** 2A202600827  
**Ngày:** 17/06/2026  
**Artifact:** B1 - Research thị trường, B2 - Research role 2 chiều, B3 - Track Decision Memo

---

## B1. Research Thị Trường Tương Lai

### Tín hiệu thị trường mình ghi nhận

- Nhu cầu không chỉ nằm ở việc "biết dùng ChatGPT", mà nằm ở khả năng xây ứng dụng AI có thể chạy thật, đo được chất lượng và kiểm soát được rủi ro.
- Các kỹ năng đang tăng nhanh: RAG, agentic workflow, tool calling, evaluation, guardrails, observability, deployment và cost control.
- Các công ty cần người nối được nhiều lớp: dữ liệu, backend, model, prompt, API, monitoring và trải nghiệm người dùng.
- Những vai trò AI thực tế ngày càng yêu cầu evidence: benchmark, log, dashboard, latency, cost, failure analysis, thay vì chỉ demo trả lời hay.

### Năng lực đang tăng

- Xây LLM application end-to-end.
- Thiết kế RAG pipeline có citation và đánh giá retrieval.
- Làm evaluation cho AI agent: golden dataset, LLM-as-judge, regression testing.
- Thiết kế guardrails và HITL cho các case rủi ro.
- Deploy và theo dõi hệ thống AI bằng logs, traces, metrics, alerts.

### Năng lực đang khan

- Người hiểu cả AI prototype và production engineering.
- Người biết debug AI theo pipeline: data -> retrieval -> generation -> evaluation -> observability.
- Người có thể biến demo AI thành sản phẩm có test, benchmark, guardrail và release gate.

### Điều làm mình bất ngờ

Mình bất ngờ vì phần khó nhất của AI app không phải lúc nào cũng là model. Nhiều lỗi đến từ dữ liệu, chunking, metadata, parser, môi trường chạy, port, `.env`, database, logging hoặc thiếu eval. Điều này làm mình thấy AI Engineer cần tư duy hệ thống nhiều hơn mình nghĩ ban đầu.

---

## B2. Research Role 2 Chiều

### Role mình chọn

**AI Application Engineer / LLM Application Engineer**

Role này nằm giữa backend, AI agent, RAG, evaluation và production readiness. Đây là hướng gần nhất với những artifact mình đã làm trong Phase 1.

### Bên ngoài - role này đòi hỏi gì?

- Thành thạo Python và có khả năng tích hợp API/backend.
- Hiểu LLM, prompt engineering, tool calling và agent workflow.
- Xây RAG pipeline: ingestion, chunking, embedding, vector database, hybrid retrieval, reranking, citation.
- Biết đánh giá AI system bằng benchmark, hit rate, MRR, faithfulness, answer relevancy, latency và cost.
- Biết guardrails: prompt injection defense, refusal, topic filter, PII handling, human-in-the-loop.
- Biết triển khai và vận hành: Docker, cloud deployment, health/readiness, structured logging, tracing, metrics, alerts.
- Có portfolio hoặc artifact chứng minh được hệ thống AI end-to-end.

### JD thật nên đối chiếu

Mình sẽ đối chiếu với 2-3 JD thuộc nhóm:

- AI Engineer / LLM Engineer.
- Machine Learning Engineer - LLM/RAG.
- AI Platform Engineer hoặc GenAI Engineer.

Các JD này thường nhắc đến: Python, API integration, RAG, vector database, LangChain/LangGraph hoặc framework tương tự, cloud deployment, monitoring, evaluation và security/safety.

### Bên trong - mình đã có gì?

- Đã làm ReAct Agent có retry, parser handling và tool guardrails.
- Đã làm research agent có tool routing, missing-info rule, confirmation boundary và transcript evidence.
- Đã làm RAG pipeline với chunking, hybrid retrieval, reranking, citation và abstention.
- Đã làm data quality pipeline có quality gate, schema validation, freshness check và eval.
- Đã làm deployment lab với Docker, Redis, API key auth, rate limit, cost guard, health/readiness.
- Đã làm observability lab với structured logs, PII scrubbing, tracing, metrics, alerts và dashboard.
- Đã làm evaluation benchmark với multi-judge, regression gate và failure analysis.
- Đã tham gia project RetailMix AI với frontend, backend, database, seed data, AI assistant và demo docs.

### Bên trong - mình còn thiếu gì?

- Chưa có RAG production thật trong project chính với vector database, metadata hierarchy và citation đủ mạnh.
- Chưa gắn evaluation tự động vào CI/CD cho AI assistant.
- Chưa có nhiều kinh nghiệm tối ưu latency và cost trên traffic thật.
- Chưa rõ hoàn toàn khi nào nên dùng multi-agent, khi nào single agent + tools là đủ.
- Portfolio cần được đóng gói gọn hơn để người khác xem nhanh được năng lực.

### Một câu kết role

Role này nghiêng về track **AI Application / Agentic AI Engineering**, vì nó kết hợp đúng phần mình vừa làm được: agent, RAG, evaluation, guardrails, deployment và observability.

---

## B3. Track Decision Memo

### 1. Nhìn lại Phase 1 và thị trường vừa nghiên cứu, loại công việc nào mình vừa làm được vừa muốn làm tiếp?

Mình vừa làm được và muốn làm tiếp nhóm công việc xây dựng ứng dụng AI có tính hệ thống: agent, RAG, gọi công cụ, đánh giá chất lượng, guardrails, observability và triển khai. Qua các bài lab, mình thấy mình có nhiều năng lượng nhất khi biến một bản demo AI còn mong manh thành một hệ thống có thể đo chất lượng, debug, kiểm thử và cải thiện được.

### 2. Track nào để mình đi sâu vào loại công việc đó?

Mình chọn track **AI Application / Agentic AI Engineering**. Track này phù hợp với các artifact mình đã làm trong Phase 1 như ReAct Agent, research agent có gọi công cụ, RAG pipeline, data quality pipeline, observability lab, AI evaluation benchmark và project RetailMix AI.

### 3. Bằng chứng nào cho thấy mình hợp với track này?

Mình đã có nhiều artifact liên quan trực tiếp: Day4 kéo độ chính xác tool-calling từ `0.70` lên `1.00`, Day8 RAG pipeline cá nhân pass `33 passed`, Day10 data quality eval đạt `21/21`, Day12 production readiness đạt `22/22`, Day13 observability có PII leak `0`, Day14 benchmark đạt `66/66 pass`. Các kết quả này cho thấy mình không chỉ làm prompt, mà đã chạm vào cả pipeline, độ tin cậy và đánh giá chất lượng.

### 4. Track còn lại hoặc lựa chọn khác có điểm mạnh gì, và vì sao mình chưa chọn?

Lựa chọn khác có thể là nghiêng hẳn về **Product/Frontend** hoặc **Data/Infrastructure**. Product/Frontend giúp demo dễ nhìn và gần người dùng hơn; Data/Infrastructure giúp hệ thống chắc hơn ở tầng nền. Tuy nhiên, mình chưa chọn các hướng đó làm track chính vì phần mình muốn đào sâu nhất là lớp nối giữa năng lực AI và sản phẩm thật: agent logic, retrieval, evaluation, guardrails và monitoring.

### 5. Mình còn thiếu gì để theo track đã chọn?

Mình còn cần làm sâu hơn về RAG production với vector database, metadata hierarchy, citation và reranking; cần gắn evaluation vào CI/CD; cần hiểu rõ hơn cách tối ưu latency/cost; và cần luyện thêm cách quyết định khi nào dùng multi-agent, khi nào single agent + tools là đủ.

### 6. Nếu 6 tháng nữa nhìn lại và thấy chọn chưa đúng, dấu hiệu sẽ là gì?

Dấu hiệu chọn chưa đúng là mình chỉ làm được demo bề ngoài nhưng không tạo ra artifact có benchmark, không đo được chất lượng AI, không debug được failure cases, hoặc không đưa được agent vào một flow sản phẩm chạy ổn. Nếu điều đó xảy ra, mình cần điều chỉnh lại hướng học sang phần mình thực sự tạo được giá trị rõ hơn.

### Quyết định cuối

Mình sẽ theo hướng **AI Application / Agentic AI Engineering** trong Phase 2, tập trung vào RAG, gọi công cụ, guardrails, observability và evaluation để xây dựng ứng dụng AI có thể kiểm chứng và vận hành được.
