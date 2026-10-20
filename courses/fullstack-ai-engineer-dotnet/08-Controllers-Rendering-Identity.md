## Step 8. Controllers, Rendering, Identity, and Navigation

<!-- outcomes: API-11 API-12 API-13 BLAZOR-07 BLAZOR-08 BLAZOR-09 BLAZOR-10 BLAZOR-11 -->

Implement controller-based endpoints and reusable filters, and protect product capabilities with authentication and authorization. On the Blazor side, observe component lifecycles and rendering, then build reusable templated components and routed pages with deliberate navigation behavior.

### Study Items  <!-- omit in toc -->

#### ASP.NET Core

1. Compare the implementation shape of controller-based and Minimal APIs and implement a cohesive controller endpoint set ([Book: Chapter 20](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-20), [ASP.NET Core API approaches](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/apis?view=aspnetcore-10.0), [Controller APIs @ 10:00](https://www.youtube.com/watch?v=38GNKtclDdE&t=600s))
2. Apply filters for reusable cross-cutting behavior and explain their execution order ([Book: Chapter 21](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-21), [Book: Chapter 22](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-22), [Minimal API Filters](https://www.youtube.com/watch?v=2XoZOPrxegw))
3. Implement authentication and authorization, distinguish roles from policies, and protect API operations consistently ([Book: Chapter 23](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-23), [Chapter 24](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-24), [Chapter 25](https://livebook.manning.com/book/asp-net-core-in-action-third-edition/chapter-25), [Authorization overview](https://learn.microsoft.com/en-us/aspnet/core/security/authorization/introduction?view=aspnetcore-10.0), [Role-based authorization](https://learn.microsoft.com/en-us/aspnet/core/security/authorization/roles?view=aspnetcore-10.0), [Policy-based authorization](https://learn.microsoft.com/en-us/aspnet/core/security/authorization/policies?view=aspnetcore-10.0), [JWT Authentication and Authorization](https://www.youtube.com/watch?v=mgeuh8k3I4g))

#### Blazor

1. Observe component lifecycle methods and update rendered state safely when work completes asynchronously ([Component Lifecycles](https://blazor-university.com/components/component-lifecycles), [Multi-Threaded Rendering](https://blazor-university.com/components/multi-threaded-rendering), [Thread safety with `InvokeAsync`](https://blazor-university.com/components/multi-threaded-rendering/invokeasync/))
2. Explain render-tree comparison and use `@key` where stable component identity matters ([Render Trees](https://blazor-university.com/components/render-trees), [Optimizing with @key](https://blazor-university.com/components/render-trees/optimising-using-key))
3. Build a reusable templated component with `RenderFragment` and a generic type parameter ([RenderFragments](https://blazor-university.com/templating-components-with-renderfragements/), [Generic Components](https://blazor-university.com/templating-components-with-renderfragements/using-typeparam-to-create-generic-components))
4. Define routes and route parameters for list, details, and editing experiences ([Defining Routes](https://blazor-university.com/routing/defining-routes), [Route Parameters](https://blazor-university.com/routing/route-parameters))
5. Use HTML and programmatic navigation and respond intentionally to navigation events across current Blazor navigation modes ([HTML Navigation](https://blazor-university.com/routing/navigating-our-app-via-html), [Code Navigation](https://blazor-university.com/routing/navigating-our-app-via-code), [Navigation Events](https://blazor-university.com/routing/detecting-navigation-events), [Current Blazor navigation](https://learn.microsoft.com/en-us/aspnet/core/blazor/fundamentals/navigation?view=aspnetcore-10.0))

### Tasks  <!-- omit in toc -->

1. As part of the **Mentor Training** path, watch the **ninth** of the twelve videos in the **Coaching** course using [this link](https://drive.google.com/drive/folders/1lBqfqw7Th-zyc3XherR2GLCK3HtK2VaK). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
2. As part of the **Mentor Training** path, watch the **tenth** of the twelve videos in the **Coaching** course using [this link](https://drive.google.com/drive/folders/1_uRxg9mzKYycKT05O93r0-9Lh2McLjSb). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
3. Pass all lessons on TypingClub.com **with 5 stars** up to lesson 374.
4. **Build an Efficient Content Management Slice** <!-- bc: 06-T2 -->
   - **Goal:** Manage content artifacts through controller endpoints and a rendering-aware Blazor UI.
   - **Deliverable:** Controller-based content endpoints, a filter for one cross-cutting concern, and a Blazor content list with lifecycle and render observations.
   - **Requirements:**
     - Implement list, details, create, and update controller actions.
     - Add a filter for validation, timing, auditing, or another justified concern.
     - Record relevant lifecycle calls during initial load and refresh.
     - Demonstrate a reordered list with and without `@key`.
   - **Acceptance criteria:**
     - [ ] Controller responses follow the existing API error conventions.
     - [ ] The filter behavior is visible and does not duplicate controller logic.
     - [ ] UI updates occur without cross-thread rendering errors.
     - [ ] The render comparison explains when `@key` preserves identity.
   - **Submission:**
     - API request examples for the controller endpoints.
     - Filter and lifecycle evidence.
     - Render behavior comparison.
5. **Build a Secured Navigable Experience** <!-- bc: 07-T2 -->
   - **Goal:** Give authenticated users access to appropriate product actions through reusable UI.
   - **Deliverable:** Authentication flow, protected API operations, parameterized Blazor pages, and a generic list or table component.
   - **Requirements:**
     - Protect at least one write operation and one role or policy-specific operation.
     - Handle unauthorized and forbidden results distinctly.
     - Use the generic component for at least two data types or views.
     - Add details and edit routes and protect unsaved work during navigation.
   - **Acceptance criteria:**
     - [ ] Anonymous, authenticated, and insufficiently authorized requests behave differently.
     - [ ] Direct URLs with valid and invalid parameters are handled safely.
     - [ ] The generic component contains no product-specific type dependency.
     - [ ] Navigation behavior is keyboard accessible and does not silently discard edits.
   - **Submission:**
     - Authentication and authorization test evidence.
     - Screenshots of routed UI states.
6. Toward the end of your step, and before your online presentation, attend a technical session with one of your track’s technical mentors and receive their feedback.
7. At least 10 days before your deadline, start coordinating and scheduling your live presentation session as the final task of this step.  
   For more details about the live presentation, please check ["Delivering an Online Presentation"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Delivering%20an%20Online%20Presentation%20--%20fa.md).
8. Hold your live presentation on LinkedIn.
