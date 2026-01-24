# Installing VS Code extensions

Extensions add new features to VS Code. This guide shows you how to find and install them.

## Opening the extensions view

Use any of these methods:

| Method             | How                                      |
| ------------------ | ---------------------------------------- |
| Keyboard (Mac)     | Cmd+Shift+X                              |
| Keyboard (Windows) | Ctrl+Shift+X                             |
| Activity Bar       | Click the Extensions icon (four squares) |
| Menu               | View → Extensions                        |

## Finding an extension

1. Open the Extensions view
2. Type the extension name in the search box
3. Look for the correct publisher (shown below the extension name)

## Installing an extension

1. Click on the extension in the search results
2. Read the description to make sure it is what you need
3. Click the blue **Install** button
4. Wait for installation to complete

## Recommended extensions prompt

When you open a project folder, VS Code may show a notification:

> "This workspace has extension recommendations. Do you want to install them?"

This happens when the project includes a `.vscode/extensions.json` file. Clicking **Install** will add all the recommended extensions at once.

## Managing installed extensions

To see your installed extensions:

1. Open the Extensions view
2. Click the filter icon (funnel shape)
3. Select "Installed"

From here you can:

- **Disable** an extension (turns it off without removing it)
- **Uninstall** an extension (removes it completely)
- **Update** an extension (if updates are available)

## Extensions for this course

This project recommends three extensions:

| Extension           | Purpose                                  |
| ------------------- | ---------------------------------------- |
| GitHub Copilot      | AI code suggestions and completions      |
| GitHub Copilot Chat | Conversational AI assistant in VS Code   |
| SpecStory           | Saves your Copilot conversations locally |

## Troubleshooting

**Extension not working?**

- Try reloading VS Code (Cmd+Shift+P or Ctrl+Shift+P, then type "Reload Window")
- Check if the extension requires you to sign in (like GitHub Copilot)
- Make sure the extension is enabled (not disabled)

**Too many extensions?**

- Extensions can slow down VS Code if you have many installed
- Disable extensions you are not currently using
- Uninstall extensions you no longer need
