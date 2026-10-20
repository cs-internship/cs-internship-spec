## Step 10. Agent-Assisted Integration

<!-- outcomes: AI-17 AI-18 API-17 BLAZOR-15 BLAZOR-16 DOTNET-AI-02 DOTNET-AI-03 -->

Use bounded agent assistance and persistent repository context to integrate remote services, browser capabilities, and a first application agent without surrendering review or control.

### Study Items  <!-- omit in toc -->

#### General AI

1. Build a bounded feature with agent mode by defining an issue, completion criteria, command boundaries, diff review, and verification checks ([Agent-First Development](https://www.youtube.com/watch?v=uu4sf8z9n8c), [Build an App with Agent Mode](https://www.youtube.com/watch?v=hmfldW7dmgw), [Copilot cloud-agent best practices](https://docs.github.com/en/copilot/tutorials/cloud-agent/get-the-best-results), [Review Copilot output](https://docs.github.com/en/copilot/how-tos/copilot-on-github/use-copilot-agents/review-copilot-output))
2. Add persistent repository context for architecture, conventions, commands, safety, and completion, author it as `AGENTS.md` so multiple coding tools share one instruction source, then compare agent work with and without it using the same task and checks ([Context Engineering with Copilot](https://www.youtube.com/watch?v=0jEzUhU8bLc), [VS Code custom instructions](https://code.visualstudio.com/docs/agent-customization/custom-instructions), [Repository custom instructions](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/add-custom-instructions/add-repository-instructions), [Evaluation best practices](https://developers.openai.com/api/docs/guides/evaluation-best-practices))
3. Classify three kinds of workplace content as public, internal, or restricted against the AI tools used in this course, then draft a short team policy covering what may be shared with each tool, disclosure of AI-generated code, license and attribution review, and who is accountable when AI-assisted changes ship ([AI Security in VS Code](https://code.visualstudio.com/docs/agents/run/security), [GitHub Copilot Documentation](https://docs.github.com/en/copilot), [OpenAI usage policies](https://openai.com/policies/usage-policies/))
4. (Optional) Drive one small feature spec-first by writing a spec, then a plan, then a task breakdown, and implementing against them, then compare the outcome quality with the issue-first agent workflow of this step using the same checks ([VS Code: Plan work](https://code.visualstudio.com/docs/agents/run/planning), [Evaluation best practices](https://developers.openai.com/api/docs/guides/evaluation-best-practices))
5. (Optional) Explain when git worktrees let multiple coding agents work the same repository safely, run one agent-assisted change in a dedicated worktree, and record the merge-back and cleanup steps ([git worktree](https://git-scm.com/docs/git-worktree), [VS Code: Agent best practices](https://code.visualstudio.com/docs/agents/best-practices))

#### ASP.NET Core

1. Build a typed remote API client, distinguish transient from permanent failures, apply current resilience handlers, and map transport objects into application models ([Book: Chapter 33](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-33), [`IHttpClientFactory`](https://learn.microsoft.com/en-us/dotnet/core/extensions/httpclient-factory), [HTTP resilience](https://learn.microsoft.com/en-us/dotnet/core/resilience/http-resilience), [Mapperly Documentation](https://mapperly.riok.app/))

#### Blazor

1. Expose a safe .NET method to JavaScript and dispose object references at the correct lifetime boundary ([Calling .NET from JavaScript](https://blazor-university.com/javascript-interop/calling-dotnet-from-javascript), [Call .NET methods from JavaScript](https://learn.microsoft.com/en-us/aspnet/core/blazor/javascript-interoperability/call-dotnet-from-javascript?view=aspnetcore-10.0))
2. Invoke browser APIs from .NET and handle `JSException` and disconnected-circuit failures ([Calling JavaScript from .NET](https://blazor-university.com/javascript-interop/calling-javascript-from-dotnet), [Call JavaScript from .NET](https://learn.microsoft.com/en-us/aspnet/core/blazor/javascript-interoperability/call-javascript-from-dotnet?view=aspnetcore-10.0), [Disconnected-circuit guidance](https://learn.microsoft.com/en-us/aspnet/core/blazor/javascript-interoperability/?view=aspnetcore-10.0))

#### .NET AI

1. Explain the Microsoft Agent Framework landscape and when to choose it over the legacy Semantic Kernel or direct Microsoft Extensions AI use ([Introduction](https://www.youtube.com/watch?v=9RNF9GsB8PU), [Agent Framework vs Semantic Kernel vs Extensions.AI](https://www.youtube.com/watch?v=6ue9SmEtG9k), [GA Part 1](https://www.youtube.com/watch?v=2ZwxQmT1l7s), [Current Agent Framework overview](https://learn.microsoft.com/en-us/agent-framework/overview/?pivots=programming-language-csharp))
2. Create and run a first agent in C# against the configured provider and compare provider options ([Getting Started](https://www.youtube.com/watch?v=HHy0-sXlmUY), [Zero to First OpenAI Agent](https://www.youtube.com/watch?v=CvA69UyqJ7U), [Using other LLMs](https://www.youtube.com/watch?v=GbyEQWwBMFk), [Current C# quickstart](https://learn.microsoft.com/en-us/agent-framework/get-started/))
3. (Optional) Generate embeddings for application content with `IEmbeddingGenerator`, retrieve the most relevant chunks for a query, and implement grounded generation that answers only from retrieved context with cited sources ([Use the `IEmbeddingGenerator` interface](https://learn.microsoft.com/en-us/dotnet/ai/iembeddinggenerator), [Build a .NET AI vector search app](https://learn.microsoft.com/en-us/dotnet/ai/vector-stores/how-to/build-vector-search-app))

### Tasks  <!-- omit in toc -->

1. Pass all lessons on TypingClub.com **with 5 stars** up to lesson 418.
2. **Establish the Agent Development Contract** <!-- bc: 09-T1 -->
   - **Goal:** Make agent-assisted changes bounded, repeatable, and reviewable.
   - **Deliverable:** Persistent repository instructions, a bounded feature issue, agent plan, command log, reviewed diff, and verification results.
   - **Requirements:**
     - Document architecture, conventions, build and test commands, safety rules, and definition of done.
     - Run a small comparison with and without repository context.
     - Reject or revise at least one unsuitable suggestion when present, or explain why all suggestions were acceptable.
   - **Acceptance criteria:**
     - [ ] The issue states scope, exclusions, and objective completion checks.
     - [ ] Repository instructions contain no secrets or machine-specific credentials.
     - [ ] The final diff contains only intended changes and passes its checks.
     - [ ] The comparison identifies the observable effect of persistent context.
   - **Submission:**
     - Repository instructions and agent-development evidence.
3. **Build the Integration Feature** <!-- bc: 09-T2 -->
   - **Goal:** Combine external data, AI processing, and a browser capability through explicit boundaries.
   - **Deliverable:** Typed remote client, mapping layer, Microsoft Extensions AI service, and a Blazor interaction that demonstrates both JavaScript-to-.NET and .NET-to-JavaScript calls.
   - **Requirements:**
     - Map remote DTOs into internal models without leaking transport concerns into the UI.
     - Handle timeout, invalid response, and unavailable-provider cases.
     - Add one justified AI transformation or analysis of external data.
     - Use JavaScript interop for a browser-only capability such as clipboard, focus, storage, or download.
   - **Acceptance criteria:**
     - [ ] Remote failures produce controlled application behavior.
     - [ ] Product code depends on application abstractions rather than provider SDK types.
     - [ ] JavaScript references are released where required and errors are handled.
     - [ ] AI output is evaluated against at least three representative cases.
   - **Submission:**
     - Remote API contract and mapping notes.
     - Failure-case and AI-evaluation results.
     - Short recording or screenshots of the interop behavior.
4. **Run the First Product Agent** <!-- bc: 09-T3 -->
   - **Goal:** Bring a first Agent Framework agent into the application behind the existing service boundaries.
   - **Deliverable:** Agent service, framework decision note, provider configuration, recorded conversations, and fallback behavior.
   - **Requirements:**
     - Register the agent behind an application abstraction so product code does not depend on agent SDK types.
     - Record a short decision note explaining why Agent Framework fits this feature compared with alternatives.
     - Keep the agent bounded to one clear product purpose.
     - Handle the unavailable-provider case with controlled behavior.
   - **Acceptance criteria:**
     - [ ] The agent completes its bounded purpose in at least three recorded conversations.
     - [ ] Provider credentials stay outside source control.
     - [ ] The decision note compares at least two alternatives with a stated reason.
     - [ ] Provider failure produces a safe, documented response.
   - **Submission:**
     - Agent decision note, conversations, and fallback evidence.
5. Toward the end of your step, and before your online presentation, attend a technical session with one of your track’s technical mentors and receive their feedback.
6. At least 10 days before your deadline, start coordinating and scheduling your live presentation session as the final task of this step.  
   For more details about the live presentation, please check ["Delivering an Online Presentation"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Delivering%20an%20Online%20Presentation%20--%20fa.md).
7. Hold your live presentation on LinkedIn.
