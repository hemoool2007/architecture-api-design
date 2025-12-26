<p align="right">
  <a href="README.md">Tiếng Việt</a> | <a href="README.en.md">English</a>
</p>

# API & Backend Design (.NET)

## 🎯 Trọng tâm

Repository này tập trung vào **API & Backend Design** với các điểm chính:

* **RESTful API design:** Nguyên tắc thiết kế RESTful API hiệu quả, dễ mở rộng.
* **Idempotency:** Xử lý các request trùng lặp an toàn.
* **Pagination / filtering / sorting:** Kỹ thuật phân trang, lọc và sắp xếp dữ liệu.
* **Rate limiting:** Giới hạn tần suất request để bảo vệ server.
* **Backward compatibility:** Thiết kế API sao cho versioning và nâng cấp không phá vỡ client.

## 🛠 .NET Focus

* **ASP.NET Core Web API:** Xây dựng backend chuẩn, hiệu năng cao.
* **Model binding & validation:** Ràng buộc dữ liệu và validate input tự động.
* **Filters vs Middleware:** Khi nào dùng filter, khi nào dùng middleware.
* **Swagger / OpenAPI:** Tài liệu API tự động, dễ kiểm thử và phát triển.

## 📂 Cấu trúc repo

```
architecture-api-design-dotnet/
├── src/
│   ├── Controllers/          # API Controllers
│   ├── Models/               # DTOs & Domain Models
│   ├── Services/             # Business logic
│   ├── Middleware/           # Custom middleware
│   ├── Filters/              # Action/Exception filters
│   └── Startup.cs / Program.cs
├── tests/                    # Unit & Integration tests
├── docs/                     # API design guidelines, swagger specs
└── README.md
```

## ⚡ Best Practices

* **Versioning:** Dùng URL versioning hoặc header versioning để bảo đảm backward compatibility.
* **Idempotent endpoints:** POST/PUT cần hỗ trợ retry mà không sinh side effect.
* **Consistent error handling:** Sử dụng middleware hoặc filter để trả về lỗi chuẩn hóa.
* **Pagination & filtering:** Tránh trả tất cả dữ liệu, hỗ trợ query parameters: `?page=1&size=20&sort=createdAt`.
* **Rate limiting:** Middleware hoặc API Gateway có thể áp dụng cho từng route hoặc user/IP.
* **Swagger / OpenAPI:** Luôn generate docs từ code, giúp client và QA dễ dùng API.

## 🔗 Links tham khảo

* [ASP.NET Core Web API Documentation](https://learn.microsoft.com/en-us/aspnet/core/web-api/?view=aspnetcore-8.0)
* [REST API Design Best Practices](https://restfulapi.net/)
* [Swagger / OpenAPI](https://swagger.io/)
