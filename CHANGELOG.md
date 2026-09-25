# Changelog

## 2026-09-25 - Per-Model Effort Settings
- Moved effort configuration to per-model settings and dropped the pinned model
- Dropped ultracode so startup uses per-model effort
- Ignored synced skills and state directories

## 2026-05-31 ~ 2026-07-16 - Model, Plugin, and TUI Settings Changes
- Switched the default model several times (claude-fable-5, opus[1m], sonnet, claude-fable-5[1m])
- Toggled ultracode on and off across model switches
- Bumped effort to xhigh; moved the TUI from default to fullscreen
- Added academic-research-skills plugin and claude-plugins-official plugin source
- Enabled push notifications and the clangd-lsp plugin
- Removed the disabled superpowers plugin and reordered config keys

## 2026-05-12 ~ 2026-05-29 - Attention Hooks, Keybindings, and README Rewrite
- Added claude-attn.sh hook for Notification and Stop events, surfacing the last assistant message in stop notifications
- claude-attn now fires notify-send for background sessions; removed its UserPromptSubmit handler and tmux logic
- Replaced the commit-push command with a commit-message generator
- Added custom keybindings.json with transcript scroll bindings
- Rewrote README.md to match the current configuration
- Enabled verbose output by default
- Ignored image-cache directory and .last-update-result.json

## 2026-04-05 ~ 2026-05-11 - Settings and MCP Cleanup
- Added, then removed, an API proxy environment configuration
- Added theme, editor, and compact settings; switched editor to normal mode
- Added auto permission and defaultMode configuration
- Removed .mcp.json server configuration
- Deleted the agents-back/ backups and old find-paper, search-papers, weekly-report, and wpaper commands
- Briefly enabled, then disabled, the superpowers plugin

## 2025-11-17 ~ 2026-02-26 - Agent Removal and Settings Housekeeping
- Added, then removed, a Neovim sync hook for file changes
- Removed all agent files (moved to agents-back/ as a backup) and disabled the auto-updater
- Added docs/invalid-ip-address.md documenting the invalid IP address issue
- Cleaned up and reformatted settings.json
- Ignored cache and backups directories in .gitignore

## 2025-09-15 ~ 2025-10-22 - Commit-Push Command and Gitignore Updates
- Removed academic-writing.md agent pending a rewrite
- Added commit-push slash command, then simplified its format and improved scope guidance
- Stopped tracking sensitive info, history log, and update.lock via .gitignore
- Reformatted Claude Code settings

## 2025-09-08 - Add Specialized Academic Agents and Remove Deprecated Commands
- Added academic-search.md agent for comprehensive multi-platform paper discovery across IACR, Google Scholar, Crossref, and CryptoBib
- Added academic-writing.md agent for transforming content to meet rigorous academic publication standards
- Added paper-research.md agent for systematic literature review with quality verification
- Added weekly-report-writing.md agent for professional progress documentation with academic language
- Removed deprecated commit-push.md and crypto-research.md commands from commands/ directory
- Restructured agents/ directory to focus on specialized academic and writing tasks

## 2025-08-13 - Add Specialized Agent Documentation
- Added blog-writing.md agent for enhancing and completing blog content with improved readability and formatting
- Added commit-push.md agent for standardized git commit message generation and changelog management
- Both agents include comprehensive descriptions, tool configurations, and usage guidelines

## 2025-08-13 - MCP Server Configuration and Command Documentation
- Added MCP server configuration for enhanced Claude Code functionality
- Added commit and push command documentation
- Improved permissions structure and configuration formatting
- Added weekly report writing assistant and academic paper research assistant documentation