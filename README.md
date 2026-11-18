# ai-collab

A demo of how several people (and their AI agents) can pursue related but distinct
research goals in one repository.

## Headline results

Keep only top-level findings here, each linking to the supporting synthesis file.

| Result | Owner | Detail |
| ------ | ----- | ------ |
| _(none yet)_ | | |

## Layout

```
README.md            headline results (this file)
knowledge/           shared knowledge base (see knowledge/README.md)
  synthesis/         human-readable summaries; read these first
  ai-notes/          AI intermediate notes and handoff context; NOT read by default
  raw-sources/       original PDFs, audio, etc.
users/<name>/        each person's working folder
  README.md          that person's headline results (sub-project "TLDR")
  inbox/             messages from other users and their agents
users/_template/     copy this to add a new user
AGENTS.md            conventions for AI agents
```

## Conventions

- **Headline results** live in this README and in each `users/<name>/README.md`.
- **Synthesis** files in `knowledge/synthesis/` summarise and link to the detailed
  notes in `knowledge/ai-notes/` that back them up.
- **Raw sources** go in `knowledge/raw-sources/`; each must be converted to markdown
  in `knowledge/ai-notes/` (same base name, e.g. `paper.pdf` -> `paper.md`).
- **Do most work in your own folder** `users/<name>/`.
- **Messaging**: to contact another user, add a file to `users/<them>/inbox/` named
  `YYYY-MM-DD-<from>-<subject>.md`. Read your own inbox at the start of a session.

See `AGENTS.md` for agent-specific instructions.
