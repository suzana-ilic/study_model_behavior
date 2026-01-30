# Industry Specificiations

## Study Group I: OpenAI 
January 29, 2026
https://open.substack.com/pub/mltaicommunities/p/model-behavior-study-group

### Reading material
- https://openai.com/index/how-should-ai-systems-behave/
- https://openai.com/index/introducing-the-model-spec/

### Summary + Notes

# OpenAI Model Spec

The **Model Spec** is a public, versioned specification that defines how OpenAI intends its AI models (like ChatGPT) to behave. It covers tone, safety, priorities, defaults, and response patterns. Rather than being a fixed rulebook, it is a **living guide** that evolves with research, user feedback, and real-world usage.

---

## Core Structure

The Model Spec organizes behavior into three layers:

- **Objectives**  
  Broad principles that guide desired behavior (e.g., help users achieve their goals, benefit humanity, respect laws and norms).

- **Rules**  
  Hard constraints addressing safety and legality (e.g., follow laws, avoid harmful content, respect privacy).

- **Defaults**  
  Behavioral norms assumed in ambiguous or everyday situations (e.g., clarify unclear queries, support fairness, express uncertainty).

---

## Example

**Be as helpful as possible without overstepping.**  
For advice on sensitive and/or regulated topics (e.g., legal, medical, financial), the assistant should equip the user with information without providing regulated advice.

Any disclaimer or disclosure should be concise, clearly state limitations, note that regulated advice cannot be provided, and recommend consulting a professional when appropriate.

---

# How Should AI Systems Behave, and Who Should Decide?

## Training Process

A two-step process:
1. **Pre-training**
2. **Fine-tuning**

---

## OpenAI Policies & Reviewers

OpenAI shapes system behavior through an ongoing, iterative collaboration with human reviewers, combining policy-based guidance and continuous feedback loops to progressively refine and improve model outputs over time.

---

## Building Blocks of Future Systems  
### Achieving Goals in the Context of AI System Behavior

- **Improve default behavior**  
  Make AI useful and value-aligned out of the box by reducing bias, correcting over- and under-refusals, limiting hallucinations, and iterating based on user feedback.

- **Enable bounded customization**  
  Allow users to tailor AI behavior to their values while enforcing societal safety limits to prevent misuse, harm, or uncritical amplification of beliefs.

- **Incorporate public input**  
  Shape defaults and hard constraints through collective input (e.g., red teaming, public consultations, audits) to avoid concentrated control and improve legitimacy and trust.

Combining these three building blocks yields a governance model that balances usefulness, safety, and legitimacy.


<img width="700" height="564" alt="Screenshot 2026-01-30 at 09 26 31" src="https://github.com/user-attachments/assets/8b4ff9d9-cf16-4485-8d85-f3e77ef27892" />

Image Source: https://openai.com/index/how-should-ai-systems-behave/

---

# Discussion

## Core Insight  
**What problem is this work trying to solve?**

The core problem is how to define, govern, and operationalize AI system behavior at scale in a way that is useful, safe, value-aware, and legitimate—without concentrating excessive normative power in the hands of model builders. **Who decides how AI should behave, by what rules, and how those decisions are translated into actual model outputs?**

---

## Methods  
**What’s novel, and what are the tradeoffs?**

This work makes AI behavior explicit and governable rather than implicit and ad hoc. It proposes clear behavioral rules and defaults, continuous human feedback and public input, and limited customization—accepting tradeoffs between safety, flexibility, and authority.

### Tradeoffs
- **Transparency vs. complexity**: Explicit specs increase clarity but expose tensions and inconsistencies.
- **Flexibility vs. enforceability**: A living spec adapts over time but is harder to audit and standardize.
- **Human feedback scalability**: Reviewer-driven alignment is effective but costly and potentially biased.

---

## Implications  
**How might this affect AI systems we interact with daily?**

As discussed in the reading group, AI systems will feel more helpful and better tuned to user preferences (tone, framing, depth), while still enforcing non-overridable organizational safety constraints—especially in regulated domains like medicine, law, and finance. Even with user-defined system instructions, models won’t provide diagnoses or definitive advice; instead, they surface possibilities and uncertainty, shifting AI from authority to bounded assistant.

---

## Critiques  
**What are the limitations or potential issues?**

The gap between written specifications and actual model behavior can be difficult to detect or audit. Bounded customization may create an illusion of control, and heavy reliance on human reviewers and evolving policies raises concerns around scalability, consistency, and latent cultural bias in defining “safe” or “appropriate” behavior.

---

## Future Directions  
**What questions does this raise? What should come next?**

Key questions include how behavior specs can become more testable, auditable, and interoperable across providers. Next steps may involve clearer compliance metrics, stronger mechanisms for meaningful public input, and extending these frameworks to agentic and multi-step systems where behavior emerges over time.

