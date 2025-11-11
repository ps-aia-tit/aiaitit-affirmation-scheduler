# aiaitit-affirmation-scheduler

# 🌅 AiaTit Affirmation Scheduler

> ** Modular. Spiritual. SaaS-aligned. **  
> A microservice to schedule and retrieve daily Sankalpa affirmations — blending backend clarity with karmic resonance.

![Java](https://img.shields.io/badge/Java-17-blue?logo=java)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-brightgreen?logo=spring)
![H2](https://img.shields.io/badge/H2-Database-blue)
![REST](https://img.shields.io/badge/REST-API-orange)
![SaaS](https://img.shields.io/badge/SaaS-Spiritual-green)
![AiaTit](https://img.shields.io/badge/AiaTit-Integration-blue)

---

## 🧭 Purpose

This Spring Boot microservice allows users to:

- Schedule daily affirmations (Sankalpas) with optional tags (e.g., clarity, career, healing)
- Retrieve today’s affirmation
- List affirmations by tag or date

Designed as a **modular SaaS component** in the AiaTit ecosystem, it reflects intentional architecture, spiritual clarity, and recruiter-facing impact.

---

## 📦 Folder Structure

```text
src/
└── main/
    └── java/com/aiatit/affirmation/
        ├── controller/
        │   └── AffirmationController.java
        ├── service/
        │   └── AffirmationService.java
        ├── model/
        │   └── Affirmation.java
        ├── repository/
        │   └── AffirmationRepository.java
        └── AffirmationSchedulerApplication.java

```

---

## 🔁 REST Endpoints

```text
POST    /affirmation/schedule
        → Schedule a new affirmation with message, tag, and date

GET     /affirmation/today
        → Retrieve today’s affirmation

GET     /affirmation/tag/{tag}
        → List affirmations by tag (e.g., clarity, career)

GET     /affirmation/date/{date}
        → Retrieve affirmation scheduled for a specific date (format: YYYY-MM-DD)

```

---

### 3. 🧪 Sample Payload


```json
{
  "message": "I act without expectation and refine without attachment.",
  "tag": "clarity",
  "scheduledDate": "2025-11-07"
}

```
---

### 4. 🚀 How to Run

```bash
mvn spring-boot:run

```

---

```markdown
curl -X POST http://localhost:8080/affirmation/schedule \
-H "Content-Type: application/json" \
-d '{"message":"I magnetize clarity through intentional action.","tag":"career","scheduledDate":"2025-11-07"}'

```

---

### 5. 🧩 Strategic Value

```markdown

- ✅ SaaS-ready: Modular, RESTful, and cloud-deployable
- 🔐 Secure messaging: Ready for integration with auth and email modules
- 🧘 Spiritual clarity: Anchors Sankalpa in backend precision
- 📄 Recruiter-facing: Markdown-stable, endpoint-documented, and badge-rich

```

---
