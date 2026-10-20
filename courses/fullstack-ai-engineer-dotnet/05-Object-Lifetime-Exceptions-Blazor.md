## Step 5. Object Lifetime, Exceptions, and the First Blazor App

<!-- outcomes: AI-14 API-05 API-06 WEB-03 BLAZOR-01 BLAZOR-02 -->

Learn how .NET manages memory and object lifetime and how C# reports and handles errors. Apply both while you design predictable routes and validation errors, lay out the application dashboard, and create your first Blazor pages. Along the way, generate a product visual and keep the final choice in human hands.

### Study Items  <!-- omit in toc -->

#### C# Language

1. [C# book](https://www.oreilly.com/library/view/programming-c-12/9781098158354/), chapter 7 : Object Lifetime
2. [Object Lifetime (Wikipedia article)](https://en.wikipedia.org/wiki/Object_lifetime)
3. [Garbage Collection (Microsoft .NET Guide)](https://learn.microsoft.com/en-us/dotnet/standard/garbage-collection/), focusing on these pages:
   - [Fundamentals of garbage collection](https://learn.microsoft.com/en-us/dotnet/standard/garbage-collection/fundamentals)
   - [Implement a Dispose method](https://learn.microsoft.com/en-us/dotnet/standard/garbage-collection/implementing-dispose)
   - [Using objects that implement IDisposable](https://learn.microsoft.com/en-us/dotnet/standard/garbage-collection/using-objects)
4. [Finalizers (Microsoft C# Programming Guide)](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/destructors)
5. [dotMemory — .NET memory profiler by JetBrains (Youtube video)](https://youtube.com/playlist?list=PLQ176FUIyIUbEfA-XkqEBBNaU28RvtWEL)
6. [5 Techniques to avoid Memory Leaks by Events in C# .NET you should know](https://web.archive.org/web/20220519175107/https://michaelscodingspot.com/5-techniques-to-avoid-memory-leaks-by-events-in-c-net-you-should-know/)
7. [C# book](https://www.oreilly.com/library/view/programming-c-12/9781098158354/), chapter 8 : Exceptions
8. [Checked or Unchecked Exceptions?](https://jenkov.com/tutorials/java-exception-handling/checked-or-unchecked-exceptions.html)
9. [C# Exception Handling Best Practices](https://stackify.com/csharp-exception-handling-best-practices/)

#### General AI

1. Generate image variations for a communication goal, inspect visible strengths and errors, compare the variations with an explicit rubric, and record the final human choice ([Create images](https://developers.openai.com/api/docs/guides/image-generation), [Evaluation best practices](https://developers.openai.com/api/docs/guides/evaluation-best-practices))

#### ASP.NET Core

1. Design literal, parameterized, constrained, and grouped routes for a coherent API ([Book: Chapter 5](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-5), [Book: Chapter 6](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-6), [Minimal API Routing](https://www.youtube.com/watch?v=KZYvpNgGBZI))
2. Apply model binding and validation, and design useful validation error responses ([Book: Chapter 7](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-7), [Validation @ 1:25:07](https://www.youtube.com/watch?v=YbRe4iIVYJk&t=5107s), [Validation Documentation](https://docs.fluentvalidation.net/), [Microsoft: API error handling](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/error-handling-api?view=aspnetcore-10.0))

#### Frontend

1. Construct application layouts with Flexbox and Grid and explain why each layout model fits its selected region ([Flexbox Reference](https://cssreference.io/flexbox/), [Grid Reference](https://cssreference.io/css-grid/), [MDN: Grid compared with other layout methods](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Grid_layout/Relationship_with_other_layout_methods))

#### Blazor

1. Compare current Blazor hosting and render modes and record a decision for the portfolio application ([Microsoft: Hosting Models](https://learn.microsoft.com/en-us/aspnet/core/blazor/hosting-models?view=aspnetcore-10.0), [Microsoft: Render Modes](https://learn.microsoft.com/en-us/aspnet/core/blazor/components/render-modes?view=aspnetcore-10.0), [Blazor University: Hosting Models](https://blazor-university.com/overview/blazor-hosting-models), [Blazor Deep Dive in .NET 10](https://www.youtube.com/watch?v=holzuW1o6cs))
2. Create a Blazor project and add the first feature page ([Creating a New Project](https://blazor-university.com/overview/creating-a-new-project), [Creating a Page](https://blazor-university.com/overview/creating-a-page))

### Tasks  <!-- omit in toc -->

1. It's time to begin your journey as a mentoring intern. Ask your coordinator to start your onboarding process for mentorship.
2. As part of the **Mentor Training** path, watch the **third** of the twelve videos in the **Coaching** course using [this link](https://drive.google.com/drive/folders/1O4JD5_fs6ako8-kvxhjv7_1qg6eoawvN?usp=share_link). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
3. As part of the **Mentor Training** path, watch the **fourth** of the twelve videos in the **Coaching** course using [this link](https://drive.google.com/drive/folders/1v38qtor7nZ00mPQDNbke8BNwgHK_vb6K). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
4. Pass all lessons on TypingClub.com **with 5 stars** up to lesson 285.
5. Look for some famous memory leak inspection tools. Name them and a little comparison of their features.
6. **Create a Reviewed Product Visual** <!-- bc: 07-T1 -->
   - **Goal:** Produce a useful visual asset without losing human editorial control.
   - **Deliverable:** Image brief, at least three generated variations, selected final asset, evaluation rubric, and selection rationale under `docs/visuals/`.
   - **Requirements:**
     - Define the communication goal, audience, placement, and dimensions.
     - Inspect each variation for visible strengths and errors, then compare all variations with the same rubric.
     - Record why a person selected the final asset over the alternatives.
   - **Acceptance criteria:**
     - [ ] The selected asset fulfills the documented communication goal.
     - [ ] Visible errors and unsupported claims have been removed.
     - [ ] The final selection is supported by the documented evaluation rubric and human review.
   - **Submission:**
     - Visual brief, variants, final image, and evaluation rubric.
7. **Build a Navigable and Validated Product Shell** <!-- bc: 03-T2 -->
   - **Goal:** Connect a structured UI to a predictable API surface.
   - **Deliverable:** A Blazor application shell, responsive dashboard layout, and routed API endpoints with validation.
   - **Requirements:**
     - Add list and details routes with constrained identifiers.
     - Validate create or update input and return useful errors.
     - Create at least two Blazor pages and navigation between them.
     - Use Flexbox or Grid for the dashboard and document the hosting decision.
   - **Acceptance criteria:**
     - [ ] Valid, invalid, and missing-resource requests have distinct responses.
     - [ ] Direct navigation to each Blazor page works.
     - [ ] The layout uses Flexbox or Grid without table-based positioning.
     - [ ] `docs/architecture.md` records the Blazor hosting decision and tradeoffs.
   - **Submission:**
     - The Blazor hosting decision.
     - API request examples covering routing and validation.
     - Screenshots of the Blazor pages at two viewport widths.
8. Toward the end of your step, and before your online presentation, attend a technical session with one of your track’s technical mentors and receive their feedback.
9. At least 10 days before your deadline, start coordinating and scheduling your live presentation session as the final task of this step.  
   For more details about the live presentation, please check ["Delivering an Online Presentation"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Delivering%20an%20Online%20Presentation%20--%20fa.md).
10. Hold your live presentation on LinkedIn.
