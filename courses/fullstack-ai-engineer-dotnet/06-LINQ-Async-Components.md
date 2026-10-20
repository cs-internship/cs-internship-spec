## Step 6. LINQ, Asynchronous Programming, and Component Architecture

<!-- outcomes: AI-10 AI-11 API-07 API-08 WEB-04 BLAZOR-03 BLAZOR-04 -->

Query data with LINQ and go deeper into multithreading and asynchronous C#, which the persistence work in Step 7 depends on. Give the portfolio application configurable services and reusable Blazor layouts and components, and build a reusable context pack and prompt tool that make AI work more reliable.

### Study Items  <!-- omit in toc -->

#### C# Language

1. [C# book](https://www.oreilly.com/library/view/programming-c-12/9781098158354/), chapter 10 : LINQ
2. [C# book](https://www.oreilly.com/library/view/programming-c-12/9781098158354/), chapter 16 : Multithreading
3. [C# book](https://www.oreilly.com/library/view/programming-c-12/9781098158354/), chapter 17 : Asynchronous Language Features
4. [C# Lock Multithreading/Tasks](https://www.youtube.com/watch?v=Y8Go3c-brcg)
5. [Thread Synchronization in C#](https://www.youtube.com/watch?v=5Zv8fF-KPrE)
6. [Improve App Responsiveness: A Guide to C# Async/Await](https://www.youtube.com/watch?v=2moh18sh5p4)

#### General AI

1. Build a prompt application that summarizes, infers, transforms, or expands text with a consistent output schema, iterative improvement, and edge-case review ([OpenAI prompt engineering](https://developers.openai.com/api/docs/guides/prompt-engineering), [Structured Outputs](https://developers.openai.com/api/docs/guides/structured-outputs), [Evaluation best practices](https://developers.openai.com/api/docs/guides/evaluation-best-practices))
2. (Optional) Watch [ChatGPT Prompt Engineering for Developers](https://learn.deeplearning.ai/courses/chatgpt-prompt-eng/lesson/dfbds/introduction) to see summarizing, inferring, transforming, and expanding prompts in practice before you build your prompt tool.
3. Create a reusable context pack with project goals, source links, examples, constraints, vocabulary, and completion criteria, measure its token footprint against the model context window and apply one truncation or summarization strategy when it exceeds budget, then run the same prompt with and without it and score both with the same rubric ([Context Engineering with Copilot](https://www.youtube.com/watch?v=0jEzUhU8bLc), [VS Code: Context engineering guide](https://code.visualstudio.com/docs/agents/guides/context-engineering-guide), [VS Code: Custom instructions](https://code.visualstudio.com/docs/agent-customization/custom-instructions), [Evaluation best practices](https://developers.openai.com/api/docs/guides/evaluation-best-practices))

#### ASP.NET Core

1. Explain dependency injection, register services, select lifetimes, and consume dependencies without service location ([Book: Chapter 8](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-8), [Book: Chapter 9](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-9), [Dependency Injection @ 2:26:52](https://www.youtube.com/watch?v=YbRe4iIVYJk&t=8812s))
2. Load environment-aware configuration and bind validated options for application behavior ([Book: Chapter 10](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-10), [Configuration @ 2:17:46](https://www.youtube.com/watch?v=YbRe4iIVYJk&t=8266s), [Microsoft: Options validation](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/configuration/options?view=aspnetcore-10.0#validateonstart))

#### Frontend

1. Apply positioning, transitions, and animations while preserving focus visibility and honoring reduced-motion preferences ([CSS Positioning](https://cssreference.io/positioning/), [CSS Transitions](https://cssreference.io/transitions/), [CSS Animations](https://cssreference.io/animations/), [MDN: `:focus-visible`](https://developer.mozilla.org/en-US/docs/Web/CSS/:focus-visible), [MDN: `prefers-reduced-motion`](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-reduced-motion))

#### Blazor

1. Create application and nested feature layouts that separate shared navigation from page content ([Creating a Blazor Layout](https://blazor-university.com/layouts/creating-a-blazor-layout), [Nested Layouts](https://blazor-university.com/layouts/nested-layouts))
2. Build reusable components and demonstrate one-way and two-way data binding ([Creating a Component](https://blazor-university.com/components/creating-a-component), [One-Way Binding](https://blazor-university.com/components/one-way-binding), [Two-Way Binding](https://blazor-university.com/components/two-way-binding))

### Tasks  <!-- omit in toc -->

1. As part of the **Mentor Training** path, watch the **fifth** of the twelve videos in the **Coaching** course using [this link](https://drive.google.com/drive/folders/1MBTCHtzWzmGqQEKe6U86jjzxUxxEtUn4). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
2. As part of the **Mentor Training** path, watch the **sixth** of the twelve videos in the **Coaching** course using [this link](https://drive.google.com/drive/folders/1EjO3sPNeiq8c0nKGB_oUyelM2jxVZRd1). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
3. Pass all lessons on TypingClub.com **with 5 stars** up to lesson 316.
4. Complete the [Working with LINQ](https://learn.microsoft.com/en-us/dotnet/csharp/tutorials/working-with-linq) tutorial. (Optional) Use [LINQPad](https://www.linqpad.net/) to run and inspect its queries.
5. Pass these exercises at exercism.io:
   - Grade School
6. **Build and Evaluate a Prompt Tool** <!-- bc: 04-T1 -->
   - **Goal:** Turn one repeated product workflow into a bounded, reviewable prompt tool.
   - **Deliverable:** Prompt template, context pack, test inputs, structured outputs, rubric results, and human-review checklist under `docs/ai/`.
   - **Requirements:**
     - Require a predictable output structure.
     - Test normal, empty, ambiguous, and adversarial inputs.
     - Compare at least three results with and without the context pack.
   - **Acceptance criteria:**
     - [ ] Output can be parsed or reviewed consistently.
     - [ ] The context comparison identifies measurable improvements and remaining failures.
     - [ ] Human approval is required before generated material enters the application.
   - **Submission:**
     - Prompt tool and context pack under `docs/ai/`.
7. **Create the Configurable Component Shell** <!-- bc: 04-T2 -->
   - **Goal:** Give the portfolio application reusable UI and backend boundaries.
   - **Deliverable:** Configured application service, validated options, nested Blazor layout, and at least two reusable bound components.
   - **Requirements:**
     - Place product logic behind an injected interface.
     - Bind configuration to a typed options class and fail clearly when required values are absent.
     - Add shared and feature layouts.
     - Add a focused transition or animation with a reduced-motion fallback.
   - **Acceptance criteria:**
     - [ ] Service registration uses an intentional lifetime documented in `docs/architecture.md`.
     - [ ] Development and production configuration can differ without code changes.
     - [ ] Components receive data through parameters or binding rather than global mutable state.
     - [ ] Keyboard focus and reduced-motion behavior remain usable.
   - **Submission:**
     - Architecture update describing dependency and configuration decisions.
     - Screenshots or recording of the component layouts and visual interaction.
8. After thoroughly reviewing the ["Technical Assistant Role"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Technical%20Assistant%20Role%20--%20fa.md) document, submit your request to serve as a Level 2 Technical Assistant.
9. Toward the end of your step, and before your online presentation, attend a technical session with one of your track’s technical mentors and receive their feedback.
10. At least 10 days before your deadline, start coordinating and scheduling your live presentation session as the final task of this step.  
    For more details about the live presentation, please check ["Delivering an Online Presentation"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Delivering%20an%20Online%20Presentation%20--%20fa.md).
11. Hold your live presentation on LinkedIn.
