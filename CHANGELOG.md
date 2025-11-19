# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

### 2025-11-19 - Sync with upstream glittercowboy/taches-cc-resources

#### Added
- Claude Code plugin structure with marketplace support
  - `.claude-plugin/plugin.json` - Plugin configuration
  - `.claude-plugin/marketplace.json` - Marketplace metadata
- New auditor subagents for quality assurance:
  - `agents/skill-auditor.md` - Expert skill auditor for best practices compliance
  - `agents/slash-command-auditor.md` - Expert slash command auditor
  - `agents/subagent-auditor.md` - Expert subagent configuration auditor
- New audit commands:
  - `/audit-skill` - Audit skill for best practices
  - `/audit-slash-command` - Audit command for best practices
  - `/audit-subagent` - Audit subagent for best practices
- New creation commands:
  - `/create-agent-skill` - Create a new skill
  - `/create-meta-prompt` - Create staged workflow prompts
  - `/create-slash-command` - Create a new slash command
  - `/create-subagent` - Create a new subagent
  - `/create-hook` - Create a new hook
- Self-improvement command:
  - `/heal-skill` - Fix skills based on execution issues
- Comprehensive skills with detailed reference documentation:
  - `skills/create-agent-skills/` - Build skills by describing what you want
  - `skills/create-meta-prompts/` - Build prompts with structured outputs
  - `skills/create-slash-commands/` - Build commands that expand into full prompts
  - `skills/create-subagents/` - Build specialized Claude instances
  - `skills/create-hooks/` - Build event-driven automation

#### Changed
- Reorganized repository structure for better clarity:
  - Moved all slash commands to `commands/` directory
  - Consolidated documentation into `docs/` directory
  - Created dedicated `skills/` directory with comprehensive references
  - Created `agents/` directory for auditor subagents
- File relocations:
  - `meta-prompting/create-prompt.md` → `commands/create-prompt.md`
  - `meta-prompting/run-prompt.md` → `commands/run-prompt.md`
  - `context-handoff/whats-next.md` → `commands/whats-next.md`
  - `todo-management/add-to-todos.md` → `commands/add-to-todos.md`
  - `todo-management/check-todos.md` → `commands/check-todos.md`
  - `context-handoff/README.md` → `docs/context-handoff.md`
  - `meta-prompting/README.md` → `docs/meta-prompting.md`
  - `todo-management/README.md` → `docs/todo-management.md`
- Updated README with:
  - Plugin installation instructions (now recommended method)
  - Reorganized command categories
  - Links to new agents and skills
  - Context summaries for each section

#### Improved
- Simplified skill-routing slash commands
- Enhanced documentation clarity across all sections
- Better organization of reference materials for each skill

#### Technical Details
- Merged 20 commits from upstream repository
- Resolved file reorganization conflicts
- Added remote: `glittercowboy` → https://github.com/glittercowboy/taches-cc-resources.git

---

## Initial Release

### Added
- Meta-prompting system
- Todo management commands
- Context handoff functionality
