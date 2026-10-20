## Step 9. Forms, Observability, and the First AI Feature

<!-- outcomes: AI-15 AI-16 API-14 BLAZOR-12 BLAZOR-13 BLAZOR-14 DOTNET-AI-01 -->

Add trustworthy data entry, structured diagnostics, and the first provider-neutral AI capability while communicating the product through a verified presentation.

### Study Items  <!-- omit in toc -->

#### General AI

1. Create a presentation from verified sources with an audience goal, story outline, accessible visuals, speaker notes, fact-checking, and rehearsal ([Gemini Notebook Integration](https://www.youtube.com/watch?v=Y-LTxr1bv9M), [Presentations with Microsoft 365 Copilot](https://www.youtube.com/watch?v=ioV4kREDrso), [Prepare a presentation with Copilot](https://support.microsoft.com/en-us/office/prepare-your-presentation-with-copilot-for-microsoft-365-7f06429e-c0c2-4819-8119-b519ad599796), [Make PowerPoint presentations accessible](https://support.microsoft.com/en-us/accessibility/powerpoint/make-your-powerpoint-presentations-accessible-to-people-with-disabilities), [Rehearse with Speaker Coach](https://support.microsoft.com/en-us/powerpoint/rehearse-your-slide-show-with-speaker-coach))
2. Use GitHub Copilot in VS Code for explanation, design, debugging, refactoring, tests, documentation, and review while verifying suggested changes ([Getting Started with GitHub Copilot](https://www.youtube.com/watch?v=n0NlxUyA7FI), [Build with agents in VS Code](https://code.visualstudio.com/docs/agents/overview), [VS Code AI smart actions](https://code.visualstudio.com/docs/editing/copilot-smart-actions), [Review and revert agent changes](https://code.visualstudio.com/docs/agents/run/review-code-edits), [Copilot cloud-agent best practices](https://docs.github.com/en/copilot/tutorials/cloud-agent/get-the-best-results))

#### ASP.NET Core

1. Use structured logging, scopes, and activity identifiers to monitor requests, correlate operations, and diagnose an application failure ([Book: Chapter 26](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-26), [Structured Logging](https://www.youtube.com/watch?v=MHJ0BHfWhRw), [ASP.NET Core logging](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/logging/?view=aspnetcore-10.0))

#### Blazor

1. Build forms that edit application data through Blazor input components ([Forms](https://blazor-university.com/forms/), [Editing Form Data](https://blazor-university.com/forms/editing-form-data))
2. Apply data annotations and custom validation with clear, accessible error notifications ([Validation](https://blazor-university.com/forms/validation), [Custom Validation](https://blazor-university.com/forms/writing-custom-validation), [Current Blazor validation](https://learn.microsoft.com/en-us/aspnet/core/blazor/forms/validation?view=aspnetcore-10.0), [Accessible error notifications](https://www.w3.org/WAI/tutorials/forms/notifications/))
3. Use public `EditContext` modification and validation APIs with navigation interception to manage unsaved changes ([EditContext concepts](https://blazor-university.com/forms/editcontext-fieldidentifiers-and-fieldstate), [`EditContext` API](https://learn.microsoft.com/en-us/dotnet/api/microsoft.aspnetcore.components.forms.editcontext?view=aspnetcore-10.0), [Current Blazor validation](https://learn.microsoft.com/en-us/aspnet/core/blazor/forms/validation?view=aspnetcore-10.0), [Blazor navigation and `NavigationLock`](https://learn.microsoft.com/en-us/aspnet/core/blazor/fundamentals/navigation?view=aspnetcore-10.0))

#### .NET AI

1. Identify Microsoft Extensions AI abstractions and implement a first AI-backed .NET feature that requests typed .NET objects through structured output and validates results before they change state ([Building AI Apps in .NET](https://www.youtube.com/watch?v=4B3ppx2U8bE), [Extensions AI overview](https://learn.microsoft.com/en-us/dotnet/ai/microsoft-extensions-ai), [Use `IChatClient`](https://learn.microsoft.com/en-us/dotnet/ai/ichatclient), [Build an AI chat app](https://learn.microsoft.com/en-us/dotnet/ai/quickstarts/build-chat-app), [Structured-output quickstart](https://learn.microsoft.com/en-us/dotnet/ai/quickstarts/structured-output))
2. Add generative AI through provider-neutral services and configuration rather than provider-specific application logic ([Adding GenAI to .NET Apps](https://www.youtube.com/watch?v=sgrsopf-fzo))
3. Stream model output with `IChatClient.CompleteStreamingAsync`, update the user interface incrementally without cross-thread render errors, and record what the chat feature needs from hosting and render modes ([Use `IChatClient`](https://learn.microsoft.com/en-us/dotnet/ai/ichatclient), [Build an AI chat app](https://learn.microsoft.com/en-us/dotnet/ai/quickstarts/build-chat-app))
4. (Optional) Run the first AI feature against a locally hosted model such as Ollama behind the same `IChatClient` abstraction and record behavioral, latency, and cost differences versus the cloud provider ([Microsoft Extensions AI overview](https://learn.microsoft.com/en-us/dotnet/ai/microsoft-extensions-ai), [Ollama](https://ollama.com/))

### Tasks  <!-- omit in toc -->

1. As part of the **Mentor Training** path, watch the **eleventh** of the twelve videos in the **Coaching** course using [this link](https://drive.google.com/drive/folders/1MnqRETVZgXRqUUYlCsiEs1SNUVSTkgyV). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
2. As part of the **Mentor Training** path, watch the **twelfth** of the twelve videos in the **Coaching** course using [this link](https://drive.google.com/drive/folders/1rF1CBqvjDmeV4_AW1HH1BCxsPZdbFz9L). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
3. Pass all lessons on TypingClub.com **with 5 stars** up to lesson 388.
4. **Present the Product Story** <!-- bc: 08-T1 -->
   - **Goal:** Explain the product problem, evidence, current solution, risks, and next milestone to a defined audience.
   - **Deliverable:** A concise slide deck, speaker notes, source list, fact-check record, accessibility check, and rehearsal notes.
   - **Requirements:**
     - Use verified material already created during the course.
     - Keep one main message per slide and provide accessible alternatives for important visuals.
     - Rehearse and revise for the intended time limit.
   - **Acceptance criteria:**
     - [ ] Claims are traceable to listed sources or project evidence.
     - [ ] Slides support rather than duplicate the spoken explanation.
     - [ ] Rehearsal notes identify and resolve at least two clarity problems.
   - **Submission:**
     - Presentation package and rehearsal notes.
5. **Build a Validated and Observable Editing Flow** <!-- bc: 08-T2 -->
   - **Goal:** Make data changes safe for users and diagnosable for developers.
   - **Deliverable:** Blazor create or edit form, custom validation, unsaved-change feedback, structured server logs, and a diagnosed failure note.
   - **Requirements:**
     - Show field-level and summary validation without losing user input.
     - Track modified state through `EditContext`.
     - Add correlation or operation context to relevant logs.
     - Use Copilot for one bounded change and record prompts, accepted edits, rejected suggestions, and verification.
   - **Acceptance criteria:**
     - [ ] Invalid data cannot be persisted.
     - [ ] Unsaved changes are visible before navigation.
     - [ ] Logs identify the request or operation without exposing secrets or sensitive form data.
     - [ ] The Copilot log shows human review and successful checks.
   - **Submission:**
     - Form validation and logging evidence.
     - Copilot work log and reviewed diff.
6. **Add the First AI Capability** <!-- bc: 08-T3 -->
   - **Goal:** Integrate a bounded generative feature without coupling the application to one provider.
   - **Deliverable:** An injected AI service, configuration, API endpoint or application service, reviewed output, and non-AI fallback.
   - **Requirements:**
     - Use Microsoft Extensions AI abstractions.
     - Keep credentials outside source control.
     - Constrain the feature to a clear input and output purpose.
     - Validate and review output before it changes persisted or user-visible data.
   - **Acceptance criteria:**
     - [ ] Provider-specific code is isolated from product logic.
     - [ ] Missing configuration produces a clear failure or documented fallback.
     - [ ] Inputs and outputs are logged safely without secrets.
     - [ ] The feature has at least three recorded evaluation cases.
   - **Submission:**
     - AI feature evaluation cases and configuration instructions.
7. After thoroughly reviewing the ["Technical Assistant Role"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Technical%20Assistant%20Role%20--%20fa.md) document, submit your request to serve as a Level 3 Technical Assistant.
8. Toward the end of your step, and before your online presentation, attend a technical session with one of your track’s technical mentors and receive their feedback.
9. At least 10 days before your deadline, start coordinating and scheduling your live presentation session as the final task of this step.  
   For more details about the live presentation, please check ["Delivering an Online Presentation"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Delivering%20an%20Online%20Presentation%20--%20fa.md).
10. Hold your live presentation on LinkedIn.
