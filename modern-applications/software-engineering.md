# Software Engineering

Software engineering provides a practical environment for applying philosophical habits of definition, decomposition, reasoning, testing, error analysis, and system design.

The goal is not to turn classical philosophy into programming doctrine. It is to use its analytical discipline to improve engineering thinking.

---

# 1. Software as Structured Reasoning

A software system can be analyzed as:

```text
Requirements
 ↓
Definitions
 ↓
Model
 ↓
Design
 ↓
Implementation
 ↓
Testing
 ↓
Observation
 ↓
Revision
```

Errors introduced early can propagate through the entire system.

---

# 2. Requirements as Definitions

Many software failures begin with unclear requirements.

Ask:

- What exactly is required?
- What is excluded?
- What assumptions are being made?
- What counts as success?
- What are edge cases?

This is closely related to the philosophical discipline of precise definition.

---

# 3. Domain Modeling

Before implementation:

```text
Entities
Properties
Relations
Constraints
Operations
States
```

This resembles an ontological analysis:

```text
What exists?
What properties does it have?
How are entities related?
What can change?
What cannot change?
```

The analogy is methodological, not doctrinal.

---

# 4. Types and Categories

Type systems force distinctions such as:

```text
User
Order
Payment
Document
Message
```

Good type design prevents invalid combinations.

This is useful training for categorical thinking:

> What belongs to a class, and what does not?

---

# 5. Relations

Database and object models depend upon relations.

Use:

```text
Entity A
  │
  │ relation
  ▼
Entity B
```

Then specify:

- cardinality;
- ownership;
- dependency;
- lifecycle;
- constraints.

This pairs naturally with the analytical study of relations.

---

# 6. Inference in Debugging

Debugging can be treated as diagnostic inference.

```text
Observed symptom
 ↓
Possible causes
 ↓
Evidence
 ↓
Elimination
 ↓
Most supported explanation
 ↓
Test
 ↓
Result
```

This is not identical to Nyāya *anumāna*, but the reasoning discipline is highly compatible.

---

# 7. Counterexample Testing

For every function, ask:

```text
Normal input
Boundary input
Empty input
Invalid input
Unexpected input
Adversarial input
```

A single counterexample can expose an overgeneralized assumption.

---

# 8. Testing as Epistemic Discipline

A test does not automatically prove that software is correct.

It provides evidence under specified conditions.

Distinguish:

```text
Test passed
      ≠
System is universally correct
```

Testing increases confidence within a domain.

---

# 9. Invariants

An invariant is a property that should remain true under specified operations.

For example:

```text
Balance ≥ 0
```

if the system's domain requires it.

A useful reasoning pattern:

```text
Initial invariant
 ↓
Operation
 ↓
Proof / test that invariant is preserved
```

---

# 10. Architecture and Modularity

Separate concerns:

```text
Input
 ↓
Domain logic
 ↓
Persistence
 ↓
External services
 ↓
Presentation
```

Clear boundaries reduce hidden dependencies.

---

# 11. AI Systems

For an AI application, separate:

```text
Input
 ↓
Retrieval
 ↓
Evidence
 ↓
Reasoning
 ↓
Verification
 ↓
Generation
 ↓
Logging
```

Do not make the language-generation component the sole source of truth.

---

# 12. Technical Decision Record

For important architecture decisions:

```text
Decision:

Problem:

Constraints:

Options:

Evidence:

Assumptions:

Trade-offs:

Rejected alternatives:

Reason for choice:

Future reversal cost:
```

This turns implicit reasoning into inspectable reasoning.

---

# 13. Error Taxonomy

When a system fails, classify the failure:

```text
Requirement error
Model error
Design error
Implementation error
Integration error
Data error
Operational error
User-interface error
```

Do not patch symptoms without identifying the layer where the error originated.

---

# 14. Practical Project

Build a small local application and maintain four artifacts:

### 1. Domain model

What exists?

### 2. Decision log

Why was each design choice made?

### 3. Test suite

What evidence supports correctness?

### 4. Failure log

What assumptions failed?

This creates a practical laboratory for analytical thinking.

---

# 15. Code Review Method

For every significant change ask:

```text
What problem does this solve?
What assumptions does it introduce?
What invariant must remain true?
What could break?
What test demonstrates correctness?
What simpler alternative exists?
```

---

# 16. Software and Philosophical Precision

Useful habits include:

- define terms before implementation;
- distinguish entities from properties;
- distinguish relations from attributes;
- expose assumptions;
- test generalizations;
- preserve provenance;
- document uncertainty;
- make reasoning inspectable.

---

# Recommended Connections

- `inference.md`
- `relationships.md`
- `ontology.md`
- `critical-thinking.md`
- `ai.md`
- `decision-theory.md`

---

# Core Principle

> **Good software engineering is partly the discipline of turning vague assumptions into explicit definitions, models, constraints, tests, and decisions.**
