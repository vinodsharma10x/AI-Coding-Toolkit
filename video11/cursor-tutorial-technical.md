# Cursor Tutorial for Beginners (AI Code Editor)

## Opening (00:00-00:22)

Today we're checking out Cursor AI - an AI-powered code editor that's been transforming how developers write code. I've been using this for the past few months alongside my journey with Bolt, V0, and Claude Code, and it's pretty interesting. 

I wanted to make a quick tutorial to share what I've learned and the best practices you can apply, especially if you're a beginner who hasn't used these AI coding tools before and wants to understand how to get the best results.

## Getting Started (00:22-01:00)

At this point, I'm assuming you've downloaded Cursor. If you haven't, it's free to start, and there's also a paid version for more features and unlimited usage. Even experienced developers should give it a try - it really makes you question how you've been working.

Once you have Cursor, I recommend opening a new folder. Go to File → Open Folder, create a new folder on your desktop, and open it. A lot of beginners work in whatever default folder it starts in, then lose their work because they don't know the location. So always create your own folder first.

## Planning Before Coding (01:00-01:45)

Before using any features I'm about to show you, make a plan. AI works best at solving small, specific, detailed tasks. The more context and information you give it, the better results you'll get.

If you just ask for something generic like "make me a todo app" or "build a portfolio website" with just 1-2 sentences, you'll get wildly different results. And once it starts going in one direction, it can branch off everywhere if you don't know what you want.

So have a clear vision. I recommend jotting down notes or even drawing a picture of what you want the UI to look like. This will really help guide the process.

## The Composer Feature (01:45-03:00)

Let's say you have a plan and know what you want to build. The first feature is the Composer.

To enable this: File → Preferences → Cursor Settings → Features → scroll down to Composer → Enable it. By default it's disabled.

Now press Ctrl+I (or Cmd+I on Mac) to open the Composer view. This can edit multiple files at once and create new files. I like starting with this when generating a brand new application or making major feature changes across multiple files.

Let me write a quick prompt. I'm specifying exactly what I want, including frameworks and languages:
- Express for the backend
- SQLite for database
- JavaScript, HTML, CSS with Tailwind for frontend

The key is being specific. If you don't know what to use, you can ask it for recommendations first.

## Generating the Application (03:00-04:30)

[Hit enter and watch it generate]

It's creating multiple files:
- server.js
- index.html
- styles.css
- script.js

It gives instructions for things it can't do directly, like running terminal commands. But it generates the majority of the application.

Once it's finished, I can review all these files, ask for revisions, or accept all changes. It's similar to reviewing a GitHub pull request. I'll accept all.

Now I have my complete application structure - index, script, styles, and server.

## The Chat Window (04:30-07:00)

The Composer is great for big features and getting started, but sometimes it can get crazy. It's also difficult to review all that code at once.

The next feature I use most is the Chat window. Press Ctrl+L (or Cmd+L on Mac).

Here you can ask anything - not just coding questions. It has access to your entire codebase context. You can ask about specific files or add context manually.

Press @ to add:
- Specific files (@server)
- Web search
- Images
- Documentation links
- PDFs

The more context you give, the better it performs.

Let's say I want to add more recipes to my server:
"@server Great, can you add some new recipes? Please make them more unique."

When it generates code, I can press Apply and it creates a diff right in the file - completely different from ChatGPT where you copy-paste everything. I can accept or reject changes.

If I don't like something, I can reply directly and it maintains that context.

## Codebase Search (07:00-08:00)

You can also search through your codebase. Instead of regular chat, you can ask "Where are my recipes defined?" and use Ctrl+Enter (or Cmd+Enter) to search.

It searches the whole codebase and gives you clickable links to exact locations. Anything blue is clickable - really easy to navigate, especially in larger codebases.

## Inline Completions & Editing (08:00-10:00)

While typing code, let's say I want to add another select box in index.html:

```html
<select>
```

It immediately gives long autocompletions. Hit Tab to accept. As I type, it suggests options and I can generate code significantly faster.

For modifying existing code, I can:
1. Highlight a block
2. Press Ctrl+K (inline editor)
3. Give instructions like "Add more detailed options please"
4. Review the diff
5. Accept or reject

This is a really fast way to make targeted changes when you know exactly what you want.

## Quick Recap (10:00-10:30)

Three main features:
1. **Composer (Ctrl+I)**: Multiple files, big features, new projects
2. **Chat (Ctrl+L)**: Targeted modifications, explanations, recommendations
3. **Inline (Ctrl+K)**: Quick edits to specific code blocks

## Image to Code Feature (10:30-12:00)

You can also use images to generate code. I grabbed a random login form image from the web.

In chat:
1. Add the image
2. "Can you please make a new HTML file that contains this form, make it look exactly like this"

One issue - it tries to apply to existing files. The chat won't create new files unless you use Composer. So:
1. Create new file manually: form.html
2. Apply the generated code
3. Accept changes

[Show the result in browser]

Pretty impressive! It captured the design quite well. Some spacing issues, but it even handled the diagonal line. With minor tweaks, this is production-ready.

## Important Considerations (12:00-13:00)

Cursor has supercharged my productivity, but I can only use it effectively because I already know how to code. 

Sure, complete beginners can use it, but it's significantly harder when you get stuck. Sometimes the AI makes mistakes or generates problematic code, and you need to dive in and fix it manually.

That's why understanding the fundamentals is still important. Cursor is a tool that amplifies your abilities, not replaces the need to understand what's happening.

## Closing (13:00-13:30)

Overall, Cursor has been super cool to use and definitely enhanced my productivity. It's changed how I approach development - from the Composer for large features to inline edits for quick fixes.

The key is knowing when to use each feature:
- Composer for big changes
- Chat for medium tasks and understanding
- Inline for quick, targeted edits

Give it a try, experiment with these features, and see how it can accelerate your development workflow. Remember to start with clear plans and specific instructions for the best results.

---

## Recording Notes:
- Keep technical and straightforward
- Focus on practical demonstration
- Show actual features working
- Minimal personal story
- Quick transitions between features
- Emphasize keyboard shortcuts
- Show common issues and solutions