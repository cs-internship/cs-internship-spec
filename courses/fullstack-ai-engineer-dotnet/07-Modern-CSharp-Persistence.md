## Step 7. Modern C# and Persistent Applications

<!-- outcomes: AI-12 API-09 API-10 WEB-05 BLAZOR-05 BLAZOR-06 -->

Catch up with modern C#, including nullable reference types, which also shape how EF Core maps your data. Then move the portfolio application from temporary behavior to a documented, persistent, responsive product while applying bounded AI loops and richer component interactions.

### Study Items  <!-- omit in toc -->

#### C# Language

1. [What's new in C# 14](https://learn.microsoft.com/en-us/dotnet/csharp/whats-new/csharp-14)
2. [Nullable Reference Types in C#](https://docs.microsoft.com/en-us/dotnet/csharp/nullable-references)
3. [Tutorial: Embracing Nullable Reference Types in C#](https://docs.microsoft.com/en-us/dotnet/csharp/tutorials/nullable-reference-types)
4. [Upgrading Your Codebase with C# Nullable Reference Types](https://docs.microsoft.com/en-us/dotnet/csharp/tutorials/upgrade-to-nullable-references)
5. [Exploring Nullable Reference Types: A Practical Guide](https://devblogs.microsoft.com/dotnet/try-out-nullable-reference-types)

#### General AI

1. Explain the agent-first harness, model, prompt, tool, and context concepts, then design and test a bounded plan-action-evaluation loop with iteration limits, stop conditions, and human approval ([Agent-First Development](https://www.youtube.com/watch?v=uu4sf8z9n8c), [Agent loop and maximum turns](https://openai.github.io/openai-agents-python/running_agents/#the-agent-loop), [Agent orchestration](https://openai.github.io/openai-agents-python/multi_agent/), [Copilot cloud-agent best practices](https://docs.github.com/en/copilot/tutorials/cloud-agent/get-the-best-results))

#### ASP.NET Core

1. Generate, inspect, and improve OpenAPI documentation for the application endpoints ([Book: Chapter 11](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-11), [OpenAPI in .NET](https://www.youtube.com/watch?v=0qtwYT4n2CM), [Include OpenAPI metadata](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/openapi/include-metadata?view=aspnetcore-10.0))
2. Model relational data, use EF Core migrations, and explain the SQL operations behind persistent CRUD behavior ([Book: Chapter 12](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-12), [EF Core @ 1:34:00](https://www.youtube.com/watch?v=YbRe4iIVYJk&t=5640s), [SQL and EF Core @ 32:42](https://www.youtube.com/watch?v=38GNKtclDdE&t=1962s), [SQL Tutorial](https://www.w3schools.com/sql/))

#### Frontend

1. Apply fluid sizing, media queries, responsive layout changes, and mobile-first checks to the product UI ([Responsive Web Design](https://www.youtube.com/watch?v=zF6VSky4SIc), [MDN: Responsive design](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Responsive_Design))

#### Blazor

1. Handle component and browser DOM events, then test mouse and keyboard interaction paths for custom controls ([Component Events](https://blazor-university.com/components/component-events), [Browser DOM Events](https://blazor-university.com/components/component-events/browser-dom-events), [bUnit event tests](https://bunit.dev/docs/interaction/trigger-event-handlers.html), [WAI: Keyboard interface](https://www.w3.org/WAI/ARIA/apg/practices/keyboard-interface/))
2. Use cascading values for shared UI context and capture unmatched attributes for extensible components ([Cascading Values](https://blazor-university.com/components/cascading-values), [Capturing Unexpected Parameters](https://blazor-university.com/components/capturing-unexpected-parameters))

### Tasks  <!-- omit in toc -->

1. As part of the **Mentor Training** path, watch the **seventh** of the twelve videos in the **Coaching** course using [this link](https://drive.google.com/drive/folders/16fch6aIfZL1laupMDYruy3HjmxV8WA-p). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
2. As part of the **Mentor Training** path, watch the **eighth** of the twelve videos in the **Coaching** course using [this link](https://drive.google.com/drive/folders/1REyXmFfCWTDpCrsbNoJojHjH9ZQEXzqx). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
3. Pass all lessons on TypingClub.com **with 5 stars** up to lesson 357.
4. Find and introduce 2 blog posts about how people experienced upgrading their projects to support nullable reference types.
5. In your opinion, what's the biggest challenge in upgrading a project to nullable reference types?
6. Find and introduce 2 libraries on GitHub which have enabled nullable reference types.
7. Find a small GitHub project and help to make it use nullable reference types.
8. Describe the situations that Pattern Matching helps. How does it help?
9. **Specify and Test a Bounded AI Loop** <!-- bc: 05-T1 -->
   - **Goal:** Define a safe iterative workflow for improving product content or data.
   - **Deliverable:** `docs/ai/bounded-loop.md` and a run log for a writer, critic, and reviser workflow.
   - **Requirements:**
     - Define inputs, evaluation rubric, maximum iterations, stop conditions, and human approval points.
     - Run one successful case and one case that stops because a limit or quality rule is reached.
     - Record every iteration without hiding failed outputs.
   - **Acceptance criteria:**
     - [ ] The loop cannot continue indefinitely.
     - [ ] A human approves any result selected for product use.
     - [ ] The run log demonstrates both success and controlled stopping.
   - **Submission:**
     - AI loop specification and run log.
10. **Build the Persistent Responsive Feature** <!-- bc: 05-T2 -->
    - **Goal:** Replace in-memory behavior with a usable database-backed vertical slice.
    - **Deliverable:** EF Core model and migration, documented CRUD API, and responsive Blazor list and details components.
    - **Requirements:**
      - Persist the primary product resource in a relational database.
      - Expose and review the OpenAPI document.
      - Use events for user actions and a cascading value for shared display context.
      - Verify the UI at small, medium, and large viewport widths.
    - **Acceptance criteria:**
      - [ ] Data remains after the application restarts.
      - [ ] A clean database can be created using committed migrations.
      - [ ] OpenAPI describes the implemented success and error responses.
      - [ ] The UI has no horizontal page overflow at the tested widths.
      - [ ] Reusable components accept standard HTML attributes where appropriate.
    - **Submission:**
      - Migration files and database setup instructions.
      - OpenAPI document or screenshot.
      - Responsive screenshots at three viewport widths.
11. Toward the end of your step, and before your online presentation, attend a technical session with one of your track’s technical mentors and receive their feedback.
12. At least 10 days before your deadline, start coordinating and scheduling your live presentation session as the final task of this step.  
    For more details about the live presentation, please check ["Delivering an Online Presentation"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Delivering%20an%20Online%20Presentation%20--%20fa.md).
13. Hold your live presentation on LinkedIn.
