<div align="center">

<a href="https://github.com/RichardLirio">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&duration=3200&pause=900&color=00D8FF&center=true&vCenter=true&width=620&lines=Backend+Developer;Node.js+%C2%B7+TypeScript+%C2%B7+NestJS;REST+APIs+and+event-driven+systems;Integrations%2C+queues+and+performance" alt="Typing SVG" />
</a>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/richard-silva-lirio-b97484250)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:richardlirio@hotmail.com)
[![Profile Views](https://komarev.com/ghpvc/?username=RichardLirio&color=00D8FF&style=for-the-badge&label=PROFILE+VIEWS)](https://github.com/RichardLirio)

</div>

---

## `whoami`

Backend Developer, Vitória — Brazil. **3+ years** shipping production APIs in the JavaScript/TypeScript ecosystem.

I work on the integration layer: payment gateways, banking APIs, government SOAP endpoints, OAuth flows, message queues. The part where retries, idempotency and token lifecycles stop being interview trivia and become the reason production stays up.

```ts
const stack = {
  runtime:  ["Node.js", "TypeScript"],
  http:     ["NestJS", "Fastify", "Express"],
  data:     ["PostgreSQL", "Redis", "Prisma", "Drizzle"],
  async:    ["BullMQ", "webhooks", "streams"],
  testing:  ["Vitest", "Jest", "Testcontainers"],
  infra:    ["Docker", "AWS", "GitHub Actions", "Sentry"],
  patterns: ["Clean Architecture", "SOLID", "DDD", "TDD"],
};
```

---

## ⚙️ How I build

**Performance**
Cache-aside with Redis on read-heavy paths. Streams instead of buffering on media and file pipelines. Query tuning and index review before reaching for a bigger instance — most "we need to scale" turns out to be an N+1 and a missing index.

**Asynchronous processing**
BullMQ for anything that doesn't need to block a response: concurrency control, job deduplication, scheduled execution, exponential backoff on retries. Idempotency keys on every operation that touches money or external state, because "at least once" delivery means you *will* get called twice.

**Integrations**
Adapter pattern at every external boundary, so swapping a provider is a new class, not a refactor. OAuth 2.0 with automatic refresh-token rotation — hardcoded tokens work in Postman and break in production an hour later. Webhook-driven sync over polling wherever the vendor allows it.

**Reliability**
Structured logging with correlation IDs. Sentry on unhandled paths. Standardized error contracts so consumers don't parse strings. Timeouts on every outbound call — an external API that hangs shouldn't take your worker pool with it.

**Testing**
Unit tests with everything mocked. Integration tests against real PostgreSQL via Testcontainers, not an in-memory fake that lies about transaction behavior. E2E on the critical paths.

---

## 🧰 Stack

<table>
<tr>
<td valign="top" width="50%">

**Core**

![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=flat-square&logo=fastify&logoColor=white)
![Express](https://img.shields.io/badge/Express-404D59?style=flat-square&logo=express&logoColor=white)

**Data**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Drizzle](https://img.shields.io/badge/Drizzle-C5F74F?style=flat-square&logo=drizzle&logoColor=black)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

**Async & Messaging**

![BullMQ](https://img.shields.io/badge/BullMQ-D63384?style=flat-square&logo=redis&logoColor=white)
![Webhooks](https://img.shields.io/badge/Webhooks-000000?style=flat-square&logo=webhooks&logoColor=white)
![OAuth2](https://img.shields.io/badge/OAuth_2.0-EB5424?style=flat-square&logo=auth0&logoColor=white)

</td>
<td valign="top" width="50%">

**Testing**

![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![Testcontainers](https://img.shields.io/badge/Testcontainers-291A3F?style=flat-square&logo=docker&logoColor=white)

**Cloud & DevOps**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Frontend (when needed)**

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)

**Principles**

![Clean Architecture](https://img.shields.io/badge/Clean_Architecture-1C1C1C?style=flat-square)
![SOLID](https://img.shields.io/badge/SOLID-1C1C1C?style=flat-square)
![TDD](https://img.shields.io/badge/TDD-1C1C1C?style=flat-square)
![DDD](https://img.shields.io/badge/DDD-1C1C1C?style=flat-square)

</td>
</tr>
</table>

---

## 🔧 Shipped to production

| | Result |
|:--|:--|
| **Banking API integrations** — Sicoob, Banestes, Sicredi via C# DLLs consumed by ERP systems. Automated PIX payments and invoice generation. | `+30% operational efficiency` |
| **Municipal tax web services (NFSe)** — SOAP integrations across multiple cities in Espírito Santo. | `−50% invoice issuance time` |
| **Hshipping** — full-stack container management platform with a days-of-supply forecasting algorithm driving export decisions. | `+40% logistics planning efficiency` |
| **Workflow automation nodes** — third-party API integrations with OAuth 2.0 delegated flows and automatic token refresh. | `0 manual token rotations` |

---

## 📌 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 🚗 [techcar_mvc](https://github.com/RichardLirio/techcar_mvc)
Complete management system for auto repair shops. Customers, vehicles, parts inventory, service orders.

`TypeScript` `Fastify` `Prisma` `PostgreSQL`

</td>
<td width="50%" valign="top">

### 📧 [background_email_server](https://github.com/RichardLirio/background_email_server)
Boilerplate for high-volume batch email delivery, processed asynchronously in the background.

`TypeScript` `Queues` `Node.js`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📚 [express-boilerplate](https://github.com/RichardLirio/express-boilerplate)
Educational boilerplate covering backend fundamentals — structure, layers, and the parts tutorials skip.

`TypeScript` `Express` `Node.js`

</td>
<td width="50%" valign="top">

### 🏋️ [api_solid_GymPass](https://github.com/RichardLirio/api_solid_GymPass)
Gym check-in application applying SOLID, design patterns, JWT with refresh tokens, Dockerized DB.

`TypeScript` `SOLID` `Docker` `JWT`

</td>
</tr>
</table>

<details>
<summary><b>📓 More →</b></summary>

<br/>

- **[nest-products](https://github.com/RichardLirio/nest-products)** — Product management API with a custom missing-letter search algorithm. `NestJS`
- **[caderno](https://github.com/RichardLirio/caderno)** — My open notebook. Notes and runnable examples of whatever I'm currently learning. `TypeScript`

</details>

---

## 📊 Stats

<div align="center">

<!-- Replace YOUR-INSTANCE with your own Vercel deployment of github-readme-stats.
     The public instance is rate-limited and cannot read private repos. -->
<img height="165" src="https://YOUR-INSTANCE.vercel.app/api?username=RichardLirio&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=00000000" alt="GitHub Stats" />
<img height="165" src="https://YOUR-INSTANCE.vercel.app/api/top-langs/?username=RichardLirio&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&bg_color=00000000" alt="Top Languages" />

<br/>

<img src="https://streak-stats.demolab.com?user=RichardLirio&theme=tokyonight&hide_border=true&background=00000000" alt="GitHub Streak" />

</div>

---

<div align="center">

**Currently deep in:** distributed systems, performance profiling, advanced design patterns.

Always up for a conversation about backend architecture.

[![LinkedIn](https://img.shields.io/badge/Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/richard-silva-lirio-b97484250)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:richardlirio@hotmail.com)

</div>
