<p align="right">
  <a href="README.md">Tiếng Việt</a> | <a href="README.en.md">English</a>
</p>

# API & Backend Design (.NET)

> Repository này tập trung vào **API & Backend Design** trong .NET,  
> theo góc nhìn của **Solution Architect .NET**.

---

## 🎯 Mục tiêu

- Hệ thống hóa tư duy **API & Backend** từ thiết kế đến triển khai
- Hiểu rõ:
  - API contracts, versioning, error handling
  - Modular backend, clean & hexagonal architecture
  - Event-driven / Async patterns
- Chuẩn bị phỏng vấn **Solution Architect / Senior .NET Engineer**
- Là nền tảng cho các demo backend thực tế

---

## 🧠 Phạm vi nội dung

### 1. API Design

- Contract design (DTO, request/response)
- Versioning strategy (URI, header, media-type)
- Validation & exception handling
- Idempotency / Retry patterns
- Rate limiting & throttling (conceptual)

### 2. Backend Architecture (.NET)

- Clean Architecture
- Modular Monolith
- Dependency Injection
- Service / Repository / Domain Layer
- Event-driven communication (Domain Event / Integration Event)
- Async patterns (Background Services, Message Queue)

### 3. Data & Storage

- Database modeling (relational & NoSQL)
- Migrations & versioning
- Caching strategies (Memory, Redis)
- Transaction / Consistency patterns (Unit of Work, Saga)

### 4. Security & Auth

- Authentication / Authorization
- JWT, OAuth2
- Claims-based / Role-based access
- Securing API endpoints

### 5. Observability

- Logging, metrics, tracing
- Health checks
- Exception monitoring
- Correlation IDs

---

## 🧪 Demo & Labs

Các demo minh họa:

- Modular Monolith API sample (ASP.NET Core)
- API Versioning demo
- Async messaging & domain events
- Error handling & logging
- Secure endpoints & auth demo

> Các demo lớn được tách thành các repository riêng trong folder `demos/`.

---

## 📐 Documentation-first Approach

- **Documentation → Design → Implementation**
- Mỗi demo có **docs đi kèm**
- ADR ghi lại **trade-off và quyết định**
- Code là **kết quả cuối cùng**, không phải tutorial

---

## 📌 Định hướng sử dụng

- Ôn tập kiến thức API & Backend Design
- Chuẩn bị phỏng vấn Solution Architect / Senior Engineer
- Tham khảo cho các project thực tế
- Là cơ sở để phát triển các repo backend khác

---

## 🔗 Cấu trúc đề xuất

```
api-backend-design-dotnet/
│
├── README.md
├── README.en.md
│
├── docs/
│   ├── architecture/
│   │   ├── context-diagram.md
│   │   ├── container-diagram.md
│   │   ├── component-diagram.md
│   │   └── decision-records/
│   │       └── ADR-001-api-design.md
│   │
│   ├── api-guidelines.md
│   └── backend-principles.md
│
├── demos/
│   ├── modular-monolith/
│   ├── api-versioning/
│   ├── async-messaging/
│   └── auth-secure-demo/
```

---

## ✅ Trạng thái hiện tại

- [x] API & Backend Design overview
- [x] Demo folder structure
- [ ] ADR & trade-off notes
- [ ] C4 diagrams cho backend
