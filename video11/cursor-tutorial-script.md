# Video 8: Cursor Tutorial - The AI Editor That Changed Everything (Complete Beginner Guide)

## Hook (00:00-00:30)

Remember when I told you about my journey from Bolt to V0 to Claude Code? Well, there's one tool I haven't talked about enough - Cursor. And honestly? This is the tool that made me feel like a "real" developer for the first time.

You're tired of copy-pasting from ChatGPT. You're frustrated with browser-based tools that feel like toys. You want to build REAL applications but traditional coding feels overwhelming.

What if I told you there's an AI code editor that bridges that gap perfectly? One that feels professional but holds your hand every step of the way?

## Introduction (00:30-01:00)

Today, I'm showing you Cursor AI - the tool that transformed how I build applications. This isn't just another tutorial. I'm going to show you exactly how I use Cursor to build features for my startup Sucana, and how you can start building real applications TODAY.

By the way, I'm Vinod Sharma. 10 months ago, I couldn't write a single line of code. Now I'm building a full-stack startup. My journey went from ChatGPT copy-paste hell → Bolt & V0 → Cursor → and finally Claude Code CLI. But Cursor? That was the game-changer.

If you're new here, welcome to the Vibe Coding series. Hit subscribe and let's level up together.

Let's dive into the tool that made me believe I could actually code.

## Why Cursor Changed Everything for Me (01:00-02:00)

[SCREEN: Show Cursor opening]

Three months into my AI coding journey, I hit a wall. Bolt and V0 were amazing for prototypes, but I needed something more. I needed to feel in control.

That's when I discovered Cursor. And listen - the first time I opened it, I almost closed it immediately. It looked like VS Code, felt professional, intimidating even.

But then I pressed Cmd+K. And everything changed.

### My Cursor Journey Timeline
- Month 1-2: Fighting with ChatGPT copy-paste
- Month 3: Discovered Cursor
- Month 4: Built my first real application
- Month 5: Started using it for Sucana
- Now: Teaching you everything I learned

## Setting Up Your Workspace (02:00-03:00)

First things first - let's set this up properly. I made so many mistakes initially, let me save you the pain.

[SCREEN: File → Open Folder]

**Critical tip**: Always create a new folder on your desktop first. Don't work in the default directory like I did for weeks - lost so much work!

```
1. Download Cursor (it's free to start)
2. File → Open Folder
3. Create new folder: "my-first-cursor-project"
4. Open it
```

Now you have a clean workspace. This is YOUR development environment.

## The Composer - Your Multi-File Wizard (03:00-05:00)

[SCREEN: Show Preferences → Features → Composer]

This feature wasn't enabled by default when I started. Lost 2 weeks not knowing it existed!

**Enable Composer:**
- File → Preferences → Cursor Settings
- Click Features
- Scroll to Composer
- Enable it

Now press **Cmd+I** (or Ctrl+I on Windows).

### My First Real App with Composer

Watch this - I'll recreate the exact prompt that got me hooked:

```
Create a recipe manager application:
- Use Express.js for backend
- SQLite for storing recipes
- Frontend with HTML, CSS (use Tailwind)
- Include: add recipe, delete recipe, search by ingredient
- Make it look modern and clean
```

[GENERATE AND SHOW FILES BEING CREATED]

Look at this! It's creating:
- `server.js` - complete backend
- `index.html` - full UI
- `styles.css` - Tailwind styling
- `script.js` - all the interactions

This is a REAL application. Not a toy. Not a demo. Real code you can deploy.

## The Chat Window - Your Coding Companion (05:00-07:00)

[SCREEN: Press Cmd+L to open chat]

After the Composer builds your foundation, the chat window becomes your best friend.

**Pro tip from my Sucana development**: The chat knows your ENTIRE codebase. Use this power!

### Adding Context Like a Pro

Press `@` to add context:
- `@server.js` - reference specific files
- `@web` - search documentation
- `@docs` - link external documentation

Example from my actual workflow:

```
@server.js Can you add 5 more unique recipes? 
Make them vegetarian and include cooking time.
```

[SHOW APPLY BUTTON AND DIFF]

See that? It doesn't just give you code - it APPLIES it directly. No copy-paste!

## Inline Editing - The Feature That Hooked Me (07:00-09:00)

This is where I felt like a "real" developer for the first time.

[SCREEN: Show inline completion]

Watch what happens when I type:

```javascript
// Function to validate email
function validate
```

[SHOW AUTOCOMPLETE]

It completes entire functions! But here's the real magic:

**Select any code → Press Cmd+K → Give instructions**

