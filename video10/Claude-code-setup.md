# Claude Code CLI Setup Guide

## What is Claude Code?

Claude Code is Anthropic's official CLI tool that brings Claude's AI capabilities directly to your terminal. It can understand your entire codebase, make complex changes across multiple files, run commands, and help with everything from debugging to deployment.

## Prerequisites

- macOS, Linux, or Windows (with WSL)
- Node.js 18 or newer
- A Claude.ai account (either Claude Code Max subscription or Anthropic API key)

## Installation

### Quick Start (How I Use It)
```bash
# Install Claude Code globally
npm install -g @anthropic-ai/claude-code

# Navigate to your project
cd /path/to/your/project

# Start Claude Code
claude
```

That's it! With Claude Code Max subscription, you don't need to configure API keys.

## Configuration

### Option 1: Claude Code Subscription (How I Use It)
If you have a **Claude Code or Claude Code Max subscription** like I do:
- No API key configuration needed
- Just install and run `claude` in your project
- Claude will open browser to authenticate on first use
- Includes usage within the Claude subscription

### Option 2: Using API Key
If you're using an Anthropic API key:
```bash
# Set via environment variable
export ANTHROPIC_API_KEY="your-api-key-here"
```

## IDE Integration (How I Use It)

### VS Code Integration (Auto-Installation!)
Claude Code works seamlessly with VS Code and popular forks (Cursor, Windsurf, VSCodium).

**Installation - It's Automatic!**
1. Open VS Code in your project
2. Open the integrated terminal (Terminal → New Terminal)
3. Run `claude` - the extension auto-installs! 🎉

## Basic Usage

### How I Start My Day with Claude Code:
```bash
# Open VS Code in my project
code /path/to/sucana

# In terminal, start Claude Code
claude --resume (to resume previously running session)

# Claude remembers context from previous sessions!
```

### My Typical Workflow

1. **Describe what I want in plain English:**
   ```
   "I want to allow users to edit campaign names inline from the campaigns list"
   ```

2. **Claude Code automatically:**
   - Reads relevant files
   - Creates/modifies multiple files
   - Runs tests if needed
   - Shows me exactly what changed

3. **I review in VS Code:**
   - See all changes in the diff viewer
   - Test the feature
   - Ask for adjustments if needed

### Key Commands I Use Daily

- **Feature Development:** "Add [feature] with proper error handling and tests." "I want to implement AWS S3 in my application to store audio and video file generated during ads creation flow."
- **Bug Fixing:** "This error is happening: [paste error]. Fix it"
- **Code Review:** "Review this code and suggest improvements"
- **Documentation:** "Update the README with these new endpoints." "create a step-by-step guide of how we configured and deployed our code on AWS."
- **Deployment:** "Guide me through deploying backend to production. I want to deploy frontend on Vercel and backend to AWS Lightsail servers."

## Powerful Features I Use

## Powerful Features I Use

### 1. Plan Mode (For Big Features) 🎯
**How I activate it:** Press `Shift+Tab` twice
**When I use it:** For new features and architectural decisions

**Example: AWS S3 Implementation**
```
Me: [Shift+Tab twice to enter plan mode]
"I want to implement AWS S3 in my application to store audio and 
video files generated during ads creation flow. What do you think 
about it and what's the best way to implement?"

Claude: [Provides detailed architecture plan, discusses pros/cons, 
suggests implementation steps]

Me: "Let's also consider CDN integration and signed URLs for security"

Claude: [Refines plan with security considerations]

Me: [Exit plan mode and Claude implements the agreed plan]
```

**Example: Facebook Marketing API Integration**
```
Me: [In plan mode]
"I want to pull FB marketing data. Here's what I'm thinking..."

Claude: [Discusses OAuth flow, data models, rate limiting, 
suggests best practices]
```

**Benefits of Plan Mode:**
- Have thoughtful discussions before coding
- Explore different approaches
- Consider edge cases and security
- Get architecture recommendations
- Claude then implements exactly what we planned

### 2. Multi-File Operations
**What I say:** "Update all React components to use the new design system." "implement a comprehensive database log for the audio generation flow."
**Claude does:** Identifies all components, updates imports, applies consistent styling

### 3. Smart Context Understanding  
Claude remembers our entire conversation. I can say:
- "Do the same for the Scripts page"
- "Like we did yesterday"
- "Fix that error from before"

### 4. Automatic Tool Selection
Claude automatically chooses the right approach:
- Uses `grep` for searching
- Uses `git` for version control
- Runs `npm test` when needed
- Checks file existence before editing

### 5. Real-Time Collaboration
With VS Code integration, I see:
- Files being edited live
- Terminal commands running
- Git changes accumulating
- All while I can test in another terminal

### 6. Intelligent Task Management
Claude tracks complex multi-step tasks:
- Creates todo lists automatically
- Marks items complete as it works
- Ensures nothing is forgotten

### 7. Production-Ready Code
Claude writes code that's:
- Properly typed (TypeScript)
- Has error handling
- Follows existing patterns in my codebase
- Includes helpful comments when needed

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

## Real-World Examples (From My Session Today)

### Example 1: Performance Optimization
**What I said:**
```
"Could you please optimize the campaign list page as it is very slow"
```
**What Claude Code did:**
- Analyzed database queries across multiple files
- Implemented batch fetching to reduce N+1 queries
- Reduced API calls from 50+ to just 2
- Result: 80-90% reduction in data transferred

### Example 2: UI Enhancement  
**What I said:**
```
"On the hook page, I would like to highlight angles just like how we show them 
on script page. Also make them expand and collapse when user click on them"
```
**What Claude Code did:**
- Read both HooksV2.tsx and Scripts.tsx to understand the design
- Added Material-UI Collapse and IconButton imports
- Implemented gradient backgrounds matching Scripts page
- Added expand/collapse state management with animations
- Sorted angles by number and expanded first by default

### Example 3: Complex Bug Fix
**What I said:**
```
"I completed the flow and it shows 100% but in progress. 
Also video is shown as unchecked"
```
**What Claude Code did:**
- Traced through the video generation endpoint
- Found status wasn't being updated to "completed"
- Updated both backend (Python) and frontend (React) logic
- Fixed the visual indicator in CampaignsList.tsx

### Example 4: Deployment Assistance
**What I said:**
```
"Backend is not deployed. What do I do to deploy. 
I can connect to AWS Lightsail using their browser"
```
**What Claude Code did:**
- Guided through SSH connection
- Discovered Docker setup (not Python venv)
- Provided exact Docker commands for deployment
- Updated project documentation with deployment steps

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