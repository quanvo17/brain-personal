---
type: Note
---
# Context Platform

***Active metadata trả lời:*** *“Dữ liệu này là gì, từ đâu đến, ai sở hữu, chất lượng thế nào và thay đổi gì?”*
***AI Context Platform phải trả lời thêm:*** *“Đối với* *người/agent này**, thực hiện* *nhiệm vụ này**, tại* *thời điểm này**, được phép biết gì, nên tin gì, cần truy xuất ngữ cảnh nào, có thể gọi công cụ nào, và bằng chứng nào phải đi kèm kết quả?”*


- Context phải gắn với **classification, consent/purpose, residency, entitlement, lineage, audit và policy enforcement**.
- Active Metadata → Gartner nhấn mạnh việc sử dụng metadata để tự động hóa data-management tasks và biến passive metadata thành metadata có khả năng **kích hoạt hành động**; tiêu chí thị trường hiện nay còn bao gồm orchestration hai chiều, tức metadata được enrich rồi đưa trở lại các hệ thống vận hành. 
  - *Hành động ở đây tức là* *hệ thống sử dụng để phát hiện sự kiện, đánh giá quy tắc và tự động thực hiện một tác vụ quản trị dữ liệu cụ thể. Các nhóm hành động cụ thể*
    - Data Classification: Tự động gắn nhãn PII, Confidential, Public; đề xuất mức độ nhạy cảm
    - Data Quality: Chạy kiểm tra chất lượng, tạo incident, cảnh báo Data Steward, cách ly dữ liệu lỗi
    - Data Lineage & Impact Analysis: Phân tích tác động khi schema thay đổi, thông báo các nhóm bị ảnh hưởng, chặn triển khai có rủi ro
    - Security & Access Control: Tạo yêu cầu phê duyệt, đồng bộ policy, thu hồi quyền hết hạn, áp dụng masking
    - Data Governance Workflow: Tạo nhiệm vụ xác nhận định nghĩa, yêu cầu phê duyệt, chuyển việc đến đúng người phụ trách
    - Data Pipeline Operations: Cảnh báo dữ liệu trễ, kích hoạt chạy lại pipeline, tạm dừng downstream job
    - Data Lifecycle Management: Đề xuất hoặc thực thi lưu trữ, xóa, archive dữ liệu theo chính sách
    - Data Discovery & Consumption: Cập nhật trạng thái certified, đề xuất bộ dữ liệu phù hợp, cảnh báo người dùng về dữ liệu không đáng tin cậy
  - Link tham khảo: [https://www.gartner.com/en/documents/6617902](https://www.gartner.com/en/documents/6617902)
- Metadata nói chung là "data about data" (DMBOOK) mô tả cấu trúc, nguồn gốc, định dạng, ý nghĩa, quyền sở hữu và các đặc tính của tài sản dữ liệu. Phân loại:
  - Business Metadata: Mô tả ý nghĩa, định nghĩa và quy tắc sử dụng dữ liệu dưới góc độ nghiệp vụ.
  - Technical Metadata: Mô tả cấu trúc, định dạng, đặc điểm kỹ thuật và quan hệ giữa các tài sản dữ liệu
  - Operational Metadata: Mô tả quá trình xử lý, vận hành và sử dụng dữ liệu.
- Tài sản dữ liệu → định nghĩa và phân loại
- AI Context Platform là lớp hạ tầng có quản trị dùng để xây dựng, liên kết, đánh giá, truy xuất và phân phối context phù hợp cho AI application/agent tại runtime, dựa trên metadata, semantics, enterprise knowledge, policy, identity, task state, history, model/tool information và feedback. 
  - Các lớp context cần quản lý:
    - Technical context: schema, type, SQL, pipeline, lineage, quality
    - Business context: glossary, metric, KPI, domain, policy, data product
    - Knowledge context: SOP, policies, FAQ, decision log, contracts, product docs
    - Operational context: freshness, incidents, SLA, usage, active alert
    - AI context: model version, prompt, tool, agent, eval, trace, guardrail
    - Execution context: user, purpose, task, entitlements, conversation state
