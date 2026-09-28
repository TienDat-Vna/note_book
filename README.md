# 📚 KHO TÀI LIỆU BACKEND THỰC CHIẾN (KBSV & REALTIME)

> **Cẩm nang kiến trúc và kỹ thuật Backend**: Java Core, Spring Boot, Base-Config Framework (KBSV PNS) và NestJS Realtime Microservices.

[![Java](https://img.shields.io/badge/Java-17%20%7C%2021-ED8B00?style=flat-square&logo=openjdk&logoColor=white)](https://www.oracle.com/java/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-6DB33F?style=flat-square&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![NestJS](https://img.shields.io/badge/NestJS-10.x-E0234E?style=flat-square&logo=nestjs&logoColor=white)](https://nestjs.com/)
[![Redis](https://img.shields.io/badge/Redis-Cluster-DC382D?style=flat-square&logo=redis&logoColor=white)](https://redis.io/)
[![Kafka](https://img.shields.io/badge/Kafka-Event--Driven-231F20?style=flat-square&logo=apachekafka&logoColor=white)](https://kafka.apache.org/)

---

## 🗂️ DANH MỤC TÀI LIỆU HỌC TẬP

| Chuyên Mục | File Tài Liệu | Nội Dung Trọng Tâm |
| :--- | :--- | :--- |
| **1. Java Core & Spring Boot** | [01_JAVA_CORE_SPRING_BOOT_COMPREHENSIVE_GUIDE.md](./01_JAVA_CORE_SPRING_BOOT_COMPREHENSIVE_GUIDE.md) | • **Java Core**: OOP, JVM Memory & GC, HashMap Treeify, Concurrency, Virtual Threads.<br/>• **Spring Core**: IoC/DI, Bean Lifecycle, AOP Proxy, Spring MVC, Data JPA (bẫy N+1), `@Transactional`.<br/>• **Đại từ điển Annotation**: Tra cứu 8 nhóm annotation thông dụng. |
| **2. Kiến Trúc Base & Config (KBSV PNS)** | [02_BASE_AND_CONFIG_ARCHITECTURE_ANALYSIS.md](./02_BASE_AND_CONFIG_ARCHITECTURE_ANALYSIS.md) | • **Package `base`**: Generic `BaseController`/`BaseService`, Dynamic `JPABuilder`, In-memory `LangService` $O(1)$, `BulkInsertService` (Raw JDBC).<br/>• **Package `config`**: Multi-Datasource (MySQL + Oracle Flex), Redis Cluster, Stateless Security Filter Chain. |
| **3. NestJS API Development** | [NESTJS_API_DEVELOPMENT_GUIDE.md](./NESTJS_API_DEVELOPMENT_GUIDE.md) | • **Kiến trúc Modular & Submodules**: Redis, Kafka, WebSocket Gateway.<br/>• **Quy trình 4 bước tạo API**: DTO $\rightarrow$ Service $\rightarrow$ Controller $\rightarrow$ Module.<br/>• **Kỹ thuật thực chiến**: Defensive Programming, Testing, Troubleshooting. |
| **4. Luồng Dữ Liệu API (Data Flow)** | [API_DATA_FLOW.md](./API_DATA_FLOW.md) | • **Ẩn dụ Nhà Hàng**: Client $\rightarrow$ Controller $\rightarrow$ Service $\rightarrow$ Storage $\rightarrow$ DTO.<br/>• **Sequence Diagram**: Chi tiết từng bước Request/Response trong thực tế. |
| **5. Sơ Đồ WebSocket Realtime** | [webSocket.png](./webSocket.png) | • Sơ đồ luồng Gateway kết nối WebSocket thời gian thực tới Client. |

---

## ⚡ BẢNG ĐỐI CHIẾU NHANH: SPRING BOOT vs NESTJS

| Thành Phần | Spring Boot (Java) | NestJS (TypeScript) | Vai Trò |
| :--- | :--- | :--- | :--- |
| **Dependency Injection** | `@Autowired` / Constructor Injection | `@Injectable()` Constructor Injection | Tự động tiêm phụ thuộc |
| **Controller** | `@RestController`, `@GetMapping` | `@Controller()`, `@Get()` | Tiếp nhận HTTP Request |
| **Business Logic** | `@Service` | `@Injectable()` Service | Xử lý nghiệp vụ chính |
| **Validation** | Jakarta Validation (`@NotNull`, `@Valid`) | `class-validator` (`ValidationPipe`) | Kiểm tra dữ liệu đầu vào |
| **ORM / Database** | Spring Data JPA (`JpaRepository`) | TypeORM (`Repository<T>`) | Truy vấn cơ sở dữ liệu |
| **Xác thực / Bảo vệ** | `OncePerRequestFilter`, Spring Security | `CanActivate` (Guards) | Xác thực JWT & phân quyền |
| **Xử lý Xuyên suốt** | Spring AOP (`@Aspect`) | Interceptors / Middleware | Logging, chuẩn hóa Response |
| **Bắt Lỗi Tập Trung** | `@ControllerAdvice` + `@ExceptionHandler` | `@Catch()` Exception Filters | Bắt và format lỗi API |

---

## 🎓 LỘ TRÌNH HỌC TẬP GỢI Ý

```
Tuần 1: Java Core Nâng Cao (OOP, JVM, Concurrency)
   └── File: 01_JAVA_CORE... (Phần 1)
Tuần 2: Spring Boot Architecture & Annotations (IoC, AOP, JPA, Security)
   └── File: 01_JAVA_CORE... (Phần 2 & 3)
Tuần 3: Kiến Trúc Framework Thực Tế (Base CRUD, Multi-DS, Redis Cluster)
   └── File: 02_BASE_AND_CONFIG...
Tuần 4: NestJS API & Realtime Streaming (Kafka, Redis, WebSocket)
   └── Files: NESTJS_API_DEVELOPMENT_GUIDE.md & API_DATA_FLOW.md
```

---

<div align="center">
  <sub>Tài liệu nội bộ • Repository: <b>TienDat-Vna/note_book</b></sub>
</div>
