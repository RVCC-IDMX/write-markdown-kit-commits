# SpecStory quick guide

SpecStory is a VS Code extension that automatically saves your Copilot conversations. This guide covers the essentials.

## What SpecStory does

Every time you chat with Copilot, SpecStory saves the conversation as a Markdown file in your project. This creates a searchable history of everything you discussed with the AI.

## Why this matters

- **Review later**: Go back and re-read explanations Copilot gave you
- **Learn from patterns**: See what prompts worked well
- **Write reflections**: Use your history to complete the AI collaboration summary

## Where conversations are saved

SpecStory creates a hidden folder in your project:

```
your-project/
├── .specstory/
│   └── history/
│       ├── 2026-01-22_09-15-chat.md
│       ├── 2026-01-22_10-30-chat.md
│       └── ...
```

Each file is named with the date and time of the conversation.

## Viewing your history

1. In VS Code, open the file explorer (folder icon in Activity Bar)
2. Look for the `.specstory` folder
3. Open the `history` folder inside it
4. Right-click any `.md` file and select **Open Preview**

**Note**: The `.specstory` folder starts with a dot, which means it is hidden by default on Mac and Linux. VS Code shows it anyway.

## Reading history in preview mode

History files are Markdown, so they look much better in preview:

1. Right-click the history file in the explorer
2. Select **Open Preview**
3. The conversation will display with clean formatting

**Tip:** You can also press `Cmd+Shift+V` (Mac) or `Ctrl+Shift+V` (Windows) to toggle preview.

## What you'll see in a history file

Each exchange follows this pattern:

- **Your prompt** appears after `_**User (timestamp)**_`
- **Copilot's response** appears after `_**Agent (model copilot/auto)**_`
- A horizontal line (`---`) separates each exchange

**See an example:** [HAP's Markdown learning session](https://gist.github.com/cynthiateeters/ade9da5a5796457a3385b460f3f227b5) shows what a clean history file looks like.

When copying prompts for your collaboration summary, look for the `_**User**_` sections—those contain exactly what you typed.

## Privacy

Your SpecStory history stays on your computer. It is NOT automatically uploaded anywhere **but only because of your .gitignore file.**

The `.gitignore` file in this project includes `.specstory/` which means:

- Your conversations will NOT be pushed to GitHub
- Only you can see your conversation history
- You control what parts (if any) you share
- Keeping the integrity of that file is super important

## Using history for your reflection

When completing your AI collaboration summary:

1. Open the `.specstory/history/` folder
2. Read through your conversations
3. Find the interactions that taught you the most
4. Summarize what you learned in your own words

You do not need to copy entire conversations—just reference the key moments and explain what you took away from them.
