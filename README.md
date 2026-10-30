# Prompts & Evaluation Guide

---

## 1. Model A and Model B — Individual Comments Filling

```text
You are an expert evaluator reviewing the full lifecycle of a model's performance in a multi-turn task.

Your evaluation must be based ONLY on:
1. The Initial Prompt and GOAL
2. Turns (follow-up prompts(turns) after initial prompt across the session)
3. A complete explanation of the model's behavior (planning, execution, logs, issues, decisions, mistakes, etc...)

Also inside this project files analyse the preference-rating.txt file to know more.

Mainly, inside this project files we have a reference-example-excalidraw.txt, which is a 5-star review.
This reference is ONLY for writing style and tone — NOT for rating decisions.

Also use reference-example-excalidraw.txt as an additional guide — the natural, human-written comment style shown there is the quality bar to match, again for tone and writing style only, not for rating decisions or content.

-----------------------------------
CRITICAL INSTRUCTIONS
-----------------------------------

1. Reference Usage:
- Use the reference ONLY to understand tone and writing style
- DO NOT copy content
- DO NOT let it influence ratings

2. Behavioral Issues Constraint:
- Any behavioral issue you mention MUST come strictly from the explanation I provide
- DO NOT invent, assume, or add new issues
- DO NOT exaggerate or generalize beyond given evidence

-----------------------------------
YOUR RESPONSIBILITIES
-----------------------------------

You must analyze:
- Planning quality
- Execution across turns
- Instruction adherence
- Handling of constraints and safety
- Logs, errors, and recovery behavior
- Consistency across the entire session

-----------------------------------
PART 1: HUMAN-LIKE COMMENTS
-----------------------------------

Fill all comment fields with NATURAL, HUMAN-WRITTEN feedback.

Style guidelines:
- Write as if you personally reviewed the session
- Keep it clear, conversational, and realistic
- Avoid robotic or repetitive phrasing
- Use natural variation in sentences
- Be specific and grounded in actual observations

The tone should feel similar to the reference,
BUT the content must be fully original and based only on the given data.

-----------------------------------
PART 2: ACCURATE RATING
-----------------------------------

You must:
- Rate strictly based on actual performance
- NOT inflate scores
- Ensure ratings match the evidence
- Reflect reasoning naturally inside the comments

-----------------------------------
IMPORTANT RULES
-----------------------------------

- Do NOT hallucinate any details
- Do NOT introduce new behavioral issues
- Do NOT generalize without evidence
- Do NOT over-explain
- Stay fully grounded in the provided turns and explanation

-----------------------------------
INPUT FORMAT
-----------------------------------

I will provide:
1. Model Name(A or B)
2. Initial Prompt
3. Follow-up prompts(Turns) (multi-turn prompts)
4. Full explanation (including behavioral issues, if any)
5. Reference image (tone only)

-----------------------------------
OUTPUT FORMAT
-----------------------------------

- Fully filled comment sections
- Natural, human-like writing
- Accurate and justified ratings


Input :-
Model :


GOAL :


Initial Prompt :


Follow-up prompts(Turns) :


Explanation:


```

---

## 2. Models Comparison — Head-to-Head Comments Filling

```text
You are an expert evaluator comparing Model A and Model B based on their completed evaluations.

Your task is to write detailed, human-like feedback for the following sections:

1. Overall Preference Comments
2. Instruction Following Comments
3. Time to Resolution Comments
4. Vibes Comments

Also inside this project files analyse the preference-rating.txt file to know more.

Mainly, inside this project files we have a reference-example-excalidraw.txt, which is a 5-star review.
This reference is ONLY for writing style and tone — NOT for rating decisions.

Also use reference-example-excalidraw.txt as an additional guide — the natural, human-written comment style shown there is the quality bar to match, again for tone and writing style only, not for decision-making.

-----------------------------------
CRITICAL RULES
-----------------------------------

1. REFERENCE USAGE
- Use it ONLY to match tone (natural, smooth, human-like)
- DO NOT copy structure or phrases
- DO NOT assume high ratings because of it

2. NO VAGUE OR GENERIC FEEDBACK
- Every statement must be meaningful, specific, and supported by evidence
- Always explain:
  - What happened
  - Why it mattered
  - How it affected the evaluation
- Connect observations directly to the rating or preference
- Include strengths and weaknesses when relevant
- Use concrete examples from the evaluation whenever available

Good feedback:
- References specific model behaviors
- Explains how those behaviors aligned or conflicted with requirements
- Connects observations to outcomes
- Makes the reasoning behind the judgment easy to understand

Avoid feedback that:
- Uses vague terms such as "good", "okay", "better", "nice", "solid", or "poor" without explanation
- Makes conclusions without evidence
- States that instructions were followed or missed without describing how
- Relies on generic praise or criticism that could apply to any model
- Focuses on impressions without connecting them to observable behavior

Examples of weak feedback:
- "Model A did okay overall."
- "Model B was better."
- "The responses felt more professional."
- "It followed instructions reasonably well."
- "The work was not very good."

These statements are insufficient unless supported by specific evidence and reasoning.

3. NO REPETITION ACROSS SECTIONS
- Each section must provide a distinct perspective
- Do not recycle the same justification across multiple sections
- If a behavior is mentioned again, discuss it from a different angle and explain a different impact
- Avoid repeating identical strengths, weaknesses, or conclusions

4. STRICT CONSISTENCY
- Base everything ONLY on the provided Model A and Model B evaluations
- Do NOT introduce assumptions, speculation, or new claims
- Every major observation should be traceable to the evaluation materials
- The written comments must fully justify the stated preference
- The explanation should make it clear why one model was preferred over the other
- Ensure the reasoning, evidence, and preference all align with each other

-----------------------------------
WRITING STYLE (VERY IMPORTANT)
-----------------------------------

- Fully human-written tone (like a real reviewer)
- Clear, simple, and easy to understand
- Slightly more descriptive, but NOT verbose
- 2–3 paras per section (ideal range)
- Natural flow, not bullet-point robotic writing

-----------------------------------
DEPTH EXPECTATION
-----------------------------------

Each section should:
- Compare both models briefly
- Clearly indicate which one is better
- Highlight some specific differences
- Explain why that difference matters in practice

-----------------------------------
SECTION GUIDANCE
-----------------------------------

1. Overall Preference Comments
- Big picture: reliability, correctness, completeness
- Which model you would trust more and why

2. Instruction Following Comments
- Adherence to requirements
- Missed constraints, correctness, discipline

3. Time to Resolution Comments
- Efficiency of reaching a stable solution
- Rework, delays, unnecessary steps

4. Vibes Comments
- Clarity, confidence, readability
- How trustworthy and polished the responses felt

-----------------------------------
OUTPUT FORMAT
-----------------------------------

Overall Preference Comments:
<2–3 paras, natural and descriptive>

Instruction Following Comments:
<2–3 paras, clear and grounded>

Time to Resolution Comments:
<2–3 paras, focused on efficiency>

Vibes Comments:
<2–3 paras, subjective but justified>

-----------------------------------
FINAL CHECK BEFORE OUTPUT
-----------------------------------

- Does each section feel written by a human?
- Is there any vague statement? (If yes → fix it)
- Any repeated phrasing across sections? (If yes → rewrite)
- Is the preference clearly justified?

IMPORTANT : MUST BE LIKE HUMAN WRITTEN TEXT....NO POSH ENGLISH...

--
Inputs are the above model a and model b comments.. and explanation and turns and goals and images provided...
```
