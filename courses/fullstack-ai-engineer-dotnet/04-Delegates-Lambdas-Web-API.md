## Step 4. Delegates, Lambdas, and the First Web API

<!-- outcomes: AI-04 AI-09 API-01 API-02 API-03 API-04 -->

Learn how delegates, lambdas, and events work in C# and take a first look at async and await, because ASP.NET Core is built on them. Then run your first ASP.NET Core application, trace requests through its middleware pipeline, and build a small Minimal API, while you practice source-grounded prompting and verification on the same technical readings.

### Study Items  <!-- omit in toc -->

#### C# Language

1. [C# book](https://www.oreilly.com/library/view/programming-c-12/9781098158354/), chapter 9 : Delegates, Lambdas and Events
2. [Asynchronous programming with async and await](https://learn.microsoft.com/en-us/dotnet/csharp/asynchronous-programming/)

#### General AI

1. Open the [Microsoft: Middleware](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/middleware/?view=aspnetcore-10.0) article assigned in this step in two available browser assistants. In fresh conversations, give both assistants the same source-bounded prompt set: summarize the pipeline, explain `Use`, `Run`, and short-circuiting, predict the request and response log order, and conduct a three-question quiz that asks one question at a time and checks each answer against a named article section. Record the page or tab context each assistant can access, verify substantive claims against the article, inspect any source links before relying on them, and correct unsupported answers ([Copilot in Edge](https://support.microsoft.com/en-us/microsoft-copilot/getting-started-with-copilot-in-microsoft-edge), [Gemini in Chrome](https://support.google.com/chrome/answer/16283624?hl=en), [Gemini source links](https://support.google.com/gemini/answer/14143489?co=GENIE.Platform%3DDesktop&hl=en), [Lateral reading](https://cor.inquirygroup.org/curriculum/collections/teaching-lateral-reading/))
2. Design prompts with a goal, audience, context, constraints, examples, and output format, then evaluate them against varied inputs and explicit criteria ([Prompt Engineering Guide](https://www.youtube.com/watch?v=uDIW34h8cmM), [OpenAI prompt engineering](https://developers.openai.com/api/docs/guides/prompt-engineering), [Evaluation best practices](https://developers.openai.com/api/docs/guides/evaluation-best-practices))

#### ASP.NET Core

1. Identify the purpose, project structure, and development workflow of ASP.NET Core ([Book: Chapter 1](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-1), [.NET 10 course](https://www.youtube.com/watch?v=YbRe4iIVYJk))
2. Explain application startup and create a first running web application ([Book: Chapter 2](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-2), [Book: Chapter 3](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-3), [First application @ 06:40](https://www.youtube.com/watch?v=YbRe4iIVYJk&t=400s), [ASP.NET Core setup @ 02:02](https://www.youtube.com/watch?v=38GNKtclDdE&t=122s))
3. Trace a request through the middleware pipeline and explain why middleware order changes behavior ([Book: Chapter 4](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-4), [Microsoft: Middleware](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/middleware/?view=aspnetcore-10.0))
4. Create JSON endpoints with route handlers, status codes, and typed results using Minimal APIs ([Book: Chapter 5](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-5), [Minimal APIs @ 36:12](https://www.youtube.com/watch?v=YbRe4iIVYJk&t=2172s), [Minimal API responses and `TypedResults`](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/minimal-apis/responses?view=aspnetcore-10.0))

### Tasks  <!-- omit in toc -->

1. As part of the **Mentor Training** path, watch the **first** of the twelve videos in the **Coaching** course using [this link](https://drive.google.com/drive/folders/1O__WMdInuPReT-vxaCvBZXLIboJJxbzq?usp=share_link). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
2. As part of the **Mentor Training** path, watch the **second** of the twelve videos in the **Coaching** course using [this link](https://drive.google.com/drive/folders/1y_mkcHY05rmvsItvC8jFw5ly8tdiEvsC?usp=share_link). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
3. Pass all lessons on TypingClub.com **with 5 stars** up to lesson 244.
4. **Start the Portfolio Application (Part B)** <!-- bc: 01-T2-b -->
   - **Goal:** Complete the first vertical slice of the product with a running backend.
   - **Deliverable:** A running ASP.NET Core application and an information endpoint in the portfolio repository.
   - **Requirements:**
     - Add an endpoint that returns the product name, purpose, and current version as JSON.
     - Add run instructions to the project README.
   - **Acceptance criteria:**
     - [ ] The application starts without unhandled errors.
     - [ ] The information endpoint returns valid JSON.
     - [ ] Another learner can follow the README to run the application.
   - **Submission:**
     - Screenshot or response capture for the information endpoint.
5. **Build a Source-Grounded Prompt and Assistant Lab** <!-- bc: 02-T1 -->
   - **Goal:** Turn the step's technical readings into a verified learning artifact and a reusable source-to-implementation prompt.
   - **Deliverable:** `docs/prompt-lab.md` containing the source record, shared prompt set, browser-context record, assistant comparison, claim-verification table, corrected middleware trace, and three iterations of a source-to-implementation prompt with rubric results.
   - **Requirements:**
     - Open [Microsoft: Middleware](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/middleware/?view=aspnetcore-10.0) in both browser assistants. If the article or a named assistant is unavailable, record the limitation and use a technical mentor-approved equivalent with the same article, or another non-video reading linked in this step.
     - Use a clean browser window containing only public course pages, and disable unrelated browsing context when the product allows it. Record the assistant, browser, access date, source URL, context setting, shared pages, and how the source was provided: current tab, selected tabs, URL, uploaded file, or pasted text.
     - Start a fresh conversation in each assistant and use the same prompt set and questions from the study item.
     - For each assistant, verify at least three substantive claims against a named heading or anchor in the article. Mark each claim `supported`, `contradicted`, or `not found`, then correct or reject the latter two.
     - Record whether either assistant displays source or related links. Open every link used as evidence and confirm that it supports the associated claim. Record `none` when an assistant provides no links, and do not treat a displayed link as proof by itself.
     - Apply the linked lateral-reading method once: leave the target page and check the publisher, currency, and authority of the middleware article using another trustworthy source. Keep this source-quality check separate from the page-grounded claim verdicts.
     - Create a reusable prompt that turns a technical reading into an implementation checklist. Specify its goal, developer audience, source context, constraints, output structure, one worked example, evidence rule, and instruction to say `not found in the source` rather than guess.
     - Run prompt version 1 on [Microsoft: Middleware](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/middleware/?view=aspnetcore-10.0), score it, and revise one observed failure. Run version 2 on [Minimal API responses and `TypedResults`](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/minimal-apis/responses?view=aspnetcore-10.0), score it, and revise again. Regression-test version 3 on both articles and one non-video Frontend reading linked in Step 3 ([CSS Tutorial](https://www.w3schools.com/css/default.asp) or [CSS Reference](https://cssreference.io/)). Use the same source-fidelity, completeness, format-compliance, and actionability rubric for every run.
   - **Acceptance criteria:**
     - [ ] The report identifies the source by title, URL, and access date and shows that both assistants received the same prompt set and questions in fresh conversations.
     - [ ] The context record states the context setting, shared pages, and source-delivery method for each assistant without exposing unrelated private browsing data.
     - [ ] The verification table includes at least three claims per assistant, a source heading or anchor and verdict for each claim, and a correction or rejection for every contradicted or unlocated claim.
     - [ ] Every assistant-provided link used as evidence was opened and checked, and the separate lateral-reading record evaluates the publisher, currency, and authority of the target article.
     - [ ] The corrected middleware trace contains only source-supported claims and predicts the before-and-after logging order used in the *Add a Styled Minimal API Slice (Part B)* task.
     - [ ] The final reusable prompt specifies the audience, constraints, output structure, worked example, evidence rule, and `not found` behavior.
     - [ ] The report shows the version 1 and version 2 failure-driven revisions and version 3 regression results for both ASP.NET Core articles and one linked Frontend reading, all scored with the same rubric.
   - **Submission:**
     - `docs/prompt-lab.md` with redacted response captures or transcripts and shared-context evidence for both assistant runs.
6. **Add a Styled Minimal API Slice (Part B)** <!-- bc: 02-T2-b -->
   - **Goal:** Introduce request processing and JSON behavior in the portfolio application.
   - **Deliverable:** Custom request-logging middleware with a predicted-versus-observed trace and in-memory Minimal API endpoints for one product resource.
   - **Requirements:**
     - Add list, details, and create endpoints for the selected resource.
     - Return appropriate success and error status codes.
     - Record method, path, status code, and elapsed time in the middleware.
     - Before coding the middleware, use the verified trace from the *Build a Source-Grounded Prompt and Assistant Lab* task to predict its before-and-after log order, then compare that prediction with the actual output for one request.
   - **Acceptance criteria:**
     - [ ] Middleware produces one trace per request, and the observed before-and-after order is compared with the source-grounded prediction in `docs/prompt-lab.md`.
     - [ ] Endpoints return valid JSON and distinguish missing resources from successful responses.
   - **Submission:**
     - API request examples for success and failure cases.
     - Screenshot of the middleware output showing the predicted and observed order.
7. Toward the end of your step, and before your online presentation, attend a technical session with one of your track’s technical mentors and receive their feedback.
8. At least 10 days before your deadline, start coordinating and scheduling your live presentation session as the final task of this step.  
   For more details about the live presentation, please check ["Delivering an Online Presentation"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Delivering%20an%20Online%20Presentation%20--%20fa.md).
9. Hold your live presentation on LinkedIn.