Real example from Sucana:
1. Select a messy function
2. Cmd+K
3. "Refactor this using async/await and add error handling"
4. Accept changes

This is how I refactored my entire Sucana backend in 2 days instead of 2 weeks.

## Image to Code - Mind-Blowing Feature (09:00-10:30)

Nobody talks about this enough, but this is how I prototype UI for Sucana.

[SCREEN: Drag in a design image]

I grabbed a random login form design from Pinterest. Watch this:

1. Open chat (Cmd+L)
2. Drag image
3. "Create an HTML file that looks exactly like this image"

[SHOW GENERATION]

But wait - it tries to apply to existing file. Here's the trick:

1. Create new file: `login.html`
2. Then apply the code
3. Open in browser

[SHOW RESULT]

From image to working code in 30 seconds. I use this for every Sucana feature mockup.

## My Cursor Workflow for Real Development (10:30-12:00)

Let me show you how I actually use Cursor for Sucana:

### Morning Routine
1. Open project
2. Cmd+L: "What did I work on yesterday?" (it remembers!)
3. Cmd+I: Plan today's feature
4. Start building

### The Three-Layer Approach
1. **Composer (Cmd+I)**: Big features, multiple files
2. **Chat (Cmd+L)**: Medium changes, explanations
3. **Inline (Cmd+K)**: Quick fixes, refactoring

### Real Sucana Example
"I need to add user authentication to my recipe app"

1. Composer: Generate auth system
2. Chat: Customize for my needs
3. Inline: Clean up and optimize

This approach built our entire authentication in 4 hours.

## Cursor vs Other Tools - My Honest Take (12:00-13:30)

After 10 months, here's my breakdown:

### When I Use Cursor
- Building features for Sucana
- Learning new frameworks
- Refactoring existing code
- When I need to feel "in control"

### When I Don't Use Cursor
- Quick prototypes (I use Bolt)
- UI components (V0 is better)
- Complex architecture (Claude Code CLI)
- Simple scripts (ChatGPT is fine)

### The Cost Question
- Free tier: Good for learning
- Pro ($20/month): What I used for months
- Cursor upgraded my productivity 10x - best $20 I spent

## Common Mistakes I Made (So You Don't Have To) (13:30-14:30)

1. **Not enabling Composer** - Lost 2 weeks
2. **Not using @ mentions** - Context is everything
3. **Fighting the AI** - Let it help you
4. **Not saving work** - Always git commit
5. **Trying to do everything in Cursor** - Use the right tool

## Your Action Plan (14:30-15:00)

Here's exactly what to do after this video:

**Today:**
1. Download Cursor (free)
2. Enable Composer
3. Build something simple (todo list, calculator)

**This Week:**
1. Recreate one of your ChatGPT projects in Cursor
2. Use all three features (Composer, Chat, Inline)
3. Deploy something real

**This Month:**
1. Build a full application
2. Master the keyboard shortcuts
3. Integrate with your workflow

## Advanced Tips from My Sucana Development (15:00-16:00)

### The Power User Setup
- Split terminal for commands
- Multiple chat windows
- Custom keyboard shortcuts
- Git integration

### My Favorite Prompts
1. "Analyze this code for security issues"
2. "Add comprehensive error handling"
3. "Convert this to TypeScript with proper types"
4. "Optimize this for production"

### The Learning Accelerator
Cursor taught me to code by showing me patterns. Every suggestion is a mini-lesson. Pay attention, learn the patterns, level up faster.

## Closing (16:00-16:30)

That's Cursor - the tool that transformed me from a complete beginner to building a real startup in 10 months.

Remember, I started exactly where you are. ChatGPT copy-paste, feeling lost, thinking "real" coding was impossible. Cursor changed that. It can change it for you too.

You don't need years of experience. You don't need a CS degree. You just need Cursor and the willingness to build.

In the next video, I'm showing you how to combine Cursor with Claude Code CLI - the ultimate power combo I use for Sucana's most complex features.

Drop a comment - what will you build first with Cursor? I personally respond to everyone because we're all on this journey together.

If this helped you level up, hit subscribe. Share this with someone who thinks coding is impossible. Let's prove them wrong together.

Keep shipping, keep learning, and I'll see you in the next one.

Remember - you're just Cmd+K away from your next feature!

---

## Recording Notes:
- High energy throughout
- Show genuine excitement at features
- Include small mistakes and fixes
- Reference personal journey frequently
- Keep demos quick and visual
- Emphasize free/affordable options
- Connect everything back to real use cases
- Smile, be encouraging
- Remember: teaching beginners who feel intimidated