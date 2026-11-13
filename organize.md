# Organize your folders to work with an agent

Copy the block below into a conversation with the agent. The goal is to design an organization that suits you, then put it in place only after you approve it.

## Prompt to copy

````markdown
Help me organize my folders so I can easily find my documents and an agent can work with them properly.

I may not be technical. I want an organization that fits my life and how I use my files, not an imposed template or a large-scale automatic move of all my files.

## How to guide me

- Work step by step, with one question at a time. Explain what you propose in simple words, recommend an option, and wait for my answer.
- Let me choose what matters to me: my activities, my habits, the folders to keep, private areas, and how I want to find my files. Handle the technical details.
- Preserve what already works. If information is available in the rules or our conversations, do not ask me for it again.
- Permission to read does not mean permission to move, rename, or delete. Before each batch of changes, show the paths involved, the consequences, and how to roll back, then wait for my approval.
- Do not create a folder structure before understanding how I use my files. Do not automatically carry out every step after a single approval.

## 1. Understand how I use my computer

Start by asking me what my main activities are and what I currently struggle to find.

Gradually explore the relevant topics without giving me an endless questionnaire:

- My professional, personal, community, or creative activities, or my studies.
- The subjects I deal with day to day: clients, projects, courses, administrative paperwork, housing, hobbies, or others based on my answers.
- How I search: by person, subject, project, date, or document type.
- The files I create, receive, consult often, and keep only for reference.
- Where they arrive and live: Documents, Desktop, Downloads, an external drive, synced or shared folders.
- The software that uses these files and the people I share them with.
- What I want to delegate to the agent: finding, reading, preparing, creating, or editing; and what must remain out of scope.

Do not assume I have clients, software products, or code. Ask only for information relevant to my situation. Summarize what you have understood and have me confirm the priorities before proposing a filing system.

## 2. Examine the authorized folders

Ask which locations you may examine and which are excluded. Start with folder names and a limited depth. Read existing filing guides and instructions. Open documents only if their content is necessary to understand where they belong, within the approved scope.

Distinguish paths that actually exist from references found in an old index. Check references before relying on them. Do not infer that a project is active, finished, or useless from its name or modification date.

Present a brief assessment:

- What is already clear and can stay in place.
- What is scattered or hard to find.
- Incoming areas where files accumulate without a destination.
- Ambiguous filing decisions that need confirmation.
- Folders whose relocation could break a link, software, syncing, or sharing.

Do not scan the entire drive by default. Ignore caches, dependencies, and system files that do not help you understand the organization. Do not browse folders containing secrets or authentication data. File names can themselves be sensitive: do not produce an exhaustive inventory intended for sharing.

Explain that using documents with a remote model may transmit their content to its provider. Local storage alone does not guarantee local processing.

## 3. Choose an entry point and a simple organization

Suggest a main folder from which we can find our way around, such as Documents if that fits my habits. An entry point does not require moving all files to the same place: some folders can stay on their drive, in their shared location, or where software expects them to be.

Then suggest a compact folder structure based on my answers. Explain each folder's role and have me approve the location, names, and groupings. Use language and terms I understand. Numeric prefixes are a sorting option, not a requirement.

Use these principles:

- **Group by subject of work.** Everything related to the same project, client, course, or other subject being followed stays together: documents, notes, deliverables, and related files. Do not systematically separate files into large “PDF,” “Word,” or “Images” collections if that scatters the same work across folders.
- **Separate things with different roles.** Ongoing activities, reusable references, and archives are not handled in the same way. A recurring activity can have its own folder without artificially becoming a project.
- **Include an incoming area if it is useful.** It holds items awaiting filing, not final deliverables. Explain how and when to review it with me, without setting up automatic cleanup.
- **Keep a clear working reference.** Avoid competing copies of the same document. Historical versions, signed originals, backup copies, and exports for distribution can serve legitimate purposes; do not confuse them with duplicates to delete.
- **Keep the structure shallow.** Create a subfolder only if it genuinely helps find or separate work. No empty branches to cover every imaginable use.
- **Allow for exceptions.** Photos, media libraries, code repositories, or folders managed by software may need their own organization. If there is code, a project's code stays with that project when its constraints allow it; tools used across projects can stay separate.

Example of possible roles, to adapt rather than reproduce automatically:

```text
Main folder/
├── To file/
├── Professional activities/
├── Personal/
├── Resources/
└── Archives/
```

Someone may need fewer categories, or different ones. Do not replace their habits with the names in this example without discussing it.

Also define the role of Desktop and Downloads: workspaces, incoming areas, or locations to leave as they are. Do not move these system folders or change their settings without an explicit request.

## 4. Give the agent guidance

Once the filing system has been chosen, suggest lightweight documentation, reusing files that are already there:

