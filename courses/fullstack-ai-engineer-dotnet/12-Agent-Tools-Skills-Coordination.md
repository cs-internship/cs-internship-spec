## Step 12. Agent Tools, Skills, and Coordination

<!-- outcomes: DOTNET-AI-05 DOTNET-AI-06 DOTNET-AI-07 DOTNET-AI-09 -->

Turn the first product agent into an actor: agents call controlled tools, package reusable skills, coordinate as specialized teams, and expose auditable decision traces while the portfolio application stays in charge.

### Study Items  <!-- omit in toc -->

#### .NET AI

1. Call controlled tools from an agent and compare the `AIAgent`, `ChatClientAgent`, and `HarnessAgent` abstractions ([Tool Calling](https://www.youtube.com/watch?v=gJTodKpv8Ik), [Advanced Tool Calling](https://www.youtube.com/watch?v=dCtojrK8bKk), [AIAgent vs ChatClientAgent](https://www.youtube.com/watch?v=pN-WV5FD_-Y), [Current Agent Framework tools](https://learn.microsoft.com/en-us/agent-framework/agents/tools/), [Agent Harness](https://learn.microsoft.com/en-us/agent-framework/concepts/harness))
2. Connect tools exposed through the Model Context Protocol to an agent ([MCP Tool Calling](https://www.youtube.com/watch?v=Y5IKdt9vdJM), [Current Agent Framework tools](https://learn.microsoft.com/en-us/agent-framework/agents/tools/))
3. Package a reusable capability with the current Agent Skills provider ([Skills in C#](https://www.youtube.com/watch?v=KHfJko3msLw), [Current Agent Skills guidance](https://learn.microsoft.com/en-us/agent-framework/agents/skills))
4. Coordinate specialized agents using structured output, agent-as-tool composition, and justified concurrent or handoff patterns ([Multi-Agent and Workflows](https://www.youtube.com/watch?v=lIXJovzXNh4), [Structured Output](https://www.youtube.com/watch?v=2YzjRZTZxUo), [Agent as a tool](https://www.youtube.com/watch?v=wL4V78s_wI4), [Concurrent workflow](https://www.youtube.com/watch?v=qYxGJ-D3Tl0), [Handoff workflow](https://www.youtube.com/watch?v=VInKZ45YKAM), [Current workflow concepts](https://learn.microsoft.com/en-us/agent-framework/concepts/workflows/))
5. Explain reasoning effort, overthinking, latency, token cost, and what reasoning may be exposed, then distinguish private model reasoning from auditable inputs, outputs, tool calls, results, retries, and traces ([Reasoning Deep Dive Part 1](https://www.youtube.com/watch?v=pD3A3rC_D5Q), [Agent tracing overview](https://learn.microsoft.com/en-us/azure/foundry/observability/concepts/trace-agent-concept), [AI-system observability](https://learn.microsoft.com/en-us/security/zero-trust/sfi/observability-ai-systems))
6. Explain direct and indirect prompt injection through user input and tool or document content, test the product agent with one crafted injection attempt, and document which constraints, least-privilege tools, and approval gates stopped it ([Tool approval](https://learn.microsoft.com/en-us/agent-framework/agents/tools/tool-approval), [Agent Framework transparency FAQ](https://github.com/microsoft/agent-framework/blob/main/TRANSPARENCY_FAQS.md))
7. Expose the application's read-only operations as MCP server tools using the C# MCP SDK, connect a coding agent to them, and record which operations were deliberately withheld ([Model Context Protocol](https://modelcontextprotocol.io/), [Current Agent Framework tools](https://learn.microsoft.com/en-us/agent-framework/agents/tools/))

### Tasks  <!-- omit in toc -->

1. **Give the Product Agent Tools** <!-- bc: 11-T1 -->
   - **Goal:** Let the agent complete real product work through a least-privilege tool set.
   - **Deliverable:** Tool-enabled agent, tool contracts, one MCP or externally exposed tool with justification, evaluation cases, and an observable decision trace.
   - **Requirements:**
     - Expose application operations as tools restricted to the minimum actions required.
     - Separate read-only tools from state-changing tools and gate the state-changing ones behind the approval path defined earlier.
     - Include at least one MCP tool, or document why MCP was not applicable.
     - Record tool calls, results, and failures without logging secrets or private data.
   - **Acceptance criteria:**
     - [ ] The agent completes a product task that requires at least two different tools.
     - [ ] State-changing actions cannot run without the documented approval path.
     - [ ] A failing tool produces a controlled agent response rather than a crash.
     - [ ] The decision trace records tool-selection rationale, calls, results, and failures for each run without exposing secrets or private chain-of-thought.
   - **Submission:**
     - Tool contracts, approval path documentation, and decision traces.
2. **Package a Reusable Agent Skill** <!-- bc: 11-T2 -->
   - **Goal:** Capture one product capability as a reusable, documented agent skill.
   - **Deliverable:** Version-pinned Agent Skills configuration, a packaged skill with instructions and resources, usage examples, and a comparison of agent behavior with and without the skill.
   - **Requirements:**
     - Define the skill purpose, inputs, and boundaries in its instructions.
     - Keep skill content versioned with the application.
     - Demonstrate the skill improving at least one measurable agent behavior.
   - **Acceptance criteria:**
     - [ ] The skill is discovered and used by the agent without code changes.
     - [ ] The with-and-without comparison shows an observable difference.
     - [ ] Skill content contains no secrets or private user data.
   - **Submission:**
     - Packaged skill and with-and-without comparison.
3. **Coordinate a Multi-Agent Workflow** <!-- bc: 11-T3 -->
   - **Goal:** Decompose one product scenario across specialized cooperating agents.
   - **Deliverable:** Multi-agent orchestration, structured output contracts between agents, a full run transcript, and an explanation of each agent's decisions.
   - **Requirements:**
     - Assign each agent one clear role and a documented contract.
     - Pass data between agents using validated structured output.
     - Compose agents directly or through the workflow built in the previous step.
     - Capture a complete run showing inputs, tool use, handoffs, and the final output.
   - **Acceptance criteria:**
     - [ ] The coordinated run integrates at least two specialized roles whose outputs are separately validated before the final result.
     - [ ] Invalid structured output is rejected rather than passed downstream.
     - [ ] The transcript attributes each decision and tool call to a named agent.
     - [ ] The explanation identifies at least one way the design can fail and how that failure is handled.
   - **Submission:**
     - Multi-agent orchestration, run transcript, and decision explanation.
4. Toward the end of your step, and before your online presentation, attend a technical session with one of your track’s technical mentors and receive their feedback.
5. At least 10 days before your deadline, start coordinating and scheduling your live presentation session as the final task of this step.  
   For more details about the live presentation, please check ["Delivering an Online Presentation"](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Delivering%20an%20Online%20Presentation%20--%20fa.md).
6. Hold your live presentation on LinkedIn.
