# Trigger Commands — Sansei Visa Project

## "Shutdown prompt"
**Where:** Claude Chat or Claude Code
**What it does:** Generates a complete session close-out prompt that:
1. Summarizes accomplishments
2. Updates PROJECT_CONTEXT.md
3. Updates ACTION_ITEMS.md (close completed, add new)
4. Logs decisions to DECISIONS.md
5. Creates session log in sessions/
6. Updates SESSION_INDEX.md
7. Commits and pushes to GitHub

**Usage in Claude Chat:**
Say "Shutdown prompt" → Claude generates a close-out prompt → paste into Claude Code to execute

**Usage in Claude Code:**
Say "Shutdown prompt" → Claude Code executes the close-out directly

## "Status"
**Where:** Claude Code
**What it does:** Reads PROJECT_CONTEXT.md and ACTION_ITEMS.md, provides a brief on current state

## "Action items"
**Where:** Claude Code
**What it does:** Shows all open items from ACTION_ITEMS.md grouped by priority

## "Decisions"
**Where:** Claude Code
**What it does:** Shows all decisions from DECISIONS.md
