# Sansei Visa Project

## Project Summary
Strategic advisory project to help Ryan Masato Sumida obtain, activate, and legally maintain a Japanese Long-Term Resident Visa based on 3rd-generation (Sansei) descent — while remaining a full-time resident of Texas.

**Repo:** `rmsumida/sansei-visa-project`
**Owner:** Ryan Masato Sumida (@rmsumida)
**Created:** 2026-03-26
**Deadline:** 2027-03-26 (1-year duration)

## Auto-Briefing
On first interaction in any session, Claude Code MUST:
1. Read `governance/PROJECT_CONTEXT.md` for current project state
2. Read `governance/ACTION_ITEMS.md` for open tasks
3. Read `governance/SESSION_INDEX.md` for the last session number
4. Brief the user with:
   - Current session number (last session + 1)
   - Days remaining until deadline
   - Count of open action items by priority
   - Recommended focus for this session

## Repo Structure
```
sansei-visa-project/
├── CLAUDE.md                          ← You are here
├── README.md
├── governance/
│   ├── PROJECT_CONTEXT.md             ← Single source of truth
│   ├── ACTION_ITEMS.md                ← Task tracker
│   ├── SESSION_INDEX.md               ← Session log index
│   ├── DECISIONS.md                   ← Decision register
│   ├── TRIGGER_COMMANDS.md            ← Trigger command specs
│   └── PROJECT_INSTRUCTIONS.md        ← Claude Chat project instructions
├── budget/.gitkeep
├── documents/                         ← Visa documents, forms, evidence
├── sessions/session-NNN.md            ← Individual session logs
└── photos/.gitkeep
```

## Session Shutdown Trigger
When the user says **"Shutdown prompt"**, Claude Code MUST:
1. Summarize what was accomplished this session
2. Update `governance/PROJECT_CONTEXT.md` with any new state
3. Update `governance/ACTION_ITEMS.md` — check off completed items, add new ones
4. Update `governance/DECISIONS.md` with any decisions made
5. Create `sessions/session-NNN.md` with the session log
6. Update `governance/SESSION_INDEX.md` with the new session entry
7. Stage, commit, and push all changes:
   ```
   git add . && git commit -m "Session NNN: <summary>" && git push
   ```

## Between-Session Commands
- **"Status"** — Read PROJECT_CONTEXT.md and ACTION_ITEMS.md, brief on current state
- **"Action items"** — Show all open items from ACTION_ITEMS.md grouped by priority
- **"Decisions"** — Show all decisions from DECISIONS.md
- **"Session log"** — Show SESSION_INDEX.md

## Project Rules
- All advice must account for maintaining full-time Texas residency
- Duration to complete project is 1 year (deadline: 2027-03-26)
- Visa category: Long-Term Resident Visa (Sansei / 3rd-generation Japanese descent)
- All legal guidance is informational — not legal advice; consult an immigration attorney for binding decisions
- Track all deadlines and expiration dates explicitly in action items
