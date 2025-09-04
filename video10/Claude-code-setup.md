# Claude Code CLI Setup Guide

## What is Claude Code?

Claude Code is Anthropic's official CLI tool that brings Claude's AI capabilities directly to your terminal. It can understand your entire codebase, make complex changes across multiple files, run commands, and help with everything from debugging to deployment.

## Prerequisites

- macOS, Linux, or Windows (with WSL)
- Node.js 18+ or Python 3.8+
- An Anthropic API key (get one at [console.anthropic.com](https://console.anthropic.com))

## Installation

### Option 1: Using npm (Recommended)
```bash
npm install -g @anthropic/claude-cli
```

### Option 2: Using pip
```bash
pip install claude-cli
```

### Option 3: Using Homebrew (macOS)
```bash
brew tap anthropic/tap
brew install claude-code
```

## Configuration

1. **Set up your API key:**
```bash
claude-code configure
# Enter your Anthropic API key when prompted
```

2. **Or set via environment variable:**
```bash
export ANTHROPIC_API_KEY="your-api-key-here"
```

## Basic Usage

### Start Claude Code in your project directory:
```bash
cd /path/to/your/project
claude-code
```

### Key Commands

- **Read files:** Claude automatically reads files you reference
- **Edit files:** Claude can modify multiple files simultaneously  
- **Run commands:** Claude can execute terminal commands
- **Search code:** Claude can search across your entire codebase
- **Git operations:** Claude can commit changes with proper messages

## Powerful Features

### 1. Multi-File Operations
```
"Update all React components to use the new design system"
```
Claude will identify and update all relevant files.

### 2. Complex Refactoring
```
"Optimize the database queries in the campaigns page"
```
Claude can analyze and improve performance across your stack.

### 3. Feature Development
```
"Add inline editing for campaign names with proper error handling"
```
Claude builds complete features with frontend, backend, and database changes.

### 4. Debugging & Fixes
```
"Fix the CORS error for PATCH requests in production"
```
Claude diagnoses issues and implements solutions.

### 5. Deployment Assistance
```
"Help me deploy this to AWS Lightsail with Docker"
```
Claude provides step-by-step deployment guidance.

## Project Setup Tips

### 1. Create a CLAUDE.md file
Add a `CLAUDE.md` file to your project root with:
- Project architecture overview
- Key file locations
- Development commands
- Deployment instructions
- Coding conventions

Example:
```markdown
# CLAUDE.md

## Project Structure
- frontend/ - React app
- backend/ - FastAPI server  
- database/ - PostgreSQL schemas

## Key Commands
- npm run dev - Start development
- npm test - Run tests
- docker-compose up - Start services

## Deployment
- Frontend: Vercel
- Backend: AWS Lightsail with Docker
```

### 2. Use Descriptive Commit Messages
Claude can generate proper commit messages:
```
"Commit these changes with a descriptive message"
```

### 3. Leverage Context Windows
Claude remembers your conversation, so you can:
- Reference previous changes
- Build features incrementally
- Maintain consistency across sessions

## Best Practices

1. **Be Specific:** "Add error handling to the user authentication flow" > "Fix the login"

2. **Provide Context:** Share relevant URLs, error messages, and requirements

3. **Review Changes:** Always review Claude's suggestions before applying

4. **Test Incrementally:** Run tests after each major change

5. **Use Version Control:** Commit working code before major refactors

## Real-World Examples

### Example 1: Performance Optimization
```
User: "The campaigns page is loading slowly"
Claude: *Analyzes queries, implements batch fetching, reduces load time by 80%*
```

### Example 2: UI Enhancement
```
User: "Make the angles on the Hooks page collapsible with prominent styling"
Claude: *Updates component with Material-UI Collapse, adds gradient backgrounds, implements expand/collapse state management*
```

### Example 3: Bug Fix
```
User: "CORS error when updating campaign names in production"
Claude: *Diagnoses preflight issue, adds OPTIONS middleware, provides deployment steps*
```

## Limitations

- Cannot access external websites directly (use curl/wget)
- Cannot modify system files without permission
- Cannot run GUI applications
- Context window has limits (though very large)

## Getting Help

- Documentation: [claude.ai/docs](https://claude.ai/docs)
- Report issues: [github.com/anthropics/claude-code/issues](https://github.com/anthropics/claude-code/issues)
- Community: [discord.gg/anthropic](https://discord.gg/anthropic)

## Pro Tips

1. **Save Context:** Keep a `CLAUDE.md` file updated with project-specific information
2. **Chain Commands:** Claude can execute multiple related tasks in sequence
3. **Use Todo Lists:** Claude can track multi-step tasks with built-in todo management
4. **Explain Errors:** Paste full error messages for better debugging
5. **Leverage Memory:** Reference earlier work with "like we did before"

---

*Claude Code transforms your terminal into an AI-powered development environment. It's not just a coding assistant—it's like having a senior developer who knows your entire codebase.*