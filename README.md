# Agent338 — Humanities base argument prototype

This repository holds a **Cursor Agent + Skill** prototype for a structured conversation about a student’s **base argument** (thesis, scope, objections, evidence) in humanities writing.

## What’s in the repo

| Item | Purpose |
|------|--------|
| `.cursor/skills/base-argument-conversation/SKILL.md` | Main skill: when to run it, conversation flow, recap format |
| `.cursor/skills/base-argument-conversation/examples.md` | Sample prompts and an illustrative exit recap |
| `.cursor/rules/humanities-argument-prototype.mdc` | Always-on guardrails (Socratic coaching, no full-essay drafting) |

## Prerequisites

- [Cursor](https://cursor.com) installed
- This folder opened as the **workspace root** in Cursor (so project skills and rules load)

## How to use it

1. **Open the project**  
   `File → Open Folder…` and select the `Agent338` directory.

2. **Start Agent chat**  
   Open the Agent (Composer) panel—not Ask mode—so the agent can follow project context, skills, and rules.

3. **Trigger the behavior**  
   Say that you want to work on your **argument**, **thesis**, or **base claim**, for example:
   - “Let’s stress-test my base argument for this paper.”
   - “I want a Socratic conversation about my thesis before I draft.”

   Paste what you have, ideally in one message:
   - Assignment prompt (and genre/length if relevant)
   - Your **current thesis** (one sentence) **or** bullet claims / short excerpt
   - Optional: rubric snippet or what the instructor emphasizes
   - Optional: draft stage (outline vs. partial vs. near-final)

4. **Follow the dialogue**  
   The skill steers **4–6 turns**: clarify thesis → stakes → premises → steel-man objection → key terms/scope → **recap** in a fixed markdown shape.

5. **If the skill doesn’t attach automatically**  
   Depending on your Cursor version, you can:
   - Repeat trigger phrases from the skill’s description (thesis, argument, humanities essay, stress-test claim), or
   - Use `@` to mention the skill if it appears in the context picker, or
   - Paste the path `.cursor/skills/base-argument-conversation/SKILL.md` and ask the agent to follow it for this thread.

## Tips for demos / grading

- Run **two or three** sample theses (too broad, too vague, strong but thin evidence) and save **screenshots or exported chat** showing one full run through the **exit recap**.
- Keep the rule file enabled (`alwaysApply: true`) so behavior stays consistent for reviewers.

## Customizing

- Edit **`SKILL.md`** to change turn count, tone, or required inputs.
- Edit **`humanities-argument-prototype.mdc`** to relax or tighten ghostwriting guardrails for your course policy.

## License / course use

Adjust this section if your course requires a specific attribution or license statement.