1. **A `README.md` at the entry point**, explaining the main folders, their roles, destinations for new documents, exceptions, and areas excluded from reading or writing.
2. **An `AGENTS.md` for filing**, specifying how the agent should use this space. Check the official documentation to see how the current agent loads these instructions. If a connection to its global instructions is needed, explain it and ask for my approval before configuring it. Do not claim a file will be read automatically without checking.
3. **An `INDEX.md` only if the volume warrants it**, with links to the main folders and entry documents. Do not create an exhaustive catalog of every file. Uncertain information must remain explicitly marked as needing confirmation.
4. **Local guides only where the rules differ**, for example in an important activity or a shared folder. Avoid copying the global guide everywhere.

The README explains the filing system; the index helps with navigation; the instructions say how to act. The rules must not contradict one another or become three copies of the same document.

In particular, present these working rules to me, then adapt them to my choices:

- Read the entry-point guide and relevant local rules before creating or filing a file.
- First look for the existing folder matching the subject. A conversation opened at the root does not authorize placing your own deliverables there.
- Do not invent a new major category without approval. If the destination is uncertain, ask me or use the incoming area when it has been explicitly designated for that purpose.
- Keep useful deliverables in their permanent folder. Reserve temporary spaces for working files; do not leave the only copy of an important result in a temporary folder that could disappear.
- Keep names stable and understandable. Use dates or versions when they genuinely help, without renaming old files just to make their appearance uniform.
- Update the affected links and guides after an approved filing change. Check that they still describe reality rather than inferring the filing system from the index alone.
- Respect reading and writing limits, even if the tool technically allows you to go further. An instruction to be careful is not a substitute for a technical permission.

Do not record any secrets in these guides. Do not copy the content of private documents into an index. These files describe the filing system; they do not replace a knowledge memory or authorize moving an existing memory.

## 5. Put it in place gradually, after approval

First propose a small, real, useful batch: a folder I know well or a few documents whose destination is clear. It is also possible to start with the new structure and rules, then file the old documents later.

Before each batch:

- Show how the current paths map to the proposed destinations, including any renaming.
- Identify name conflicts, destinations that already exist, and items whose role is still uncertain. Never replace an existing file for convenience.
- Check the constraints: internal links, shortcuts, paths used by applications or scripts, referenced attachments, code repositories, access rights, and shared folders.
- Explain the particular risk of synced locations: a local move or deletion may propagate remotely or affect collaborators. A visible file may only be a preview that has not been downloaded. Do not trigger bulk downloads or changes to sharing without approval.
- Plan an appropriate rollback. If a backup or copy is needed, explain its location, scope, and any cost, then ask for approval. Do not create a full copy of the entire computer.

Wait for my approval of the specific operations and agree with me on who will move the batch:

- **You move it** if the source folders, destinations, and consequences are clear, you have the necessary access, and I authorize you to do so. Apply only the approved batch; if an ambiguity arises, stop the affected move and ask for clarification.
- **I move it myself** if I prefer to or if you cannot act directly. Guide me step by step, with simple instructions suited to my system and interface: which folder to select, where to move it, and what to check. Give one action at a time, then wait for my confirmation before continuing. Do not simultaneously carry out the moves you ask me to make. If a warning, name conflict, or unexpected result appears, help me understand it before any further action; do not ask me to force a replacement.

In both cases, preserve the documents' content and the metadata needed to use them; do not rewrite files to file them. Do not follow a symbolic link or shortcut to another location without checking its destination and the authorization to access it.

After the batch, check the destinations and file integrity using appropriate methods. Check modified links and the access needed. For manual moves, carry out the checks available to you and guide me through the others. Distinguish what you checked directly from what I confirmed. If a dependency cannot be checked, say so instead of claiming everything works. Have me confirm the result before expanding the filing work.

Do not delete suspected duplicates, empty the trash, or automatically clean up old folders. Ambiguous cases stay in place or in an expressly agreed review area.

## 6. Check that the filing system is usable

Using a few existing files that I authorize you to use:

- Show how to find a document from the entry point by following the guides and links.
- Explain where to file a new document of the same kind, without creating a demonstration file.
- Check that the proposed path matches how I use my files, not just a technical rationale.
- Check that the agent finds the filing instructions and distinguishes permanent, temporary, shared, and excluded folders.
- Check that indexes point to real paths and that items left for confirmation remain visible.

If something requires too much explanation or too many subfolders, propose a simplification and wait for my approval before making it.

Finish with a brief summary: the organization chosen, navigation files created or adapted, batches actually moved, areas left untouched, checks performed, and pending points. Suggest a simple habit for filing future documents, without scheduling a task or automating deletion.

Start with a single question about my main activities and what I want to find more easily. Do not modify any files before our initial choices and my approvals.
````
