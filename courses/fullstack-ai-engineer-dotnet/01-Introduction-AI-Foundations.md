## Step 1. Introduction, AI Foundations, and HTML

<!-- outcomes: AI-01 AI-02 AI-03 WEB-01 -->

Write your first C# programs, using Git to track your work and GitHub to host your code. Build a shared understanding of how generative AI works, where it fails, and why a person stays responsible for its results. You also start the portfolio application that grows through the whole course: choose its product domain and publish a semantic HTML page that communicates the idea.

### Study Items  <!-- omit in toc -->

#### C# Language

1. [C# book](https://www.oreilly.com/library/view/programming-c-12/9781098158354/), chapter 1 : C# Introduction
2. [C# book](https://www.oreilly.com/library/view/programming-c-12/9781098158354/), chapter 2 : Basic Coding in C#
3. [Introduction to Programming with CSharp](https://docs.microsoft.com/en-us/dotnet/csharp/tutorials/intro-to-csharp/local-environment)
   1. Read all the four tutorials.
   2. Run the codes locally while reading.

#### General AI

1. Explain generative AI, common model types, capabilities, limitations, useful applications, and decisions that should remain human-controlled ([Generative AI in a Nutshell](https://www.youtube.com/watch?v=2IK3DFHRFfw))
2. Explain in plain language how a large language model generates a response and why that response can be wrong ([Large Language Models](https://www.youtube.com/watch?v=osKyvYJ3PRM), [LLM Deep Dive](https://www.youtube.com/watch?v=7xTGNNLPyMI))
3. Explain how hallucinations can produce fluent but false or unsupported answers, verify a model answer against a known fact or inspectable source, and explain why a person remains responsible for using the result ([Hallucinations @ 01:20:44](https://www.youtube.com/watch?v=7xTGNNLPyMI&t=4844s), [Testing Known Answers @ 01:26:09](https://www.youtube.com/watch?v=7xTGNNLPyMI&t=5169s), [Human Responsibility @ 03:09:21](https://www.youtube.com/watch?v=7xTGNNLPyMI&t=11361s))

#### Frontend

1. Demonstrate HTML document structure, semantic elements, headings, links, lists, forms, and accessible content organization ([HTML Tutorial](https://www.w3schools.com/html/default.asp))

### Tasks  <!-- omit in toc -->

1. As part of the **Mentor Training** path, watch the **third** of the eight videos in the **Communication Training** course using [this link](https://drive.google.com/file/d/1omtXZwZCVE7mmtQNM1TnGy7Py5KXLgBx/view?usp=sharing). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
2. As part of the **Mentor Training** path, watch the **fourth** of the eight videos in the **Communication Training** course using [this link](https://drive.google.com/file/d/1Nr_vAxNQ3wx7zOrc7v7RJNHfRWFTSac-/view?usp=sharing). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
3. Pass all lessons on TypingClub.com **with 5 stars** up to lesson 88.
4. Create a GitHub account.
5. Follow at least 3 people on LinkedIn and 5 people (or accounts) on Twitter that are active and famous on C#.
6. Set up your development environment.
   1. [Download](https://dotnet.microsoft.com/download) .Net core sdk and install it.
   2. Create your first console app. Walk through [this tutorial](https://dotnet.microsoft.com/learn/dotnet/hello-world-tutorial/install).
7. Register at exercism.io. Join C# track in **practice mode**.
8. Pass these exercises at exercism.io:
   - Hello world (exercise number 1)
   - Two Fer
   - Leap
   - RNA Transcription
   - Gigasecond
9. Search about *bubble sort* algorithm. Write a program that has a method that receives a list of numbers and returns a sorted equivalent list. The method should be the bubble sort algorithm.
10. **Create an AI Foundations Pack** <!-- bc: 01-T1 -->
    - **Goal:** Document the AI concepts, verification habits, and human responsibility that will guide the project.
    - **Deliverable:** `docs/ai-foundations.md` containing a short plain-language LLM explanation, five possible AI applications, three decisions that remain human-controlled, and a hallucination and verification test table.
    - **Requirements:**
      - Run two model checks whose answers can be verified: one normal factual question and one question with a false premise or nonexistent detail.
      - For each check, record the prompt, response, source or known answer, unsupported or invented details, correction, and final human decision.
      - Explain briefly how an LLM generates text and why its answer may be wrong.
    - **Acceptance criteria:**
      - [ ] The explanation describes next-token prediction in plain language and states that a plausible response may still be wrong.
      - [ ] The report lists five possible applications and three decisions that remain human-controlled.
      - [ ] The test table contains both required checks.
      - [ ] Each checked claim has evidence and a verdict of verified, contradicted, or not verifiable.
      - [ ] Unsupported or invented details are identified as possible hallucinations and are corrected or rejected.
      - [ ] Each check records who owns the final decision and whether the model output is used, corrected, or rejected.
    - **Submission:**
      - `docs/ai-foundations.md`.
11. **Start the Portfolio Application (Part A)** <!-- bc: 01-T2-a -->
    - **Goal:** Create the first vertical slice of the product.
    - **Deliverable:** A repository containing a semantic HTML product page.
    - **Requirements:**
      - Choose a product domain and state its user, problem, and proposed value.
      - Add a semantic HTML page with header, navigation, main content, feature list, and footer.
    - **Acceptance criteria:**
      - [ ] The HTML uses semantic elements and has a logical heading order.
    - **Submission:**
      - Screenshot of the HTML page.
      - Short note describing the chosen product domain.
12. Toward the end of your step, and before your online presentation, attend a technical session with one of your track’s technical mentors and receive their feedback.
13. At least 10 days before your deadline, start coordinating and scheduling your live presentation session as the final task of this step.  
    For more details about the live presentation, please check ["Delivering an Online Presentation"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Delivering%20an%20Online%20Presentation%20--%20fa.md).
14. Hold your live presentation on LinkedIn.
