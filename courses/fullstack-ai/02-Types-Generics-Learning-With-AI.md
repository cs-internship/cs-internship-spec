## Step 2. Types, Generics, and Learning with AI

<!-- outcomes: AI-05 AI-06 AI-07 AI-08 -->

Learn how the C# type system and generics shape your code, and practice debugging it. In parallel, learn how to learn and research with AI: compare guided study with direct answers, build a source-grounded notebook, run the same question through two deep-research tools, and verify the claims before you use them to scope the next feature of your portfolio application.

### Study Items  <!-- omit in toc -->

#### C# Language

1. [C# book](https://www.oreilly.com/library/view/programming-c-12/9781098158354/), chapter 3 : Types
2. [What is debugging?](https://learn.microsoft.com/en-us/visualstudio/debugger/what-is-debugging?view=vs-2022)
3. [Tutorial: Learn to debug C# code using Visual Studio](https://learn.microsoft.com/en-us/visualstudio/get-started/csharp/tutorial-debugger?view=vs-2022&toc=%2Fvisualstudio%2Fdebugger%2Ftoc.json)
4. [First look at the Visual Studio Debugger](https://learn.microsoft.com/en-us/visualstudio/debugger/debugger-feature-tour?view=vs-2022)
5. [Use breakpoints in the Visual Studio debugger](https://learn.microsoft.com/en-us/visualstudio/debugger/using-breakpoints?view=vs-2022)
6. (Optional) [C# Breakpoints and Conditions](https://www.youtube.com/watch?v=YEL92u-3cRY)
7. (Optional) [How to Debug in Visual Studio](https://www.youtube.com/watch?v=__3wlUxMXlA)
8. [C# book](https://www.oreilly.com/library/view/programming-c-12/9781098158354/), chapter 4 : Generics
9. [Constraints on type parameters (C# Programming Guide)](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/generics/constraints-on-type-parameters)
10. [Differences Between C++ Templates and C# Generics (C# Programming Guide)](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/generics/differences-between-cpp-templates-and-csharp-generics)

#### General AI

1. Use Gemini text, file, image, model-selection, temporary-chat, Canvas, Guided Learning, and Deep Research features, then record which feature fits each learning or productivity goal ([Gemini Practical Course](https://www.youtube.com/watch?v=-_FizlRlfYs))
2. Conduct a guided Study Mode session with prior-knowledge questions, learner attempts, feedback, and a mastery check, then compare it with direct-answer chat using the same learning goal and criteria ([Introducing Study Mode](https://www.youtube.com/watch?v=XDYilxy1dn8), [Study Mode Guide](https://help.openai.com/en/articles/11780217-study-mode), [Evaluation best practices](https://developers.openai.com/api/docs/guides/evaluation-best-practices))
3. Build a source-grounded notebook, configure its sources and instructions, use cited chat, and verify important claims against the original material ([Gemini Notebook Integration](https://www.youtube.com/watch?v=Y-LTxr1bv9M), [Product Guide](https://support.google.com/gemininotebook/answer/16164461?hl=en))
4. Run the same question through two deep-research tools, then compare report scope, source selection and quality, citation traceability, and claims that fail source checks ([Gemini Practical Course](https://www.youtube.com/watch?v=-_FizlRlfYs), [Gemini Deep Research guide](https://support.google.com/gemini/answer/15719111?hl=en), [ChatGPT Deep Research](https://www.youtube.com/watch?v=YkCDVn3_wiw), [ChatGPT Deep Research guide](https://help.openai.com/en/articles/10500283-deep-research), [Lateral reading](https://cor.inquirygroup.org/curriculum/collections/teaching-lateral-reading/), [Evaluation best practices](https://developers.openai.com/api/docs/guides/evaluation-best-practices))

### Tasks  <!-- omit in toc -->

1. As part of the **Mentor Training** path, watch the **fifth** of the eight videos in the **Communication Training** course using [this link](https://drive.google.com/file/d/1ncbYej5CvvJNVu6GlnKFTxxJ7iYjVXv0/view?usp=sharing). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
2. As part of the **Mentor Training** path, watch the **sixth** of the eight videos in the **Communication Training** course using [this link](https://drive.google.com/file/d/1L-xFO4gbmBmxepTldUT61_HuA4d3T9eU/view?usp=sharing). To complete this task, please follow the instructions provided on [this page](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md).
3. Pass all lessons on TypingClub.com **with 5 stars** up to lesson 137.
4. Choose 3 bloggers who write about C# and describe why they matter to you.
5. Search for dotPeek, what is it? Open and investigate one of your program dlls that you have written so far.
6. Pass these exercises at exercism.io:
   - Allergies
   - Clock
   - Circular Buffer
   - Pangram
   - Pascal's Triangle
7. Project: Calculator Console Application
   - Create a console application that performs basic arithmetic operations (addition, subtraction, multiplication, and division) on two numbers entered by the user.
     - The application should prompt the user to enter two numbers.
     - The application should then prompt the user to choose an operation: addition, subtraction, multiplication, or division.
     - The application should perform the chosen operation and display the result.
     - The application should handle invalid inputs (e.g., division by zero).
8. Project: Create a simple library system to store and manage different types of library items (e.g., books, magazines, DVDs). (This project will help you understand and work with generics in C#)
   - Your project should have the following components:
       - `LibraryItem<T>`: A generic class representing an item in the library.
       - `Library`: A class containing a generic method to add items to a collection.
       - `LibraryManager`: The main class to manage library items and demonstrate the use of generic collections.
9. **Produce a Source-Grounded Feature Brief** <!-- bc: 03-T1 -->
   - **Goal:** Use research evidence to choose and scope the next product feature.
   - **Deliverable:** `docs/feature-research.md`, a Gemini feature-selection log, a guided-versus-direct Study Mode comparison, and a shareable notebook link or export.
   - **Requirements:**
     - Use a source-grounded notebook with organized sources and explicit notebook instructions, plus two deep-research tools.
     - Verify at least five important claims against original sources.
     - Include one Study Mode session with prior-knowledge questions, learner attempts, feedback, and a mastery check.
     - Record which Gemini features were used, which were rejected, and why each selected interaction fit the learning goal.
     - If a named tool is unavailable, document the limitation and use a technical mentor-approved equivalent with the same evidence requirements.
   - **Acceptance criteria:**
     - [ ] Every central claim has a traceable source.
     - [ ] The recommendation distinguishes evidence from inference.
     - [ ] The brief records at least one limitation or unresolved question.
     - [ ] The notebook exposes citations that resolve to its original sources.
     - [ ] The Study Mode comparison distinguishes guided learning from direct-answer behavior.
   - **Submission:**
     - `docs/feature-research.md`, Gemini feature-selection log, Study Mode comparison, and notebook link or export.
   - **Tip:** You can use this step's C# topic, such as generics, as the learning goal of the Study Mode session.
10. Toward the end of your step, and before your online presentation, attend a technical session with one of your track’s technical mentors and receive their feedback.
11. At least 10 days before your deadline, start coordinating and scheduling your live presentation session as the final task of this step.  
    For more details about the live presentation, please check ["Delivering an Online Presentation"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Delivering%20an%20Online%20Presentation%20--%20fa.md).
12. Hold your live presentation on LinkedIn.
