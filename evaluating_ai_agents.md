# Evaluating AI Agents

Community Notes from our study group, June 20, 2026

Deeplearning.ai -> [Go to course](https://www.deeplearning.ai/courses/evaluating-ai-agents)

Here's a synthesis of what the group landed on:

## Course assessment

Solid mental map for a 2-hour intro, well-organized and easy to follow (at least until Lab 1), but starts to get very dense especially from Lab 2 on tracing which felt rushed. Jupyter as a medium drew some grumbling, easy to follow along but introduce a need for more engaging hands-on alternatives. Concepts like "spans" need self-exploration to really stick. Useful as scaffolding for ongoing vibe-coded projects rather than a deep treatment. Tables printed in the small Jupyter notebooks embedded in the platform could be hard to read - with issues such as column shifts - as the number of table categories increase.

### Technical takeaways

- Error handling matters more than the course emphasizes — graceful failure ("if no analysis is returned") prevents cascading breakage downstream.
- Arize Phoenix is open source; the UI for organizing traces and spans used in the course.
- OTel appears to be the de facto tracing standard — the group flagged this as worth interrogating (are there real alternatives?).
- Building the agent is the easy part; observability is where the hard problems live.
- Contained execution environments for code-running agents were flagged as under-covered — possibly addressed later, possibly feedback for future iterations.
- Evaluation scope is categorized between LLM Model and LLM System; analogues with traditional software testing.
- Some metrics were listed; a comprehensive list might be useful for future studies.
- "even small changes can cause performance regressions".
- Simpler router = better & more consistent performance, but narrower capabilities - evaluation could helps close the gap.
- Splitting up tasks into two (or more) simpler tasks/calls is recommended compared to completing a single, more complex, difficult task.
- Modifying router entries is an interative feedback process to improve model capability.
- Code-based evals are especially useful to compare ground truth data with application output.

## Open questions the group surfaced

- Should graders be application-specific rather than generic?
- Need for more robust multi-judge setups — single LLM-as-judge feels thin.
- Evals for the tools an agent calls, not just the agent's outputs.
- Sycophancy / agreeableness wasn't mentioned — is it considered irrelevant in production, or just out of scope here?
- How do you evaluate generative tasks with a wide space of valid outputs (e.g., test case generation from PRDs) beyond basic LLM-as-judge?
- Always using discrete classification labels may not be the best idea?

## Idea floated
- Releasing something as an open-source agent / project off the back of the group's exploration.
