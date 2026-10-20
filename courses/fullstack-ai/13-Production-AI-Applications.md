## Step 13. Production AI Applications

<!-- outcomes: AI-20 API-15 API-16 API-20 BLAZOR-19 DOTNET-AI-10 DOTNET-AI-11 -->

Prepare the portfolio application for real operation by evaluating its AI opportunities, hardening and orchestrating its services, verifying its agent packages, and adding a validated generative interface.

### Study Items  <!-- omit in toc -->

#### General AI

1. Create an AI opportunity map covering intelligent features, smaller models, multimodal interfaces, tool use, agents, evaluation, risk, and non-AI alternatives or fallbacks ([AI for Application Developers](https://www.youtube.com/watch?v=awztkr8n0AA), [NIST AI RMF Playbook](https://www.nist.gov/itl/ai-risk-management-framework/nist-ai-rmf-playbook), [Agent Framework evaluation](https://learn.microsoft.com/en-us/agent-framework/agents/evaluation))

#### ASP.NET Core

1. Publish an ASP.NET Core application and document a repeatable, target-specific deployment and rollback process ([Book: Chapter 27](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-27), [`dotnet publish`](https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-publish), [ASP.NET Core hosting and deployment](https://learn.microsoft.com/en-us/aspnet/core/host-and-deploy/?view=aspnetcore-10.0), [Azure deployment slots example](https://learn.microsoft.com/en-us/azure/app-service/deploy-staging-slots))
2. Apply HTTPS, secret handling, secure headers, least privilege, dependency review, and production hardening ([Book: Chapter 28](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-28), [Chapter 29](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-29), [HTTPS and HSTS](https://learn.microsoft.com/en-us/aspnet/core/security/enforcing-ssl?view=aspnetcore-10.0), [Application secrets](https://learn.microsoft.com/en-us/aspnet/core/security/app-secrets?view=aspnetcore-10.0), [Resource authorization](https://learn.microsoft.com/en-us/aspnet/core/security/authorization/secure-data?view=aspnetcore-10.0), [Review vulnerable packages](https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-package-list), [OWASP HTTP security headers](https://cheatsheetseries.owasp.org/cheatsheets/HTTP_Headers_Cheat_Sheet.html))
3. Model and run the application resources through a .NET Aspire AppHost and inspect their health, logs, traces, and metrics ([Introduction to .NET Aspire](https://www.youtube.com/watch?v=x2KAfsFydIo), [Add Aspire to an existing app](https://learn.microsoft.com/en-us/dotnet/aspire/get-started/add-aspire-existing-app), [Aspire dashboard overview](https://learn.microsoft.com/en-us/dotnet/aspire/fundamentals/dashboard/overview), [Explore the dashboard](https://learn.microsoft.com/en-us/dotnet/aspire/fundamentals/dashboard/explore))

#### Blazor

1. Evaluate current Blazor hosting, render, Hybrid, and optional framework choices against the product requirements, treating Bit Platform as a case study rather than the sole authority ([Blazor hosting models](https://learn.microsoft.com/en-us/aspnet/core/blazor/hosting-models?view=aspnetcore-10.0), [Blazor render modes](https://learn.microsoft.com/en-us/aspnet/core/blazor/components/render-modes?view=aspnetcore-10.0), [Blazor Hybrid](https://learn.microsoft.com/en-us/aspnet/core/blazor/hybrid/?view=aspnetcore-10.0), [Bit Platform](https://bitplatform.dev/))

#### .NET AI

1. Implement generative UI interactions with AG-UI and connect them to the product agents ([How to use AG-UI](https://www.youtube.com/watch?v=tDQc6lZUbYc), [Advanced AG-UI](https://www.youtube.com/watch?v=9nEcVoQCkYA), [AG-UI and A2UI](https://www.youtube.com/watch?v=aYe12ryuB4s), [Current AG-UI integration](https://learn.microsoft.com/en-us/agent-framework/integrations/ag-ui/), [AG-UI getting started](https://learn.microsoft.com/en-us/agent-framework/integrations/ag-ui/getting-started))
2. Explain how agent protocols such as A2A let independent agents and services cooperate ([A2A Protocol](https://www.youtube.com/watch?v=g72ks3rY9qQ), [Current A2A integration](https://learn.microsoft.com/en-us/agent-framework/integrations/a2a))
3. Record the audit date, exact Agent Framework package versions, lifecycle status, and breaking-change risk against production requirements ([GA Part 2](https://www.youtube.com/watch?v=UaRB9uC1rTI), [Current overview](https://learn.microsoft.com/en-us/agent-framework/overview/?pivots=programming-language-csharp), [Official releases](https://github.com/microsoft/agent-framework/releases))
4. Read token usage from AI responses, record estimated cost per AI feature over a representative workload, and define a budget or alert threshold that triggers review ([OpenAI pricing](https://developers.openai.com/api/docs/pricing), [Agent Framework overview](https://learn.microsoft.com/en-us/agent-framework/overview/?pivots=programming-language-csharp))
5. Add a response cache for deterministic AI prompts, screen inputs and outputs with moderation or guardrails for one user-facing feature, and record whether Azure AI Foundry or an equivalent service is justified for model deployment in this product ([Agent Framework overview](https://learn.microsoft.com/en-us/agent-framework/overview/?pivots=programming-language-csharp), [Azure AI Foundry](https://learn.microsoft.com/en-us/azure/ai-foundry/))

### Tasks  <!-- omit in toc -->

1. **Approve the Production AI Architecture** <!-- bc: 12-T1 -->
   - **Goal:** Make evidence-based decisions about AI, UI, security, and operational boundaries.
   - **Deliverable:** AI opportunity map, architecture decision record, threat and failure review, evaluation plan, and non-AI fallbacks.
   - **Requirements:**
     - Score opportunities for user value, feasibility, evidence quality, cost, latency, verification effort, and harm.
     - Decide which of the implemented agent capabilities ship to production and which stay behind a flag or are excluded.
     - Select one generative UI interaction that fits the product and the existing agents.
     - Define human approval points and behavior when AI is unavailable.
     - Evaluate the current Blazor architecture and record whether a production framework change is justified.
   - **Acceptance criteria:**
     - [ ] Rejected or deferred AI opportunities include a clear reason.
     - [ ] Each selected feature has measurable evaluation criteria.
     - [ ] The architecture record distinguishes current decisions from future options.
     - [ ] Every critical AI path has a safe fallback or controlled failure.
   - **Submission:**
     - Opportunity map and architecture decision record.
2. **Orchestrate and Harden the Application** <!-- bc: 12-T2 -->
   - **Goal:** Make all application resources repeatable, observable, and suitable for deployment.
   - **Deliverable:** Aspire AppHost, health checks, secure configuration, date-pinned AI package review, publish instructions, rollback procedure, and production-readiness checklist.
   - **Requirements:**
     - Model the web UI, API, database, and supporting resources in the AppHost.
     - Keep secrets outside source control and use least-privilege access.
     - Enforce HTTPS and review public endpoints and error details.
     - Review exact AI and agent package versions against the official release history and package-specific stable, prerelease, or experimental status; record upgrade, pinning, or removal decisions.
     - Capture resource health, logs, and one distributed operation where available.
   - **Acceptance criteria:**
     - [ ] A new developer can start the complete system from documented commands.
     - [ ] The Aspire dashboard shows expected resources as healthy.
     - [ ] Repository history and configuration contain no committed secrets.
     - [ ] Package review decisions are recorded with reasons.
     - [ ] Publish and rollback instructions are executable and unambiguous.
   - **Submission:**
     - Production-readiness, security, and package review checklist.
     - AppHost and deployment evidence.
3. **Add the Generative Interface** <!-- bc: 12-T3 -->
   - **Goal:** Implement the approved generative UI interaction on top of the existing agents within the documented safety boundaries.
   - **Deliverable:** Generative UI component, agent connection, protocol usage or justification, evaluation cases, and fallback behavior.
   - **Requirements:**
     - Drive the interface from the tool-using agents built in the previous step.
     - Validate generated UI data before rendering or acting on it.
     - Make agent progress, approval requests, failures, and completion visible to the user.
     - Use or justify an agent protocol such as A2A where agents or services cross boundaries.
     - Test normal, invalid, unavailable-provider, and denied-approval scenarios.
   - **Acceptance criteria:**
     - [ ] The agent cannot perform an approval-gated action without approval.
     - [ ] Invalid generated UI data fails safely.
     - [ ] The user can distinguish generated suggestions from committed application state.
     - [ ] Evaluation results meet the thresholds defined in the architecture task.
   - **Submission:**
     - Generative UI evaluation results.
4. Toward the end of your step, and before your online presentation, attend a technical session with one of your track’s technical mentors and receive their feedback.
5. At least 10 days before your deadline, start coordinating and scheduling your live presentation session as the final task of this step.  
   For more details about the live presentation, please check ["Delivering an Online Presentation"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Delivering%20an%20Online%20Presentation%20--%20fa.md).
6. Hold your live presentation on LinkedIn.
