# CLAUDE.md - AI Assistant Guide

## Repository Overview

**Repository Type**: GitHub Profile README
**Owner**: ryu (ryugen-io)
**Purpose**: Personal profile showcasing AI/MCP technology stack and projects
**Primary File**: `README.md`

This is a documentation-only repository containing a GitHub profile README. It has no source code, dependencies, or build systems.

---

## Repository Structure

```
ryugen-io/
├── README.md              # GitHub profile README (main content)
├── CLAUDE.md             # This file - AI assistant guide
└── .git/                 # Git repository metadata
```

### Current State
- **Total Files**: 2 (README.md, CLAUDE.md)
- **Languages**: None (documentation only)
- **Dependencies**: None
- **Build System**: None
- **CI/CD**: None

---

## Content Guidelines

### README.md Conventions

The README.md serves as a GitHub profile page and follows these conventions:

1. **Tone & Style**
   - Personal and casual
   - Direct and concise
   - Tech-focused without excessive marketing language
   - **No emojis** (removed in commit bd21aaa)

2. **Structure**
   - Opening greeting with author name
   - Brief mission statement
   - Technology stack with badge links
   - Current focus/projects
   - Contact information

3. **Badge Format**
   - Uses shields.io badges
   - Format: `[![Label](badge-url)](link-url)`
   - Includes logo and color customization
   - Current badges:
     - Anthropic Claude (purple: #6C47FF)
     - MCP Protocol (orange)
     - Rust (orange with logo)

4. **Technology Stack Display**
   - Lists current working technologies
   - Links to official project pages
   - Highlights specific tools (e.g., "Serena MCP")
   - Includes version years for languages (e.g., "Rust 2024")

### Content Preferences

Based on commit history:
- **Avoid**: Excessive emojis (see commit bd21aaa: "Remove emojis from profile")
- **Prefer**: Clean, text-based formatting with shields.io badges
- **Focus**: AI development, MCP protocol, Rust, automation
- **Style**: Straightforward descriptions over hype

---

## Development Workflow

### Git Branch Strategy

- **Main Branch**: `main` (not specified in git config, likely default)
- **Feature Branches**: Use `claude/` prefix for AI assistant work
  - Format: `claude/claude-md-<session-id>`
  - Example: `claude/claude-md-mi0pusm9opq9vai9-019otrda3WNHiQrWWtS66Tpg`

### Commit Message Conventions

Based on existing commit history:

```
Pattern: <Action> <subject> [with <detail>]

Examples:
✓ "Update README with MCP and AI buddy details"
✓ "Remove emojis from profile"
✓ "Add profile README with AI/MCP stack"

Guidelines:
- Use imperative mood ("Add", "Update", "Remove")
- Be specific about what changed
- Include "why" context when helpful
- Keep under 72 characters when possible
```

### Making Changes

1. **Before Editing**
   - Read README.md to understand current state
   - Check git log for recent changes and patterns
   - Verify current branch with `git status`

2. **When Editing README.md**
   - Maintain existing structure
   - Follow badge format conventions
   - Keep tone consistent (personal, tech-focused)
   - No emojis unless explicitly requested
   - Ensure all links are valid and relevant

3. **Committing**
   ```bash
   git add <files>
   git commit -m "Clear, descriptive message"
   git push -u origin <branch-name>
   ```

4. **Push Requirements**
   - Use `git push -u origin <branch-name>`
   - Branch must start with `claude/` for AI assistant work
   - Retry up to 4 times with exponential backoff if network issues

---

## Common Tasks for AI Assistants

### Task 1: Update Technology Stack

When updating the "Currently working with" section:

1. Maintain badge format:
   ```markdown
   [![Label](https://img.shields.io/badge/Text-Value-Color?logo=logoname&logoColor=white)](https://link-url)
   ```

2. Keep badges grouped logically
3. Update description text to match
4. Verify all URLs are accessible

### Task 2: Add New Projects/Links

When adding new project mentions:

1. Link to official project pages
2. Use **bold** for emphasis on key tools
3. Keep descriptions brief (one line preferred)
4. Maintain consistent formatting with existing entries

### Task 3: Content Refresh

When refreshing outdated content:

1. Check if technology versions need updating (e.g., "Rust 2024" → "Rust 2025")
2. Verify all external links still work
3. Remove deprecated tools or outdated references
4. Update badge colors if branding has changed

### Task 4: Formatting Fixes

When fixing formatting issues:

1. Ensure consistent spacing (blank lines between sections)
2. Check badge syntax is correct
3. Verify Markdown rendering (headings, links, lists)
4. Remove any accidental emoji additions

---

## Technology Context

### Current Stack (as of Nov 2025)

- **AI Platform**: Claude (Anthropic) - Opus model
- **Protocol**: MCP (Model Context Protocol)
- **Language**: Rust (2024 edition)
- **MCP Server**: Serena MCP (https://github.com/cristianvogel/serena)

### Key External Resources

- [Anthropic Claude](https://www.anthropic.com/claude)
- [Model Context Protocol](https://modelcontextprotocol.io)
- [Rust Language](https://www.rust-lang.org/)
- [Serena MCP Server](https://github.com/cristianvogel/serena)

---

## File-Specific Notes

### README.md

- **Line Count**: ~20 lines
- **Last Updated**: Nov 10, 2025 (commit f09d204)
- **Encoding**: UTF-8
- **Line Endings**: LF (Unix-style)
- **Max Line Length**: ~120 characters (badge lines)

**Recent Changes**:
- f09d204: Added Serena MCP and Claude Opus details
- bd21aaa: Removed emojis for cleaner appearance
- 5533901: Initial creation with AI/MCP stack info

---

## Git Configuration

### Remote Repository

```
URL: http://local_proxy@127.0.0.1:19447/git/ryugen-io/ryugen-io
```

### Git Settings

- File mode tracking: Enabled
- Ref update logging: Enabled
- Repository format version: 0

---

## AI Assistant Best Practices

### DO:
- ✓ Read README.md before making any changes
- ✓ Follow existing commit message patterns
- ✓ Maintain the current tone and style
- ✓ Use shields.io badges for technology references
- ✓ Keep content concise and focused
- ✓ Verify links before adding them
- ✓ Use `claude/` branch prefix for development
- ✓ Push with `-u origin <branch-name>`

### DON'T:
- ✗ Add emojis (they were intentionally removed)
- ✗ Make content overly promotional or marketing-heavy
- ✗ Add unnecessary files or directories
- ✗ Create build systems or dependencies (this is profile-only)
- ✗ Push to main without explicit permission
- ✗ Ignore existing formatting conventions
- ✗ Add large sections that break the concise nature

### When in Doubt:
1. Review git history: `git log --oneline`
2. Check existing content patterns in README.md
3. Ask the user for clarification
4. Maintain existing style over introducing new patterns

---

## Troubleshooting

### Issue: Git push fails with 403
**Solution**: Ensure branch name starts with `claude/` and matches session ID format

### Issue: Badge not rendering
**Solution**: Check URL encoding, verify shields.io syntax, test badge URL in browser

### Issue: Unclear what to update
**Solution**: Ask user for specific requirements, review recent commits for context

---

## Version History

| Date | Version | Changes |
|------|---------|---------|
| 2025-11-15 | 1.0 | Initial CLAUDE.md creation with comprehensive guidelines |

---

## Additional Notes

This repository is intentionally minimal. Its sole purpose is to serve as a GitHub profile README. There are no plans for:
- Source code additions
- Build systems or CI/CD
- Dependencies or package management
- Complex directory structures
- Automated testing

Any changes should focus on keeping the README.md accurate, current, and aligned with the owner's (ryu's) technology focus and personal brand.

---

**Last Updated**: 2025-11-15
**Last Reviewed By**: AI Assistant (Claude)
**Next Review**: As needed when significant profile updates occur
