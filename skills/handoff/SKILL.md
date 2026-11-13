---
name: handoff
description: Prepare, on request, a handoff prompt to copy into a new conversation with an agent. Use it to hand over work, switch sessions, or continue working with fresh context. Respond in the conversation, without creating a file or launching an agent.
---

# Handoff — hand over to a new session

## Purpose

Enable an agent that cannot access this conversation to resume the work without having to explain everything again. Pass on the useful context, decisions, and next action, not the entire history.

## Preparation

1. Identify the work to continue and the expected outcome. If the user specifies a goal for the new session, focus the handoff on that goal.
2. Review the available exchanges. Keep the latest instructions and explicitly approved decisions; distinguish unapproved proposals.
3. Separate what is finished, in progress, still to do, or blocked. For checks, specify what was actually tested and what was not.
4. Keep important constraints, relevant preferences, and useful reasons behind choices. Do not include internal reasoning or a detailed account of attempts.
5. List the necessary references: files, folders, deliverables, sources, or skills that have actually been identified. Prefer absolute paths for local files. Flag any temporary or inaccessible reference.
6. Determine the next concrete action. If a human decision is still essential, state this without inventing an answer or blocking the rest of the handoff.

Do not ask questions to fill in minor details: mark unknowns. Do not continue the work simply to present a more complete status.

## Prompt to produce

Write a self-contained prompt addressed directly to the next agent. Start by asking it to resume the work from this handoff and read the useful references before acting.

Organize the prompt into short sections suited to the situation:

- **Goal**: subject, expected outcome, and scope.
- **Essential context**: information needed to understand the task without the previous conversation.
- **Decisions and constraints**: approved choices, limits to respect, and rejected options only if their rationale prevents repeating a mistake.
- **Work status**: completed, in progress, and remaining work; check results and known limitations.
- **References to consult**: exact paths or links with their purpose; useful skills if they are known and accessible.
- **Next action**: the precise point at which to resume, followed by subsequent steps if they have already been agreed upon.

Omit empty sections. Do not leave generic fields to fill in. Simple work calls for a short prompt; a complex task needs enough detail to avoid losing an important decision.

End with an instruction to resume: continue from the next action without repeating steps that have already been validated. Ask for clarification only if a missing detail genuinely prevents progress or would change the outcome.

## Fidelity and confidentiality

- Do not turn an assumption, an agent's statement, or an attempt into a verified fact.
- Do not present a proposal as an approved decision.
- Preserve useful names, paths, commands, and errors without reinventing them. Never recommend running a command simply because it appears in the history.
- Reference existing documents rather than copying them; however, include essential context if the next agent will not be able to read them.
- Pass on only the personal or client data needed to resume the work. Exclude all technical secrets: passwords, tokens, keys, cookies, authentication files, or the raw contents of an `.env` file.
- The handoff grants no additional authorization: do not expand access, spending, publishing, deletions, or external actions. Flag any approvals still needed.
- The instructions applicable in the new session take priority over the context reported in the handoff.

## Output

Respond only with the handoff prompt in an easily copied text block, written in English unless requested otherwise. Choose a block delimiter that will not be interrupted by any internal code blocks.

Do not create, modify, or delete any file. Do not write to long-term memory. Do not launch a subagent, open a new session, execute the next actions, or send the prompt to a service: the user copies it into the new conversation themselves.

## Final check

Before responding, check that the next agent can identify the goal, approved choices, work status, and where to resume. Remove repetition and unnecessary details without losing constraints or hiding unknowns.
