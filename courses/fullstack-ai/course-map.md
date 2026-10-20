# Full-Stack AI Engineer (.NET) Course Map <!-- omit in toc -->

This map records where every part of the [Full-Stack AI Engineer (.NET)](README.md) course comes from. Mentors use it to review the course, to calibrate its workload, and to apply upstream changes from the bootcamp to the right step (see [ATTRIBUTION.md](ATTRIBUTION.md)).

Sources:

- The [C# course](../csharp/README.md) of this repository, based on [Programming C# 12.0](https://www.oreilly.com/library/view/programming-c-12/9781098158354/).
- The [CrystaCode Full-Stack AI Bootcamp](https://github.com/CrystaCode/full-stack-ai-bootcamp) at commit [`2f4c677`](https://github.com/CrystaCode/full-stack-ai-bootcamp/tree/2f4c6772d73200b92b54bfad65609e5df16b7368) (2026-09-22), MIT License.

Bootcamp tasks are written as `NN-Tm`: task *m* of bootcamp step *NN*. A task split across two steps ends in `-a` or `-b`. The same identifiers appear as invisible markers (`<!-- bc: NN-Tm -->` and `<!-- outcomes: ... -->`) in the step files.

## Contents <!-- omit in toc -->

- [Steps](#steps)
- [Bootcamp Outcomes](#bootcamp-outcomes)
- [C# Course Steps](#c-course-steps)
- [Adaptation Log](#adaptation-log)
- [Workload](#workload)

## Steps

C# chapters are ordered by what each step's web and AI work needs: lambdas (ch. 9) and an async/await introduction come before the first Minimal API and middleware, exceptions (ch. 8) sit beside API error handling, object lifetime (ch. 7) comes before dependency-injection lifetimes, LINQ and async (ch. 10, 16–17) come before EF Core, and nullable reference types sit beside EF Core. Bootcamp work that needs no C# (AI literacy, HTML, CSS) fills Steps 1–3, so ASP.NET Core starts only after inheritance.

Program tasks follow the step number, exactly as in the C#, Web, and Machine Learning courses. Every step also ends with the technical session, the scheduling task, and the LinkedIn live presentation.

| Step | C# source | Bootcamp study items (upstream step) | Bootcamp tasks | Program tasks |
|---|---|---|---|---|
| [Step 1](01-Introduction-AI-Foundations.md): Introduction, AI Foundations, and HTML | Step 1 (ch. 1–2, intro tutorials, Git) | General AI (01); Frontend (01) | `01-T1` Create an AI Foundations Pack; `01-T2-a` Start the Portfolio Application (Part A) | Mentor Training: Communication 3, 4; TypingClub 88 |
| [Step 2](02-Types-Generics-Learning-With-AI.md): Types, Generics, and Learning with AI | Steps 2–3 (ch. 3–4, debugging) | General AI (03) | `03-T1` Produce a Source-Grounded Feature Brief | Mentor Training: Communication 5, 6; TypingClub 137 |
| [Step 3](03-Collections-Inheritance-Content.md): Collections, Inheritance, and Verified Content | Steps 4–5 (ch. 5–6) | General AI (06); Frontend (02) | `06-T1` Produce a Verified Content Pack; `02-T2-a` Add a Styled Minimal API Slice (Part A) | Mentor Training: Communication 7, 8; TypingClub 202; TA Level 1 |
| [Step 4](04-Delegates-Lambdas-Web-API.md): Delegates, Lambdas, and the First Web API | Step 8 (ch. 9); Step 10 async/await article | General AI (02); ASP.NET Core (01, 02) | `01-T2-b` Start the Portfolio Application (Part B); `02-T1` Build a Source-Grounded Prompt and Assistant Lab; `02-T2-b` Add a Styled Minimal API Slice (Part B) | Mentor Training: Coaching 1, 2; TypingClub 244 |
| [Step 5](05-Object-Lifetime-Exceptions-Blazor.md): Object Lifetime, Exceptions, and the First Blazor App | Steps 6–7 (ch. 7–8); Step 8 events article | General AI (07); ASP.NET Core (03); Frontend (03); Blazor (03) | `07-T1` Create a Reviewed Product Visual; `03-T2` Build a Navigable and Validated Product Shell | Onboarding; Mentor Training: Coaching 3, 4; TypingClub 285 |
| [Step 6](06-LINQ-Async-Components.md): LINQ, Asynchronous Programming, and Component Architecture | Steps 9–10 (ch. 10, 16–17) | General AI (04); ASP.NET Core (04); Frontend (04); Blazor (04) | `04-T1` Build and Evaluate a Prompt Tool; `04-T2` Create the Configurable Component Shell | Mentor Training: Coaching 5, 6; TypingClub 316; TA Level 2 |
| [Step 7](07-Modern-CSharp-Persistence.md): Modern C# and Persistent Applications | Step 11 (C# 14, nullable reference types) | General AI (05); ASP.NET Core (05); Frontend (05); Blazor (05) | `05-T1` Specify and Test a Bounded AI Loop; `05-T2` Build the Persistent Responsive Feature | Mentor Training: Coaching 7, 8; TypingClub 357 |
| [Step 8](08-Controllers-Rendering-Identity.md): Controllers, Rendering, Identity, and Navigation | None | ASP.NET Core (06, 07); Blazor (06, 07) | `06-T2` Build an Efficient Content Management Slice; `07-T2` Build a Secured Navigable Experience | Mentor Training: Coaching 9, 10; TypingClub 374 |
| [Step 9](09-Forms-Observability-First-AI-Feature.md): Forms, Observability, and the First AI Feature | None | General AI (08); ASP.NET Core (08); Blazor (08); .NET AI (08) | `08-T1` Present the Product Story; `08-T2` Build a Validated and Observable Editing Flow; `08-T3` Add the First AI Capability | Mentor Training: Coaching 11, 12; TypingClub 388; TA Level 3 |
| [Step 10](10-Agent-Assisted-Integration.md): Agent-Assisted Integration | None | General AI (09); ASP.NET Core (09); Blazor (09); .NET AI (09) | `09-T1` Establish the Agent Development Contract; `09-T2` Build the Integration Feature; `09-T3` Run the First Product Agent | TypingClub 418 |
| [Step 11](11-Reliable-Automated-Workflows.md): Reliable and Automated Workflows | None | General AI (10); ASP.NET Core (10); Blazor (10); .NET AI (10) | `10-T1` Build a Recoverable AI Workflow; `10-T2` Build the Reliability Suite; `10-T3` Compare AI-Assisted IDE Workflows | TypingClub 429 |
| [Step 12](12-Agent-Tools-Skills-Coordination.md): Agent Tools, Skills, and Coordination | None | .NET AI (11) | `11-T1` Give the Product Agent Tools; `11-T2` Package a Reusable Agent Skill; `11-T3` Coordinate a Multi-Agent Workflow | None |
| [Step 13](13-Production-AI-Applications.md): Production AI Applications | None | General AI (12); ASP.NET Core (12); Blazor (12); .NET AI (12) | `12-T1` Approve the Production AI Architecture; `12-T2` Orchestrate and Harden the Application; `12-T3` Add the Generative Interface | None |
| [Step 14](14-Integrated-Capstone.md): Integrated Capstone | None | Capstone Review (13) | `13-T1` Complete the Capstone Release; `13-T2` Assemble the Evidence Portfolio; `13-T3` Demonstrate and Defend the Product | None |

## Bootcamp Outcomes

Every outcome of the bootcamp's [coverage map](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/design/course-map.md) has exactly one primary step in this course.

### General AI

| Source ID | Source outcome | Bootcamp step | Full-Stack AI Engineer (.NET) step |
|---|---|---|---|
| `AI-01` | Explain generative AI capabilities, limitations, applications, and human-controlled decisions | [Step 01](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-01.md) | [Step 1](01-Introduction-AI-Foundations.md) |
| `AI-02` | Explain how large language models generate responses | [Step 01](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-01.md) | [Step 1](01-Introduction-AI-Foundations.md) |
| `AI-03` | Recognize hallucinations, verify important model outputs, and retain human accountability | [Step 01](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-01.md) | [Step 1](01-Introduction-AI-Foundations.md) |
| `AI-04` | Compare integrated browser assistants on source-grounded work | [Step 02](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-02.md) | [Step 4](04-Delegates-Lambdas-Web-API.md) |
| `AI-05` | Use Gemini features for learning and productivity | [Step 03](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-03.md) | [Step 2](02-Types-Generics-Learning-With-AI.md) |
| `AI-06` | Conduct and evaluate a guided Study Mode session | [Step 03](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-03.md) | [Step 2](02-Types-Generics-Learning-With-AI.md) |
| `AI-07` | Build and verify a source-grounded notebook | [Step 03](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-03.md) | [Step 2](02-Types-Generics-Learning-With-AI.md) |
| `AI-08` | Compare deep-research tools and evidence quality | [Step 03](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-03.md) | [Step 2](02-Types-Generics-Learning-With-AI.md) |
| `AI-09` | Apply and evaluate prompt-engineering principles | [Step 02](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-02.md) | [Step 4](04-Delegates-Lambdas-Web-API.md) |
| `AI-10` | Build and review a prompt-based application | [Step 04](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-04.md) | [Step 6](06-LINQ-Async-Components.md) |
| `AI-11` | Build and evaluate a reusable context pack | [Step 04](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-04.md) | [Step 6](06-LINQ-Async-Components.md) |
| `AI-12` | Design and test a bounded AI loop | [Step 05](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-05.md) | [Step 7](07-Modern-CSharp-Persistence.md) |
| `AI-13` | Transform a verified brief for multiple audiences | [Step 06](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-06.md) | [Step 3](03-Collections-Inheritance-Content.md) |
| `AI-14` | Generate, compare, and select image variations for a communication goal | [Step 07](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-07.md) | [Step 5](05-Object-Lifetime-Exceptions-Blazor.md) |
| `AI-15` | Create and rehearse a source-grounded presentation | [Step 08](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-08.md) | [Step 9](09-Forms-Observability-First-AI-Feature.md) |
| `AI-16` | Use GitHub Copilot in VS Code with review and verification | [Step 08](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-08.md) | [Step 9](09-Forms-Observability-First-AI-Feature.md) |
| `AI-17` | Build a bounded feature with agent mode | [Step 09](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-09.md) | [Step 10](10-Agent-Assisted-Integration.md) |
| `AI-18` | Add and evaluate persistent repository context | [Step 09](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-09.md) | [Step 10](10-Agent-Assisted-Integration.md) |
| `AI-19` | Use and compare GitHub Copilot in Visual Studio | [Step 10](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-10.md) | [Step 11](11-Reliable-Automated-Workflows.md) |
| `AI-20` | Map appropriate AI opportunities for an application | [Step 12](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-12.md) | [Step 13](13-Production-AI-Applications.md) |
| `AI-21` | Produce an integrated AI portfolio project | [Step 13](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-13.md) | [Step 14](14-Integrated-Capstone.md) |

### ASP.NET Core

| Source ID | Source outcome | Bootcamp step | Full-Stack AI Engineer (.NET) step |
|---|---|---|---|
| `API-01` | Get started with ASP.NET Core | [Step 01](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-01.md) | [Step 4](04-Delegates-Lambdas-Web-API.md) |
| `API-02` | Explain ASP.NET Core and build a first application | [Step 01](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-01.md) | [Step 4](04-Delegates-Lambdas-Web-API.md) |
| `API-03` | Handle requests with the middleware pipeline | [Step 02](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-02.md) | [Step 4](04-Delegates-Lambdas-Web-API.md) |
| `API-04` | Create a JSON API with Minimal APIs | [Step 02](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-02.md) | [Step 4](04-Delegates-Lambdas-Web-API.md) |
| `API-05` | Map URLs to endpoints with routing | [Step 03](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-03.md) | [Step 5](05-Object-Lifetime-Exceptions-Blazor.md) |
| `API-06` | Apply model binding and validation | [Step 03](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-03.md) | [Step 5](05-Object-Lifetime-Exceptions-Blazor.md) |
| `API-07` | Use dependency injection | [Step 04](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-04.md) | [Step 6](06-LINQ-Async-Components.md) |
| `API-08` | Configure an ASP.NET Core application | [Step 04](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-04.md) | [Step 6](06-LINQ-Async-Components.md) |
| `API-09` | Document APIs with OpenAPI | [Step 05](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-05.md) | [Step 7](07-Modern-CSharp-Persistence.md) |
| `API-10` | Persist relational data with EF Core and SQL | [Step 05](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-05.md) | [Step 7](07-Modern-CSharp-Persistence.md) |
| `API-11` | Build HTTP APIs with controllers | [Step 06](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-06.md) | [Step 8](08-Controllers-Rendering-Identity.md) |
| `API-12` | Apply endpoint or action filters | [Step 06](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-06.md) | [Step 8](08-Controllers-Rendering-Identity.md) |
| `API-13` | Implement authentication and authorization | [Step 07](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-07.md) | [Step 8](08-Controllers-Rendering-Identity.md) |
| `API-14` | Monitor and troubleshoot with logging | [Step 08](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-08.md) | [Step 9](09-Forms-Observability-First-AI-Feature.md) |
| `API-15` | Publish and deploy an application | [Step 12](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-12.md) | [Step 13](13-Production-AI-Applications.md) |
| `API-16` | Apply HTTPS and security hardening | [Step 12](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-12.md) | [Step 13](13-Production-AI-Applications.md) |
| `API-17` | Call remote APIs and map objects | [Step 09](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-09.md) | [Step 10](10-Agent-Assisted-Integration.md) |
| `API-18` | Build background tasks and services | [Step 10](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-10.md) | [Step 11](11-Reliable-Automated-Workflows.md) |
| `API-19` | Test ASP.NET Core applications | [Step 10](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-10.md) | [Step 11](11-Reliable-Automated-Workflows.md) |
| `API-20` | Orchestrate services with .NET Aspire | [Step 12](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-12.md) | [Step 13](13-Production-AI-Applications.md) |

### Frontend

| Source ID | Source outcome | Bootcamp step | Full-Stack AI Engineer (.NET) step |
|---|---|---|---|
| `WEB-01` | Use HTML basics and semantic markup | [Step 01](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-01.md) | [Step 1](01-Introduction-AI-Foundations.md) |
| `WEB-02` | Apply CSS selectors, properties, and the box model | [Step 02](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-02.md) | [Step 3](03-Collections-Inheritance-Content.md) |
| `WEB-03` | Build layouts with Flexbox and Grid | [Step 03](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-03.md) | [Step 5](05-Object-Lifetime-Exceptions-Blazor.md) |
| `WEB-04` | Use positioning, transitions, and animations | [Step 04](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-04.md) | [Step 6](06-LINQ-Async-Components.md) |
| `WEB-05` | Implement responsive web design | [Step 05](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-05.md) | [Step 7](07-Modern-CSharp-Persistence.md) |

### Blazor

| Source ID | Source outcome | Bootcamp step | Full-Stack AI Engineer (.NET) step |
|---|---|---|---|
| `BLAZOR-01` | Explain current Blazor hosting and render modes | [Step 03](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-03.md) | [Step 5](05-Object-Lifetime-Exceptions-Blazor.md) |
| `BLAZOR-02` | Create Blazor projects and pages | [Step 03](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-03.md) | [Step 5](05-Object-Lifetime-Exceptions-Blazor.md) |
| `BLAZOR-03` | Build layouts and nested layouts | [Step 04](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-04.md) | [Step 6](06-LINQ-Async-Components.md) |
| `BLAZOR-04` | Build components with data binding | [Step 04](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-04.md) | [Step 6](06-LINQ-Async-Components.md) |
| `BLAZOR-05` | Handle component and DOM events | [Step 05](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-05.md) | [Step 7](07-Modern-CSharp-Persistence.md) |
| `BLAZOR-06` | Use cascading values and captured attributes | [Step 05](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-05.md) | [Step 7](07-Modern-CSharp-Persistence.md) |
| `BLAZOR-07` | Explain component lifecycles and rendering synchronization | [Step 06](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-06.md) | [Step 8](08-Controllers-Rendering-Identity.md) |
| `BLAZOR-08` | Analyze render trees and optimize with keys | [Step 06](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-06.md) | [Step 8](08-Controllers-Rendering-Identity.md) |
| `BLAZOR-09` | Build templated and generic components | [Step 07](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-07.md) | [Step 8](08-Controllers-Rendering-Identity.md) |
| `BLAZOR-10` | Define routes and route parameters | [Step 07](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-07.md) | [Step 8](08-Controllers-Rendering-Identity.md) |
| `BLAZOR-11` | Implement navigation and navigation events | [Step 07](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-07.md) | [Step 8](08-Controllers-Rendering-Identity.md) |
| `BLAZOR-12` | Build forms for editing data | [Step 08](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-08.md) | [Step 9](09-Forms-Observability-First-AI-Feature.md) |
| `BLAZOR-13` | Apply standard and custom validation | [Step 08](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-08.md) | [Step 9](09-Forms-Observability-First-AI-Feature.md) |
| `BLAZOR-14` | Manage form state with EditContext | [Step 08](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-08.md) | [Step 9](09-Forms-Observability-First-AI-Feature.md) |
| `BLAZOR-15` | Call .NET from JavaScript | [Step 09](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-09.md) | [Step 10](10-Agent-Assisted-Integration.md) |
| `BLAZOR-16` | Call JavaScript from .NET | [Step 09](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-09.md) | [Step 10](10-Agent-Assisted-Integration.md) |
| `BLAZOR-17` | Inject dependencies into components | [Step 10](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-10.md) | [Step 11](11-Reliable-Automated-Workflows.md) |
| `BLAZOR-18` | Apply component scopes and dependency lifetimes | [Step 10](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-10.md) | [Step 11](11-Reliable-Automated-Workflows.md) |
| `BLAZOR-19` | Evaluate production and cross-platform architecture | [Step 12](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-12.md) | [Step 13](13-Production-AI-Applications.md) |

### .NET AI

| Source ID | Source outcome | Bootcamp step | Full-Stack AI Engineer (.NET) step |
|---|---|---|---|
| `DOTNET-AI-01` | Add GenAI to a .NET app with Microsoft Extensions AI | [Step 08](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-08.md) | [Step 9](09-Forms-Observability-First-AI-Feature.md) |
| `DOTNET-AI-02` | Understand the Microsoft Agent Framework landscape | [Step 09](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-09.md) | [Step 10](10-Agent-Assisted-Integration.md) |
| `DOTNET-AI-03` | Create a first agent in C# | [Step 09](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-09.md) | [Step 10](10-Agent-Assisted-Integration.md) |
| `DOTNET-AI-04` | Persist state, configure settings and memory, and apply middleware | [Step 10](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-10.md) | [Step 11](11-Reliable-Automated-Workflows.md) |
| `DOTNET-AI-05` | Call controlled tools from an agent | [Step 11](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-11.md) | [Step 12](12-Agent-Tools-Skills-Coordination.md) |
| `DOTNET-AI-06` | Package capabilities with the current Agent Skills provider | [Step 11](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-11.md) | [Step 12](12-Agent-Tools-Skills-Coordination.md) |
| `DOTNET-AI-07` | Coordinate multi-agent systems | [Step 11](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-11.md) | [Step 12](12-Agent-Tools-Skills-Coordination.md) |
| `DOTNET-AI-08` | Build Agent Framework workflows | [Step 10](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-10.md) | [Step 11](11-Reliable-Automated-Workflows.md) |
| `DOTNET-AI-09` | Explain reasoning-model tradeoffs and distinguish private reasoning from auditable runtime evidence | [Step 11](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-11.md) | [Step 12](12-Agent-Tools-Skills-Coordination.md) |
| `DOTNET-AI-10` | Build generative UI and use agent protocols | [Step 12](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-12.md) | [Step 13](13-Production-AI-Applications.md) |
| `DOTNET-AI-11` | Review the date-pinned current Agent Framework package and release status | [Step 12](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-12.md) | [Step 13](13-Production-AI-Applications.md) |

### Reinforcement

These outcomes are covered earlier and deliberately re-evaluated against the finished capstone.

| Source ID | Bootcamp step | Full-Stack AI Engineer (.NET) step | Evidence |
|---|---|---|---|
| `AI-03` | [Step 13](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-13.md) | [Step 14](14-Integrated-Capstone.md) | Final hallucination checks, verification evidence, corrections, and human decision record |
| `AI-20` | [Step 13](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-13.md) | [Step 14](14-Integrated-Capstone.md) | Updated AI opportunity and fallback review |
| `API-16` | [Step 13](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-13.md) | [Step 14](14-Integrated-Capstone.md) | Capstone security and secret checks |
| `API-19` | [Step 13](https://github.com/CrystaCode/full-stack-ai-bootcamp/blob/2f4c6772d73200b92b54bfad65609e5df16b7368/course/step-13.md) | [Step 14](14-Integrated-Capstone.md) | Final critical-journey test evidence |

## C# Course Steps

Mentor Training, TypingClub, Technical Assistant, and onboarding tasks follow the step number, so they are not carried with the content below.

| C# step | Full-Stack AI Engineer (.NET) step | Notes |
|---|---|---|
| [1. Introduction](../csharp/01-Introduction.md) | [Step 1](01-Introduction-AI-Foundations.md) | The two AI videos (Kniberg, Berman) are removed because they are the AI-01 and AI-02 resources of the same step. |
| [2. Types](../csharp/02-Types.md) | [Step 2](02-Types-Generics-Learning-With-AI.md) | The Karpathy video is removed because it is the AI-02 and AI-03 resource in Step 1. The two YouTube debugging videos are optional. |
| [3. Generics](../csharp/03-Generics.md) | [Step 2](02-Types-Generics-Learning-With-AI.md) | The Sanderson video is removed because it is the AI-20 resource in Step 13 and is reviewed again in Step 14. |
| [4. Collections](../csharp/04-Collections.md) | [Step 3](03-Collections-Inheritance-Content.md) | The DeepLearning.AI prompt-engineering course moves to Step 6 as an optional resource beside AI-10, whose verbs (summarize, infer, transform, expand) it teaches. |
| [5. Inheritance](../csharp/05-Inheritance.md) | [Step 3](03-Collections-Inheritance-Content.md) | The Stack Overflow question on generics in C#, Java, and C++ is removed because it repeats the Microsoft article on C++ templates in Step 2. |
| [6. Object Lifetime](../csharp/06-Object-LifeTime.md) | [Step 5](05-Object-Lifetime-Exceptions-Blazor.md) | "All sublinks" of the garbage collection guide is narrowed to three named pages. |
| [7. Exceptions](../csharp/07-Exceptions.md) | [Step 5](05-Object-Lifetime-Exceptions-Blazor.md) | The checked-or-unchecked article now uses its canonical https address. |
| [8. Delegates, Lambdas and Events](../csharp/08-Delegates-Lambdas-Events.md) | [Step 4](04-Delegates-Lambdas-Web-API.md); events article in [Step 5](05-Object-Lifetime-Exceptions-Blazor.md) | The chapter moves before the first Minimal API. The article on memory leaks through events moves to Step 5, after the garbage collection material it relies on. |
| [9. LINQ](../csharp/09-LINQ.md) | [Step 6](06-LINQ-Async-Components.md) | "LinqPad exercises" becomes the [Working with LINQ](https://learn.microsoft.com/en-us/dotnet/csharp/tutorials/working-with-linq) tutorial, with LINQPad optional. |
| [10. Asynchronous Language Features](../csharp/10-Asynchronous-Language-Features.md) | async/await article in [Step 4](04-Delegates-Lambdas-Web-API.md); the rest in [Step 6](06-LINQ-Async-Components.md) | The "Improve App Responsiveness" video moves from Tasks to Study Items. |
| [11. C# New Features](../csharp/11-C%23-New-Features.md) | [Step 7](07-Modern-CSharp-Persistence.md) | The C# 13 article and video are replaced by "What's new in C# 14", the version that ships with .NET 10, which the bootcamp resources target. Tasks that said "C# 8.0" now name nullable reference types directly. |

## Adaptation Log

### Bootcamp

- **Kept verbatim:** study items, resource links, `(Optional)` labels, task titles, goals, deliverables, requirements, acceptance criteria, and Submission bullets, except for the changes listed here.
- **Sections:** each step keeps the program's Study Items and Tasks format. The bootcamp's Outcomes, Completion Criteria, Source Outcomes, and Navigation sections are dropped; source outcomes live in this map and in the step markers. Each Submission bullet moves into the task it belongs to, and the generic "link to the step commit" bullet moves to the [README](README.md#how-the-course-works).
- **Step introductions:** Steps 1–8 have introductions written for this course. Steps 9–14 use the bootcamp's step descriptions.
- **Wording changes** (each applied exactly once):
  - `02-T1`, `03-T1`: "an instructor-approved equivalent" → "a technical mentor-approved equivalent".
  - `02-T1`: "one non-video Frontend reading linked in this step" → "one non-video Frontend reading linked in Step 3 (CSS Tutorial or CSS Reference)", because the CSS readings now sit in Step 3.
  - `02-T1` acceptance criterion: "used in Task 2" → "used in the *Add a Styled Minimal API Slice (Part B)* task".
  - `02-T2`: "the verified trace from Task 1" → "the verified trace from the *Build a Source-Grounded Prompt and Assistant Lab* task".
  - Bootcamp Step 13, study item 1: the relative link `../design/flows/flow-ai-general.md` → the same file at commit `2f4c677`.
  - `13-T2` acceptance criterion: "in the coverage map" → "in the [course coverage map](course-map.md)".
- **Split tasks:** each requirement, acceptance criterion, and Submission bullet moves with its part.
  - `01-T2-a` (Step 1): product domain and semantic HTML page. Deliverable: "A repository containing a semantic HTML product page." The goal is unchanged.
  - `01-T2-b` (Step 4): ASP.NET Core application, information endpoint, and README run instructions. Goal: "Complete the first vertical slice of the product with a running backend." Deliverable: "A running ASP.NET Core application and an information endpoint in the portfolio repository."
  - `02-T2-a` (Step 3): stylesheet. Goal: "Introduce visual styling in the portfolio application." Deliverable: "A styled product page."
  - `02-T2-b` (Step 4): middleware and Minimal API. Goal: "Introduce request processing and JSON behavior in the portfolio application." Deliverable: "Custom request-logging middleware with a predicted-versus-observed trace and in-memory Minimal API endpoints for one product resource."
  - Three Submission bullets that covered both parts of a split are divided between the parts (Bootcamp Step 1 bullet 3, Step 2 bullet 3, and Step 3 bullet 1, whose "hosting decision" belongs to `03-T2`).
- **Moved tasks:** `03-T1` (Step 2), `06-T1` (Step 3), and `07-T1` (Step 5) need no C#, so they fill the early steps. `06-T1` uses the verified brief that `03-T1` produces.
- **Added note:** `03-T1` carries a marked *Tip* suggesting the step's C# topic as the Study Mode learning goal. Its requirements are unchanged.
- **Positional phrases checked and left unchanged:** "article assigned in this step" and "another non-video reading linked in this step" (`02-T1`, still in the same step), "existing API error conventions" (`06-T2`, Step 8, after Steps 4–5), "already created during the course" (`08-T1`), "approval path defined earlier" (`11-T1`), and "built in the previous step" (`11-T3`, `12-T3`). Steps 9–14 map one-to-one to bootcamp Steps 8–13, so these phrases keep their meaning.

### C# Course

- **Kept verbatim:** study items, exercism lists, mini-projects, and research tasks, except for the changes listed in [C# Course Steps](#c-course-steps) and these fixes:
  - Step 1: "Join C# track in **practice mode**:" ends with a period, and "Gigaseconds" is spelled "Gigasecond", as on exercism.
  - Step 3: "Pass these at exercism.io" becomes "Pass these exercises at exercism.io" (merged into Step 2's list).
  - Step 4: "chapter 5: Collections" gets the same spacing as the other chapters.
  - Step 5: the animal-hierarchy project drops its inline `<br>` and "Project Description:" label; its description bullets are unchanged.
- **Merged lists:** exercism lists of C# steps that share a combined step are merged into one task.
- **Boilerplate:** the closing tasks are copied from the C# course. The only change is the "For more details" line, which is now indented under its task.

## Workload

The self-learning stage is about 9 months at 25–30 hours a week, which leaves roughly 70 hours per step for 14 steps. Use these counts to calibrate deadlines and to spot overloaded steps. Chapters count *Programming C# 12.0* and *ASP.NET Core in Action* chapters.

| Step | C# study items | AI and web study items | Book chapters | Exercism exercises | C# projects | Bootcamp tasks | Acceptance criteria | All tasks |
|---|---|---|---|---|---|---|---|---|
| [Step 1](01-Introduction-AI-Foundations.md) | 6 | 4 (0 optional) | 2 | 5 | 0 | 2 | 7 | 14 |
| [Step 2](02-Types-Generics-Learning-With-AI.md) | 10 | 4 (0 optional) | 2 | 5 | 2 | 1 | 5 | 12 |
| [Step 3](03-Collections-Inheritance-Content.md) | 5 | 2 (0 optional) | 2 | 5 | 2 | 2 | 5 | 13 |
| [Step 4](04-Delegates-Lambdas-Web-API.md) | 2 | 6 (0 optional) | 6 | 0 | 0 | 3 | 12 | 9 |
| [Step 5](05-Object-Lifetime-Exceptions-Blazor.md) | 9 | 6 (0 optional) | 5 | 0 | 0 | 2 | 7 | 10 |
| [Step 6](06-LINQ-Async-Components.md) | 6 | 8 (1 optional) | 6 | 1 | 0 | 2 | 7 | 11 |
| [Step 7](07-Modern-CSharp-Persistence.md) | 5 | 6 (0 optional) | 2 | 0 | 0 | 2 | 8 | 13 |
| [Step 8](08-Controllers-Rendering-Identity.md) | 0 | 8 (0 optional) | 6 | 0 | 0 | 2 | 8 | 8 |
| [Step 9](09-Forms-Observability-First-AI-Feature.md) | 0 | 10 (1 optional) | 1 | 0 | 0 | 3 | 11 | 10 |
| [Step 10](10-Agent-Assisted-Integration.md) | 0 | 11 (3 optional) | 1 | 0 | 0 | 3 | 12 | 7 |
| [Step 11](11-Reliable-Automated-Workflows.md) | 0 | 12 (2 optional) | 3 | 0 | 0 | 3 | 11 | 7 |
| [Step 12](12-Agent-Tools-Skills-Coordination.md) | 0 | 7 (0 optional) | 0 | 0 | 0 | 3 | 11 | 6 |
| [Step 13](13-Production-AI-Applications.md) | 0 | 10 (0 optional) | 3 | 0 | 0 | 3 | 13 | 6 |
| [Step 14](14-Integrated-Capstone.md) | 0 | 4 (0 optional) | 0 | 0 | 0 | 3 | 12 | 6 |
