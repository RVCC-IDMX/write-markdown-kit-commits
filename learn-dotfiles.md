# Dotfiles and .gitignore

Files and folders that start with a dot (`.`) have special meaning in software development. This guide explains what they are and why they matter.

## What are dotfiles?

A dotfile is any file or folder whose name starts with a period:

- `.gitignore`
- `.github/`
- `.vscode/`
- `.specstory/`

## Why the dot?

On Mac and Linux, files starting with a dot are hidden by default. This keeps project folders clean by hiding configuration files that most users do not need to see every day.

Windows does not hide these files automatically, but the convention still applies.

## Common dotfiles in projects

| File/Folder   | Purpose                                        |
| ------------- | ---------------------------------------------- |
| `.gitignore`  | Tells Git which files to NOT track             |
| `.github/`    | GitHub-specific settings and instructions      |
| `.vscode/`    | VS Code workspace settings                     |
| `.specstory/` | SpecStory conversation history                 |
| `.env`        | Environment variables (often contains secrets) |

## Understanding .gitignore

The `.gitignore` file is a list of files and folders that Git should ignore. When you run `git add` or push to GitHub, anything listed in `.gitignore` is skipped.

### Example .gitignore

```text
# Ignore SpecStory conversation history
.specstory/

# Ignore Claude Code files
.claude/

# Ignore system files
.DS_Store
Thumbs.db

# Ignore sensitive files
.env
```

### How patterns work

| Pattern          | What it ignores                           |
| ---------------- | ----------------------------------------- |
| `file.txt`       | A specific file named file.txt            |
| `*.log`          | All files ending in .log                  |
| `folder/`        | An entire folder and everything inside it |
| `!important.log` | Exception: do NOT ignore this file        |

Lines starting with `#` are comments and are ignored.

## Why .gitignore matters for privacy

Some files should never be pushed to GitHub:

- **Conversation history** (`.specstory/`) - Your AI chats are private
- **API keys and secrets** (`.env`) - Could be misused if exposed
- **Personal settings** (`.claude/`) - May contain private preferences

By listing these in `.gitignore`, you prevent accidentally sharing private information.

## The .gitignore in this project

This project's `.gitignore` includes:

```text
.specstory/
.claude/
```

This means your Copilot conversations and any Claude Code settings will stay on your computer and never be uploaded to GitHub.

## Checking what Git is tracking

To see which files Git is tracking (and which it is ignoring):

```bash
git status
```

Files listed under "Untracked files" are not being tracked. If a file you expect to see is missing, it is probably listed in `.gitignore`.
