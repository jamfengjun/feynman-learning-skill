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

5. **Verify before confidence**
   - Separate what came from user-provided material, what is general background knowledge, what is inferred, and what must be verified.
   - For high-stakes or changing domains, verify with current authoritative sources before giving a firm conclusion.

## Anti-Hallucination Protocol

Use this protocol whenever the task touches medicine, law, finance, policy, current technology, company facts, market data, academic claims, or any claim the user may rely on externally.

1. **Classify each important claim**
   - Fact: directly supported by source material or reliable references.
   - Interpretation: the agent's explanation of facts.
   - Assumption: plausible but not yet proven.
   - Open question: cannot be answered safely without more evidence.

2. **Source discipline**
   - Prefer the user's original material first.
   - For current or high-risk facts, use authoritative sources: official documentation, laws/regulations, clinical guidelines, peer-reviewed papers, standards bodies, or primary company filings.
   - Do not cite a source as supporting a claim unless the source actually supports that claim.

3. **No invention rule**
   - Do not invent customer cases, revenue, partnerships, clinical results, certifications, policy text, citations, paper findings, or implementation details.
   - Use "待验证", "假设", "示例占位", or "需要补充证据" instead of filling gaps with confident prose.

4. **Confidence control**
   - Give confidence levels for research or decision outputs: high, medium, low.
   - Explain confidence in one sentence: evidence strength, source quality, recency, and whether the claim depends on context.

5. **Feynman gap check**
   - If an explanation relies on vague phrases such as "显著提升", "行业领先", "临床验证充分", "安全可靠", or "政策支持", ask what metric, comparator, population, date, standard, or source proves it.
   - If a term cannot be explained plainly, define it or mark it as a gap before using it in conclusions.

## Professional Domains

### Computer Science And AI

When explaining algorithms, systems, models, APIs, or software architecture:

- Split the answer into mechanism, input/output, assumptions, failure modes, and minimal example.
- For current APIs, libraries, model capabilities, benchmarks, or security guidance, check official docs or primary papers.
- Distinguish conceptual explanation from production implementation advice.
- Include edge cases and what would falsify the explanation.

### Medicine And Health AI

When explaining disease, diagnosis, treatment, clinical workflow, medical devices, or health AI:

- Prefer clinical guidelines, consensus statements, systematic reviews, drug labels, or official health agencies.
- Separate mechanism explanation from clinical recommendation.
- Use conservative medical AI language: auxiliary screening, trend observation, risk stratification, clinician review, not a replacement for diagnosis or treatment.
- State when a claim needs validation by clinical study, sample size, population, endpoint, and comparator.
- Include safety boundaries and referral/doctor-review language when user-facing.

### Cross-Disciplinary Work

For topics like medical AI, digital health, computational biology, health economics, or regulated software:

- Build a two-column map: domain facts on one side, technical claims on the other.
- Identify translation risks where one field's term may mean something different in the other.
- Mark regulatory, ethical, data quality, bias, and deployment risks separately from scientific validity.

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
- Evidence map: known, uncertain, missing, source needed
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
- Treat "simple explanation" as a test of understanding, not permission to remove evidence or uncertainty.
- Make the explanation shorter only after it is accurate.
- If a term cannot be explained simply, define it or flag it as a knowledge gap.
- For Chinese business or formal contexts, default to professional, direct, high-density wording.
- When the task is external-facing, produce a polished version the user can send or speak from directly.

## Feynman Case Patterns

Use these patterns as examples of the method in action.

### Concept Learning Case

Topic: gradient descent.

- Plain explanation: imagine walking downhill in fog; each step checks which direction lowers the height most.
- Gap check: if "gradient" cannot be explained, define it as the direction and size of fastest change.
- Rebuild: connect learning rate, local minima, and over-shooting to the hill-walking example.

### Medical AI Case

Topic: AI tongue image analysis for diabetes management.

- Plain explanation: tongue images may provide auxiliary body-state signals, but blood glucose and HbA1c remain the clinical anchors.
- Gap check: ask whether there is validated evidence linking image features to outcomes in the target population.
- Rebuild: position the tool as auxiliary screening or trend observation with clinician review, not independent diagnosis.

### Business Negotiation Case

Topic: hospital pilot for an AI health-management tool.

- Plain explanation: the value is not "AI is advanced"; the value is reducing follow-up workload and finding risk signals earlier.
- Gap check: prove data security, workflow fit, clinical boundary, and measurable pilot endpoints.
- Rebuild: ask for a small pilot with agreed metrics before discussing broader procurement.

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

### Evidence Map Template

```markdown
事实：

解释：

假设：

待验证：

高风险结论：

置信度：
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
