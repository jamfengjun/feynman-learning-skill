---
name: feynman-learning
description: Use this skill when the user wants to learn, research, explain, teach, prepare a speech, simplify complex material, test understanding, create study notes, build a presentation narrative, or prepare a business negotiation using the Feynman learning method. Also use when the user asks to "用费曼学习法", "讲明白", "蒸馏概念", "把复杂内容讲给外行", "准备演讲", "准备谈判", "研究一个主题", or turn messy source material into clear explanation, questions, objections, and action points.
---

# Feynman Learning

## Core Loop

Use the Feynman method as a clarity engine, not a school-note template.

1. **Name the target**
   - Define the exact topic, claim, decision, audience, and expected output.
   - If the target is vague, ask one concise clarification before proceeding.

2. **Explain in plain language**
   - Explain the idea as if speaking to a smart beginner.
   - Prefer concrete examples, cause-and-effect chains, and everyday analogies.
   - Avoid jargon unless it is the object of explanation.

3. **Expose gaps**
   - List what is unclear, unsupported, assumed, contradictory, or hard to explain.
   - Convert each gap into a question, verification task, or missing evidence item.

4. **Rebuild for use**
   - Rewrite the explanation for the user's task: learning note, research map, speech, negotiation brief, Q&A, or decision memo.
   - Preserve nuance; do not oversimplify important tradeoffs.

## Output Selection

Choose the output shape based on the user's intent.

### Learning

Use when the user wants to understand a concept, book, paper, course, framework, or unfamiliar domain.

Return:

- One-sentence essence
- Plain-language explanation
- Key concepts and their relationships
- Minimal example
- Common misunderstandings
- Self-test questions
- Remaining gaps or next reading targets

### Research

Use when the user wants to investigate a topic, industry, company, policy, technology, market, or academic question.

Return:

- Research question
- Current best explanation
- Evidence map: known, uncertain, missing
- Competing hypotheses or viewpoints
- Terms that need precise definitions
- What to verify next
- Draft conclusion with confidence level

When the user needs current facts, market conditions, regulations, prices, recent papers, or live company information, verify with current sources before presenting conclusions.

### Speech And Teaching

Use when the user prepares a talk, class, presentation, interview answer, investor pitch, or public explanation.

Return:

- Audience and desired shift in belief or action
- Core message
- Opening hook
- Explanation ladder: simple premise -> mechanism -> example -> implication
- Story or analogy
- Slide or section outline
- Likely audience questions
- Short closing line

Keep spoken language natural. Replace abstract nouns with active sentences whenever possible.

### Business Negotiation

Use when the user prepares a sales conversation, partnership discussion, investor meeting, procurement negotiation, internal persuasion, or difficult stakeholder conversation.

Return:

- Objective and minimum acceptable outcome
- Other party's likely incentives, fears, and constraints
- Plain explanation of the value proposition
- Points that must be proven
- Likely objections and responses
- Questions to ask before making concessions
- Concession ladder: give, ask, hold
- Closing script or next-step proposal

Do not invent facts, customer cases, revenue, certifications, partnerships, or commitments. Mark unsupported claims as assumptions or placeholders.

## Reasoning Rules

- Start from the user's source material when provided; do not replace it with generic theory.
- Distinguish facts, interpretations, assumptions, and open questions.
- Make the explanation shorter only after it is accurate.
- If a term cannot be explained simply, define it or flag it as a knowledge gap.
- For Chinese business or formal contexts, default to professional, direct, high-density wording.
- When the task is external-facing, produce a polished version the user can send or speak from directly.

## Useful Templates

### Explanation Template

```markdown
一句话本质：

通俗解释：

为什么重要：

例子：

容易误解的地方：

我还需要确认：
```

### Gap Audit Template

```markdown
我能讲清楚的：

我讲不清楚的：

缺少的证据：

可能的反例：

下一步验证：
```

### Negotiation Template

```markdown
我方目标：

对方真正关心：

一句话价值：

必须证明：

可能反对：

回应口径：

可让步：

不能让：

下一步话术：
```
