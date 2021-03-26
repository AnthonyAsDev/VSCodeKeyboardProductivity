# VSCodeKeyboardProductivity

Productivity boost with the keyboard in Visual Studio Code

## 🔥 Extensions

### **Vim**

Vim emulation for Visual Studio Code

> _Download Link_  
> https://marketplace.visualstudio.com/items?itemName=vscodevim.vim

### **Which Key**

Whichkey like menu for Visual Studio Code

> _Download Link_  
> https://marketplace.visualstudio.com/items?itemName=VSpaceCode.whichkey

### **Simple New File**

Create new files from the command palette.

> _Download Link_  
> https://marketplace.visualstudio.com/items?itemName=fayras.simple-new-file

## ⚙️ Settings

### **Vim**

<details>
  <summary>Settings</summary>

```json
{
  "vim.leader": "<space>",
  "vim.insertModeKeyBindingsNonRecursive": [
    {
      "before": ["j", "k"],
      "after": ["<esc>"]
    }
  ],
  "vim.normalModeKeyBindingsNonRecursive": [
    // Vim
    {
      "before": ["J"],
      "after": ["5", "j"]
    },
    {
      "before": ["K"],
      "after": ["5", "k"]
    },
    // Which Key
    {
      "before": [":"],
      "commands": ["whichkey.show"]
    },
    // VSCode
    {
      "name": "Close Editor",
      "before": ["<leader>", "q"],
      "commands": ["workbench.action.closeActiveEditor"]
    },
    {
      "name": "Rename Symbol",
      "before": ["<leader>", "r"],
      "commands": ["editor.action.rename"]
    },
    {
      "name": "Go to Matching Pair",
      "before": ["<leader>", "t"],
      "commands": ["editor.emmet.action.matchTag"]
    },
    {
      "name": "Focus Breadcrumbs",
      "before": ["<leader>", "y"],
      "commands": ["breadcrumbs.focusAndSelect"]
    },
    {
      "name": "Transform to Tittle Case",
      "before": ["<leader>", "u"],
      "commands": ["editor.action.transformToTitlecase"]
    },
    {
      "name": "Focus on Files Explorer",
      "before": ["<leader>", "i"],
      "commands": ["workbench.files.action.focusFilesExplorer"]
    },
    {
      "name": "Go to File",
      "before": ["<leader>", "o"],
      "commands": ["workbench.action.quickOpen"]
    },
    {
      "name": "Show All Commands",
      "before": ["<leader>", "p"],
      "commands": ["workbench.action.showCommands"]
    },
    {
      "name": "Source Action",
      "before": ["<leader>", "a"],
      "commands": ["editor.action.sourceAction"]
    },
    {
      "name": "Save",
      "before": ["<leader>", "s"],
      "commands": ["workbench.action.files.save"]
    },
    {
      "name": "Toggle Side Bar Visibility",
      "before": ["<leader>", "d"],
      "commands": ["workbench.action.toggleSidebarVisibility"]
    },
    {
      "name": "Format Document",
      "before": ["<leader>", "f"],
      "commands": ["editor.action.formatDocument"]
    },
    {
      "name": "Trigger Suggest",
      "before": ["<leader>", "g"],
      "commands": ["editor.action.triggerSuggest"]
    },
    {
      "name": "Navigate to the View on the Left",
      "before": ["<leader>", "h"],
      "commands": ["workbench.action.navigateLeft"]
    },
    {
      "name": "Navigate to the View Below",
      "before": ["<leader>", "j"],
      "commands": ["workbench.action.navigateDown"]
    },
    {
      "name": "Navigate to the View Above",
      "before": ["<leader>", "k"],
      "commands": ["workbench.action.navigateUp"]
    },
    {
      "name": "Navigate to the View on the Right",
      "before": ["<leader>", "l"],
      "commands": ["workbench.action.navigateRight"]
    },
    {
      "name": "Simple New File",
      "before": ["<leader>", "n"],
      "commands": ["extension.simpleNewFile"]
    }
  ],
  "vim.visualModeKeyBindingsNonRecursive": [
    // Vim
    {
      "before": ["J"],
      "after": ["5", "j"]
    },
    {
      "before": ["K"],
      "after": ["5", "k"]
    },
    // Which Key
    {
      "before": [":"],
      "commands": ["whichkey.show"]
    }
  ]
}
```

</details>
<br />
  
### **Which Key**

<details>
  <summary>Settings</summary>

```json
{
  "whichkey.bindings": [
    {
      "key": " ",
      "name": "Commands",
      "type": "command",
      "command": "workbench.action.showCommands"
    },
    {
      "key": "\t",
      "name": "Last buffer",
      "type": "commands",
      "commands": [
        "workbench.action.quickOpenPreviousRecentlyUsedEditorInGroup",
        "list.select"
      ]
    },
    {
      "key": "!",
      "name": "Show terminal",
      "type": "command",
      "command": "workbench.action.terminal.focus"
    },
    {
      "key": "\"",
      "name": "Open new external terminal",
      "type": "command",
      "command": "workbench.action.terminal.openNativeConsole"
    },
    {
      "key": "'",
      "name": "Show terminal",
      "type": "command",
      "command": "workbench.action.terminal.focus"
    },
    {
      "key": "*",
      "name": "Search in project with selection",
      "type": "commands",
      "commands": [
        "editor.action.addSelectionToNextFindMatch",
        "workbench.action.findInFiles",
        "search.action.focusSearchList"
      ]
    },
    {
      "key": "/",
      "name": "Search in project",
      "type": "command",
      "command": "workbench.action.findInFiles"
    },
    {
      "key": ";",
      "name": "Toggle comment",
      "type": "command",
      "command": "editor.action.commentLine"
    },
    {
      "key": "v",
      "name": "Smart select/expand region",
      "type": "transient",
      "command": "editor.action.smartSelect.grow",
      "bindings": [
        {
          "key": "v",
          "name": "Grow selection",
          "type": "command",
          "command": "editor.action.smartSelect.grow"
        },
        {
          "key": "V",
          "name": "Shrink selection",
          "type": "command",
          "command": "editor.action.smartSelect.shrink"
        }
      ]
    },
    {
      "key": "b",
      "name": "+Buffers",
      "type": "bindings",
      "bindings": [
        {
          "key": "0",
          "name": "Last buffer in window",
          "type": "command",
          "command": "workbench.action.lastEditorInGroup"
        },
        {
          "key": "1",
          "name": "First buffer in window",
          "type": "command",
          "command": "workbench.action.firstEditorInGroup"
        },
        {
          "key": "b",
          "name": "Show all buffers",
          "type": "command",
          "command": "workbench.action.showAllEditorsByMostRecentlyUsed"
        },
        {
          "key": "d",
          "name": "Close active buffer",
          "type": "command",
          "command": "workbench.action.closeActiveEditor"
        },
        {
          "key": "h",
          "name": "Move buffer into left window",
          "type": "command",
          "command": "workbench.action.moveEditorToLeftGroup"
        },
        {
          "key": "j",
          "name": "Move buffer into below window",
          "type": "command",
          "command": "workbench.action.moveEditorToBelowGroup"
        },
        {
          "key": "k",
          "name": "Move buffer into above window",
          "type": "command",
          "command": "workbench.action.moveEditorToAboveGroup"
        },
        {
          "key": "l",
          "name": "Move buffer into right window",
          "type": "command",
          "command": "workbench.action.moveEditorToRightGroup"
        },
        {
          "key": "n",
          "name": "Next buffer",
          "type": "command",
          "command": "workbench.action.nextEditor"
        },
        {
          "key": "p",
          "name": "Previous buffer",
          "type": "command",
          "command": "workbench.action.previousEditor"
        },
        {
          "key": "s",
          "name": "Scratch buffer",
          "type": "command",
          "command": "workbench.action.files.newUntitledFile"
        },
        {
          "key": "t",
          "name": "Pin buffer",
          "type": "command",
          "command": "workbench.action.pinEditor"
        },
        {
          "key": "u",
          "name": "Reopen closed buffer",
          "type": "command",
          "command": "workbench.action.reopenClosedEditor"
        },
        {
          "key": "B",
          "name": "Show all buffers in active window",
          "type": "command",
          "command": "workbench.action.showEditorsInActiveGroup"
        },
        {
          "key": "H",
          "name": "Move buffer into left window",
          "type": "command",
          "command": "workbench.action.moveEditorToLeftGroup"
        },
        {
          "key": "J",
          "name": "Move buffer into below window",
          "type": "command",
          "command": "workbench.action.moveEditorToBelowGroup"
        },
        {
          "key": "K",
          "name": "Move buffer into above window",
          "type": "command",
          "command": "workbench.action.moveEditorToAboveGroup"
        },
        {
          "key": "L",
          "name": "Move buffer into right window",
          "type": "command",
          "command": "workbench.action.moveEditorToRightGroup"
        },
        {
          "key": "M",
          "name": "Close other buffers",
          "type": "command",
          "command": "workbench.action.closeOtherEditors"
        },
        {
          "key": "P",
          "name": "Paste clipboard to buffer",
          "type": "commands",
          "commands": [
            "editor.action.selectAll",
            "editor.action.clipboardPasteAction"
          ]
        },
        {
          "key": "T",
          "name": "Unpin buffer",
          "type": "command",
          "command": "workbench.action.unpinEditor"
        },
        {
          "key": "Y",
          "name": "Copy buffer to clipboard",
          "type": "command",
          "command": "vspacecode.copyWholeBuffer"
        },
        {
          "key": "N",
          "name": "+New Buffer",
          "type": "bindings",
          "bindings": [
            {
              "key": "h",
              "name": "New untitled buffer (split left)",
              "type": "commands",
              "commands": [
                "workbench.action.splitEditorLeft",
                "workbench.action.files.newUntitledFile",
                "workbench.action.closeOtherEditors"
              ]
            },
            {
              "key": "j",
              "name": "New untitled buffer (split down)",
              "type": "commands",
              "commands": [
                "workbench.action.splitEditorDown",
                "workbench.action.files.newUntitledFile",
                "workbench.action.closeOtherEditors"
              ]
            },
            {
              "key": "k",
              "name": "New untitled buffer (split up)",
              "type": "commands",
              "commands": [
                "workbench.action.splitEditorUp",
                "workbench.action.files.newUntitledFile",
                "workbench.action.closeOtherEditors"
              ]
            },
            {
              "key": "l",
              "name": "New untitled buffer (split right)",
              "type": "commands",
              "commands": [
                "workbench.action.splitEditorRight",
                "workbench.action.files.newUntitledFile",
                "workbench.action.closeOtherEditors"
              ]
            },
            {
              "key": "n",
              "name": "New untitled buffer",
              "type": "command",
              "command": "workbench.action.files.newUntitledFile"
            }
          ]
        }
      ]
    },
    {
      "key": "c",
      "name": "+Compile/Comments",
      "type": "bindings",
      "bindings": [
        {
          "key": "c",
          "name": "Compile project",
          "type": "command",
          "command": "workbench.action.tasks.build"
        },
        {
          "key": "l",
          "name": "Toggle line comment",
          "type": "command",
          "command": "editor.action.commentLine"
        },
        {
          "key": "n",
          "name": "Next error",
          "type": "command",
          "command": "editor.action.marker.nextInFiles"
        },
        {
          "key": "N",
          "name": "Previous error",
          "type": "command",
          "command": "editor.action.marker.prevInFiles"
        }
      ]
    },
    {
      "key": "d",
      "name": "+Debug",
      "type": "bindings",
      "bindings": [
        {
          "key": "c",
          "name": "Continue debug",
          "type": "command",
          "command": "workbench.action.debug.continue"
        },
        {
          "key": "d",
          "name": "Start debug",
          "type": "command",
          "command": "workbench.action.debug.start"
        },
        {
          "key": "i",
          "name": "Step into",
          "type": "command",
          "command": "workbench.action.debug.stepInto"
        },
        {
          "key": "j",
          "name": "Jump to cursor",
          "type": "command",
          "command": "debug.jumpToCursor"
        },
        {
          "key": "o",
          "name": "Step out",
          "type": "command",
          "command": "workbench.action.debug.stepOut"
        },
        {
          "key": "p",
          "name": "Pause debug",
          "type": "command",
          "command": "workbench.action.debug.pause"
        },
        {
          "key": "s",
          "name": "Step over",
          "type": "command",
          "command": "workbench.action.debug.stepOver"
        },
        {
          "key": "v",
          "name": "REPL",
          "type": "command",
          "command": "workbench.debug.action.toggleRepl"
        },
        {
          "key": "w",
          "name": "Focus on watch window",
          "type": "command",
          "command": "workbench.debug.action.focusWatchView"
        },
        {
          "key": "D",
          "name": "Run without debugging",
          "type": "command",
          "command": "workbench.action.debug.run"
        },
        {
          "key": "R",
          "name": "Restart debug",
          "type": "command",
          "command": "workbench.action.debug.restart"
        },
        {
          "key": "S",
          "name": "Stop debug",
          "type": "command",
          "command": "workbench.action.debug.stop"
        },
        {
          "key": "W",
          "name": "Add to watch",
          "type": "command",
          "command": "editor.debug.action.selectionToWatch"
        },
        {
          "key": "b",
          "name": "+Breakpoint",
          "type": "bindings",
          "bindings": [
            {
              "key": "b",
              "name": "Toggle breakpoint",
              "type": "command",
              "command": "editor.debug.action.toggleBreakpoint"
            },
            {
              "key": "c",
              "name": "Add conditional breakpoint",
              "type": "command",
              "command": "editor.debug.action.conditionalBreakpoint"
            },
            {
              "key": "d",
              "name": "Delete breakpoint",
              "type": "command",
              "command": "debug.removeBreakpoint"
            },
            {
              "key": "e",
              "name": "Enable breakpoint",
              "type": "command",
              "command": "debug.enableOrDisableBreakpoint"
            },
            {
              "key": "f",
              "name": "Add function breakpoint",
              "type": "command",
              "command": "workbench.debug.viewlet.action.addFunctionBreakpointAction"
            },
            {
              "key": "i",
              "name": "Toggle inline breakpoint",
              "type": "command",
              "command": "editor.debug.action.toggleInlineBreakpoint"
            },
            {
              "key": "n",
              "name": "Next breakpoint",
              "type": "transient",
              "command": "editor.debug.action.goToNextBreakpoint",
              "bindings": [
                {
                  "key": "n",
                  "name": "Next breakpoint",
                  "type": "command",
                  "command": "editor.debug.action.goToNextBreakpoint"
                },
                {
                  "key": "p",
                  "name": "Previous breakpoint",
                  "type": "command",
                  "command": "editor.debug.action.goToPreviousBreakpoint"
                }
              ]
            },
            {
              "key": "p",
              "name": "Previous breakpoint",
              "type": "transient",
              "command": "editor.debug.action.goToPreviousBreakpoint",
              "bindings": [
                {
                  "key": "n",
                  "name": "Next breakpoint",
                  "type": "command",
                  "command": "editor.debug.action.goToNextBreakpoint"
                },
                {
                  "key": "p",
                  "name": "Previous breakpoint",
                  "type": "command",
                  "command": "editor.debug.action.goToPreviousBreakpoint"
                }
              ]
            },
            {
              "key": "s",
              "name": "Disable breakpoint",
              "type": "command",
              "command": "debug.enableOrDisableBreakpoint"
            },
            {
              "key": "D",
              "name": "Delete all breakpoints",
              "type": "command",
              "command": "workbench.debug.viewlet.action.removeAllBreakpoints"
            },
            {
              "key": "E",
              "name": "Enable all breakpoints",
              "type": "command",
              "command": "workbench.debug.viewlet.action.enableAllBreakpoints"
            },
            {
              "key": "S",
              "name": "Disable all breakpoints",
              "type": "command",
              "command": "workbench.debug.viewlet.action.disableAllBreakpoints"
            }
          ]
        }
      ]
    },
    {
      "key": "e",
      "name": "+Errors",
      "type": "bindings",
      "bindings": [
        {
          "key": ".",
          "name": "Error transient",
          "type": "transient",
          "bindings": [
            {
              "key": "n",
              "name": "Next error",
              "type": "command",
              "command": "editor.action.marker.nextInFiles"
            },
            {
              "key": "p",
              "name": "Previous error",
              "type": "command",
              "command": "editor.action.marker.prevInFiles"
            },
            {
              "key": "N",
              "name": "Previous error",
              "type": "command",
              "command": "editor.action.marker.prevInFiles"
            }
          ]
        },
        {
          "key": "l",
          "name": "List errors",
          "type": "command",
          "command": "workbench.actions.view.problems"
        },
        {
          "key": "n",
          "name": "Next error",
          "type": "command",
          "command": "editor.action.marker.nextInFiles"
        },
        {
          "key": "p",
          "name": "Previous error",
          "type": "command",
          "command": "editor.action.marker.prevInFiles"
        },
        {
          "key": "N",
          "name": "Previous error",
          "type": "command",
          "command": "editor.action.marker.prevInFiles"
        }
      ]
    },
    {
      "key": "f",
      "name": "+File",
      "type": "bindings",
      "bindings": [
        {
          "key": "f",
          "name": "Open file/folder",
          "type": "command",
          "command": "file-browser.open"
        },
        {
          "key": "l",
          "name": "Change file language",
          "type": "command",
          "command": "workbench.action.editor.changeLanguageMode"
        },
        {
          "key": "n",
          "name": "New file",
          "type": "command",
          "command": "explorer.newFile"
        },
        {
          "key": "o",
          "name": "+Open with",
          "type": "command",
          "command": "explorer.openWith"
        },
        {
          "key": "r",
          "name": "+Open recent",
          "type": "command",
          "command": "workbench.action.openRecent"
        },
        {
          "key": "s",
          "name": "Save file",
          "type": "command",
          "command": "workbench.action.files.save"
        },
        {
          "key": "t",
          "name": "Toggle tree/explorer view",
          "type": "conditional",
          "bindings": [
            {
              "key": "",
              "name": "Show explorer view",
              "type": "command",
              "command": "workbench.view.explorer"
            },
            {
              "key": "when:sideBarVisible && explorerViewletVisible",
              "name": "Hide side bar",
              "type": "command",
              "command": "workbench.action.toggleSidebarVisibility"
            }
          ]
        },
        {
          "key": "w",
          "name": "Open active in new window",
          "type": "command",
          "command": "workbench.action.files.showOpenedFileInNewWindow"
        },
        {
          "key": "D",
          "name": "Delete current file",
          "type": "commands",
          "commands": [
            "workbench.files.action.showActiveFileInExplorer",
            "deleteFile"
          ]
        },
        {
          "key": "L",
          "name": "Locate file",
          "type": "command",
          "command": "revealFileInOS"
        },
        {
          "key": "R",
          "name": "Rename file",
          "type": "commands",
          "commands": [
            "workbench.files.action.showActiveFileInExplorer",
            "renameFile"
          ]
        },
        {
          "key": "S",
          "name": "Save all files",
          "type": "command",
          "command": "workbench.action.files.saveAll"
        },
        {
          "key": "T",
          "name": "Show active file in tree/explorer view",
          "type": "command",
          "command": "workbench.files.action.showActiveFileInExplorer"
        },
        {
          "key": "e",
          "name": "+Emacs/VSpaceCode",
          "type": "bindings",
          "bindings": [
            {
              "key": "d",
              "name": "Open settings",
              "type": "command",
              "command": "workbench.action.openGlobalSettings"
            },
            {
              "key": "k",
              "name": "Open global key bindings",
              "type": "command",
              "command": "workbench.action.openGlobalKeybindings"
            },
            {
              "key": "l",
              "name": "Open language settings",
              "type": "command",
              "command": "workbench.action.configureLanguageBasedSettings"
            },
            {
              "key": "s",
              "name": "Configure user snippets",
              "type": "command",
              "command": "workbench.action.openSnippets"
            },
            {
              "key": "w",
              "name": "Open workspace settings",
              "type": "command",
              "command": "workbench.action.openWorkspaceSettings"
            },
            {
              "key": "D",
              "name": "Open settings JSON",
              "type": "command",
              "command": "workbench.action.openSettingsJson"
            },
            {
              "key": "K",
              "name": "Open global key bindings JSON",
              "type": "command",
              "command": "workbench.action.openGlobalKeybindingsFile"
            },
            {
              "key": "W",
              "name": "Open workspace settings JSON",
              "type": "command",
              "command": "workbench.action.openWorkspaceSettingsFile"
            }
          ]
        },
        {
          "key": "i",
          "name": "+Indentation",
          "type": "bindings",
          "bindings": [
            {
              "key": "d",
              "name": "Detect indentation",
              "type": "command",
              "command": "editor.action.detectIndentation"
            },
            {
              "key": "i",
              "name": "Change indentation",
              "type": "command",
              "command": "changeEditorIndentation"
            },
            {
              "key": "r",
              "name": "Reindent",
              "type": "command",
              "command": "editor.action.reindentlines"
            },
            {
              "key": "s",
              "name": "Convert indentation to spaces",
              "type": "command",
              "command": "editor.action.indentationToSpaces"
            },
            {
              "key": "t",
              "name": "Convert indentation to tabs",
              "type": "command",
              "command": "editor.action.indentationToTabs"
            },
            {
              "key": "R",
              "name": "Reindent selected",
              "type": "command",
              "command": "editor.action.reindentselectedlines"
            }
          ]
        }
      ]
    },
    {
      "key": "g",
      "name": "+Git",
      "type": "bindings",
      "bindings": [
        {
          "key": "i",
          "name": "Init",
          "type": "command",
          "command": "git.init"
        },
        {
          "key": "g",
          "name": "Source Control",
          "type": "command",
          "command": "workbench.view.scm"
        },
        {
          "key": "p",
          "name": "Pull",
          "type": "command",
          "command": "git.pull"
        },
        {
          "key": "P",
          "name": "Push",
          "type": "command",
          "command": "git.push"
        },
        {
          "key": "f",
          "name": "Fetch",
          "type": "command",
          "command": "git.fetch"
        },
        {
          "key": "y",
          "name": "Clone",
          "type": "command",
          "command": "git.clone"
        },
        {
          "key": "o",
          "name": "Checkout to",
          "type": "command",
          "command": "git.checkout"
        },
        {
          "key": "c",
          "name": "+Commit",
          "type": "bindings",
          "bindings": [
            {
              "key": "c",
              "name": "Commit",
              "type": "command",
              "command": "git.commit"
            },
            {
              "key": "s",
              "name": "Commit Staged",
              "type": "command",
              "command": "git.commitStaged"
            },
            {
              "key": "a",
              "name": "Commit All",
              "type": "command",
              "command": "git.commitAll"
            },
            {
              "key": "u",
              "name": "Undo Last Commit",
              "type": "command",
              "command": "git.undoCommit"
            },
            {
              "key": "r",
              "name": "Abort Rebase",
              "type": "command",
              "command": "git.rebaseAbort"
            }
          ]
        },
        {
          "key": "s",
          "name": "+Changes",
          "type": "bindings",
          "bindings": [
            {
              "key": "s",
              "name": "Stage Change",
              "type": "command",
              "command": "git.stage"
            },
            {
              "key": "S",
              "name": "Stage All Changes",
              "type": "command",
              "command": "git.stageAll"
            },
            {
              "key": "u",
              "name": "Unstage Changes",
              "type": "command",
              "command": "git.unstage"
            },
            {
              "key": "U",
              "name": "Unstage All Changes",
              "type": "command",
              "command": "git.unstageAll"
            },
            {
              "key": "d",
              "name": "Discard Changes",
              "type": "command",
              "command": "git.clean"
            },
            {
              "key": "D",
              "name": "Discard All Changes",
              "type": "command",
              "command": "git.cleanAll"
            }
          ]
        },
        {
          "key": "b",
          "name": "+Branch",
          "type": "bindings",
          "bindings": [
            {
              "key": "c",
              "name": "Create Branch",
              "type": "command",
              "command": "git.branch"
            },
            {
              "key": "d",
              "name": "Delete Branch",
              "type": "command",
              "command": "git.deleteBranch"
            },
            {
              "key": "m",
              "name": "Merge Branch",
              "type": "command",
              "command": "git.merge"
            },
            {
              "key": "p",
              "name": "Publish Branch",
              "type": "command",
              "command": "git.publish"
            },
            {
              "key": "r",
              "name": "Rebase Branch",
              "type": "command",
              "command": "git.rebase"
            },
            {
              "key": "R",
              "name": "Rename Branch",
              "type": "command",
              "command": "git.renameBranch"
            }
          ]
        },
        {
          "key": "h",
          "name": "+Stash",
          "type": "bindings",
          "bindings": [
            {
              "key": "s",
              "name": "Stash",
              "type": "command",
              "command": "git.stash"
            },
            {
              "key": "a",
              "name": "Apply Stash",
              "type": "command",
              "command": "git.stashApply"
            },
            {
              "key": "A",
              "name": "Apply Latest Stash",
              "type": "command",
              "command": "git.stashApplyLatest"
            },
            {
              "key": "d",
              "name": "Drop Stash",
              "type": "command",
              "command": "git.stashDrop"
            },
            {
              "key": "p",
              "name": "Pop Stash",
              "type": "command",
              "command": "git.stashPop"
            },
            {
              "key": "P",
              "name": "Pop Latest Stash",
              "type": "command",
              "command": "git.stashPopLatest"
            }
          ]
        },
        {
          "key": "t",
          "name": "+Tag",
          "type": "bindings",
          "bindings": [
            {
              "key": "c",
              "name": "Create Tag",
              "type": "command",
              "command": "git.createTag"
            },
            {
              "key": "d",
              "name": "Delete Tag",
              "type": "command",
              "command": "git.deleteTag"
            }
          ]
        },
        {
          "key": "r",
          "name": "+Remote",
          "type": "bindings",
          "bindings": [
            {
              "key": "a",
              "name": "Add Remote",
              "type": "command",
              "command": "git.addRemote"
            },
            {
              "key": "r",
              "name": "Remove Remote",
              "type": "command",
              "command": "git.removeRemote"
            }
          ]
        }
      ]
    },
    {
      "key": "h",
      "name": "+Help",
      "type": "bindings",
      "bindings": [
        {
          "key": "d",
          "name": "Open VSCode Documentation",
          "type": "command",
          "command": "workbench.action.openDocumentationUrl"
        },
        {
          "key": "k",
          "name": "Open global key bindings",
          "type": "command",
          "command": "workbench.action.openGlobalKeybindings"
        },
        {
          "key": "I",
          "name": "Report VSCode Issue",
          "type": "command",
          "command": "workbench.action.openIssueReporter"
        },
        {
          "key": "T",
          "name": "Open VSCode Tutorial",
          "type": "command",
          "command": "workbench.action.showInteractivePlayground"
        }
      ]
    },
    {
      "key": "i",
      "name": "+Insert",
      "type": "bindings",
      "bindings": [
        {
          "key": "j",
          "name": "Insert line below",
          "type": "command",
          "command": "editor.action.insertLineAfter"
        },
        {
          "key": "k",
          "name": "Insert line above",
          "type": "command",
          "command": "editor.action.insertLineBefore"
        },
        {
          "key": "s",
          "name": "Insert snippet",
          "type": "command",
          "command": "editor.action.insertSnippet"
        }
      ]
    },
    {
      "key": "j",
      "name": "+Jump/Join/Split",
      "type": "bindings",
      "bindings": [
        {
          "key": "+",
          "name": "Format buffer",
          "type": "command",
          "command": "editor.action.formatDocument"
        },
        {
          "key": "=",
          "name": "Format region or buffer",
          "type": "command",
          "command": "editor.action.format"
        },
        {
          "key": "c",
          "name": "Jump to previous change",
          "type": "command",
          "command": "workbench.action.editor.previousChange"
        },
        {
          "key": "i",
          "name": "Jump to symbol in buffer",
          "type": "command",
          "command": "workbench.action.gotoSymbol"
        },
        {
          "key": "j",
          "name": "Jump to character",
          "type": "command",
          "command": "vim.remap",
          "args": {
            "after": ["leader", "leader", "s"]
          }
        },
        {
          "key": "l",
          "name": "Jump to line",
          "type": "command",
          "command": "vim.remap",
          "args": {
            "after": ["leader", "leader", "leader", "b", "d", "j", "k"]
          }
        },
        {
          "key": "n",
          "name": "Split new line",
          "type": "command",
          "command": "lineBreakInsert"
        },
        {
          "key": "v",
          "name": "Jump to outline/variables",
          "type": "command",
          "command": "breadcrumbs.focusAndSelect"
        },
        {
          "key": "w",
          "name": "Jump to word",
          "type": "command",
          "command": "vim.remap",
          "args": {
            "after": ["leader", "leader", "leader", "b", "d", "w"]
          }
        },
        {
          "key": "C",
          "name": "Jump to next change",
          "type": "command",
          "command": "workbench.action.editor.nextChange"
        },
        {
          "key": "I",
          "name": "Jump to symbol in workspace",
          "type": "command",
          "command": "workbench.action.showAllSymbols"
        }
      ]
    },
    {
      "key": "l",
      "name": "+Layouts",
      "type": "bindings",
      "bindings": [
        {
          "key": "d",
          "name": "Close workspace",
          "type": "command",
          "command": "workbench.action.closeFolder"
        }
      ]
    },
    {
      "key": "p",
      "name": "+Project",
      "type": "bindings",
      "bindings": [
        {
          "key": "c",
          "name": "Compile project",
          "type": "command",
          "command": "workbench.action.tasks.build"
        },
        {
          "key": "f",
          "name": "+Find file in project",
          "type": "command",
          "command": "workbench.action.quickOpen"
        },
        {
          "key": "l",
          "name": "+Switch project",
          "type": "command",
          "command": "workbench.action.openRecent"
        },
        {
          "key": "p",
          "name": "+Switch project",
          "type": "command",
          "command": "workbench.action.openRecent"
        },
        {
          "key": "t",
          "name": "Show tree/explorer view",
          "type": "command",
          "command": "workbench.view.explorer"
        },
        {
          "key": "R",
          "name": "+Replace in files",
          "type": "command",
          "command": "workbench.action.replaceInFiles"
        },
        {
          "key": "T",
          "name": "Test project",
          "type": "command",
          "command": "workbench.action.tasks.test"
        }
      ]
    },
    {
      "key": "q",
      "name": "+Quit",
      "type": "bindings",
      "bindings": [
        {
          "key": "f",
          "name": "Close frame",
          "type": "command",
          "command": "workbench.action.closeWindow"
        },
        {
          "key": "q",
          "name": "Close frame",
          "type": "command",
          "command": "workbench.action.closeWindow"
        },
        {
          "key": "r",
          "name": "Reload frame",
          "type": "command",
          "command": "workbench.action.reloadWindow"
        },
        {
          "key": "s",
          "name": "Save all and close frame",
          "type": "commands",
          "commands": [
            "workbench.action.files.saveAll",
            "workbench.action.closeWindow"
          ]
        },
        {
          "key": "Q",
          "name": "Quit application",
          "type": "command",
          "command": "workbench.action.quit"
        },
        {
          "key": "R",
          "name": "Reload frame with extensions disabled",
          "type": "command",
          "command": "workbench.action.reloadWindowWithExtensionsDisabled"
        }
      ]
    },
    {
      "key": "r",
      "name": "+Resume",
      "type": "bindings",
      "bindings": [
        {
          "key": "b",
          "name": "Recent buffers",
          "type": "command",
          "command": "workbench.action.showAllEditorsByMostRecentlyUsed"
        },
        {
          "key": "s",
          "name": "Search in project",
          "type": "command",
          "command": "workbench.action.findInFiles"
        }
      ]
    },
    {
      "key": "s",
      "name": "+Search/Symbol",
      "type": "bindings",
      "bindings": [
        {
          "key": "c",
          "name": "Clear highlight",
          "type": "command",
          "command": "vim.remap",
          "args": {
            "commands": [
              {
                "command": ":noh"
              }
            ]
          }
        },
        {
          "key": "e",
          "name": "Edit symbol",
          "type": "command",
          "command": "editor.action.rename"
        },
        {
          "key": "h",
          "name": "Highlight symbol",
          "type": "transient",
          "command": "editor.action.wordHighlight.trigger",
          "bindings": [
            {
              "key": "/",
              "name": "Search in project with selection",
              "type": "commands",
              "commands": [
                "editor.action.addSelectionToNextFindMatch",
                "workbench.action.findInFiles"
              ]
            },
            {
              "key": "n",
              "name": "Next occurrence",
              "type": "command",
              "command": "editor.action.wordHighlight.next"
            },
            {
              "key": "p",
              "name": "Previous occurrence",
              "type": "command",
              "command": "editor.action.wordHighlight.prev"
            },
            {
              "key": "N",
              "name": "Previous occurrence",
              "type": "command",
              "command": "editor.action.wordHighlight.prev"
            }
          ]
        },
        {
          "key": "j",
          "name": "Jump to symbol in buffer",
          "type": "command",
          "command": "workbench.action.gotoSymbol"
        },
        {
          "key": "p",
          "name": "Search in project",
          "type": "command",
          "command": "workbench.action.findInFiles"
        },
        {
          "key": "r",
          "name": "Search all references",
          "type": "command",
          "command": "editor.action.referenceSearch.trigger"
        },
        {
          "key": "J",
          "name": "Jump to symbol in workspace",
          "type": "command",
          "command": "workbench.action.showAllSymbols"
        },
        {
          "key": "P",
          "name": "Search in project with selection",
          "type": "commands",
          "commands": [
            "editor.action.addSelectionToNextFindMatch",
            "workbench.action.findInFiles"
          ]
        },
        {
          "key": "R",
          "name": "Search all references in side bar",
          "type": "command",
          "command": "references-view.find"
        }
      ]
    },
    {
      "key": "t",
      "name": "+Toggles",
      "type": "bindings",
      "bindings": [
        {
          "key": "c",
          "name": "Toggle find case sensitive",
          "type": "command",
          "command": "toggleFindCaseSensitive"
        },
        {
          "key": "l",
          "name": "Toggle word wrap",
          "type": "command",
          "command": "editor.action.toggleWordWrap"
        },
        {
          "key": "w",
          "name": "Toggle render whitespace",
          "type": "command",
          "command": "editor.action.toggleRenderWhitespace"
        }
      ]
    },
    {
      "key": "w",
      "name": "+Window",
      "type": "bindings",
      "bindings": [
        {
          "key": "-",
          "name": "Split window below",
          "type": "command",
          "command": "workbench.action.splitEditorDown"
        },
        {
          "key": "/",
          "name": "Split window right",
          "type": "command",
          "command": "workbench.action.splitEditor"
        },
        {
          "key": "=",
          "name": "Reset window sizes",
          "type": "command",
          "command": "workbench.action.evenEditorWidths"
        },
        {
          "key": "[",
          "name": "Shrink window",
          "type": "transient",
          "command": "workbench.action.decreaseViewSize",
          "bindings": [
            {
              "key": "[",
              "name": "Shrink window",
              "type": "command",
              "command": "workbench.action.decreaseViewSize"
            },
            {
              "key": "]",
              "name": "Enlarge window",
              "type": "command",
              "command": "workbench.action.increaseViewSize"
            }
          ]
        },
        {
          "key": "]",
          "name": "Enlarge window",
          "type": "transient",
          "command": "workbench.action.increaseViewSize",
          "bindings": [
            {
              "key": "[",
              "name": "Shrink window",
              "type": "command",
              "command": "workbench.action.decreaseViewSize"
            },
            {
              "key": "]",
              "name": "Enlarge window",
              "type": "command",
              "command": "workbench.action.increaseViewSize"
            }
          ]
        },
        {
          "key": "d",
          "name": "Close window",
          "type": "command",
          "command": "workbench.action.closeEditorsInGroup"
        },
        {
          "key": "h",
          "name": "Focus window left",
          "type": "command",
          "command": "workbench.action.focusPreviousGroup"
        },
        {
          "key": "j",
          "name": "Focus window down",
          "type": "command",
          "command": "workbench.action.focusBelowGroup"
        },
        {
          "key": "k",
          "name": "Focus window up",
          "type": "command",
          "command": "workbench.action.focusAboveGroup"
        },
        {
          "key": "l",
          "name": "Focus window right",
          "type": "command",
          "command": "workbench.action.focusNextGroup"
        },
        {
          "key": "m",
          "name": "Maximize window",
          "type": "command",
          "command": "workbench.action.toggleEditorWidths"
        },
        {
          "key": "o",
          "name": "Switch frame",
          "type": "command",
          "command": "workbench.action.quickSwitchWindow"
        },
        {
          "key": "s",
          "name": "Split window below",
          "type": "command",
          "command": "workbench.action.splitEditorDown"
        },
        {
          "key": "v",
          "name": "Split window right",
          "type": "command",
          "command": "workbench.action.splitEditor"
        },
        {
          "key": "w",
          "name": "Focus next window",
          "type": "command",
          "command": "workbench.action.focusNextGroup"
        },
        {
          "key": "x",
          "name": "Close all windows",
          "type": "command",
          "command": "workbench.action.closeAllGroups"
        },
        {
          "key": "z",
          "name": "Combine all buffers",
          "type": "command",
          "command": "workbench.action.joinAllGroups"
        },
        {
          "key": "D",
          "name": "Close all other windows",
          "type": "command",
          "command": "workbench.action.closeEditorsInOtherGroups"
        },
        {
          "key": "F",
          "name": "Open new empty frame",
          "type": "command",
          "command": "workbench.action.newWindow"
        },
        {
          "key": "H",
          "name": "Move window left",
          "type": "command",
          "command": "workbench.action.moveActiveEditorGroupLeft"
        },
        {
          "key": "J",
          "name": "Move window down",
          "type": "command",
          "command": "workbench.action.moveActiveEditorGroupDown"
        },
        {
          "key": "K",
          "name": "Move window up",
          "type": "command",
          "command": "workbench.action.moveActiveEditorGroupUp"
        },
        {
          "key": "L",
          "name": "Move window right",
          "type": "command",
          "command": "workbench.action.moveActiveEditorGroupRight"
        },
        {
          "key": "M",
          "name": "Maximize window and hide side bar",
          "type": "command",
          "command": "workbench.action.maximizeEditor"
        },
        {
          "key": "W",
          "name": "Focus previous window",
          "type": "command",
          "command": "workbench.action.focusPreviousGroup"
        }
      ]
    },
    {
      "key": "x",
      "name": "+Text",
      "type": "bindings",
      "bindings": [
        {
          "key": ".",
          "name": "Quick fix",
          "type": "command",
          "command": "editor.action.quickFix"
        },
        {
          "key": "a",
          "name": "Find all references",
          "type": "command",
          "command": "editor.action.referenceSearch.trigger"
        },
        {
          "key": "i",
          "name": "Organize Imports",
          "type": "command",
          "command": "editor.action.organizeImports"
        },
        {
          "key": "r",
          "name": "Rename symbol",
          "type": "command",
          "command": "editor.action.rename"
        },
        {
          "key": "u",
          "name": "To lower case",
          "type": "command",
          "command": "editor.action.transformToLowercase"
        },
        {
          "key": "J",
          "name": "Move lines down",
          "type": "transient",
          "command": "editor.action.moveLinesDownAction",
          "bindings": [
            {
              "key": "J",
              "name": "Move lines down",
              "type": "command",
              "command": "editor.action.moveLinesDownAction"
            },
            {
              "key": "K",
              "name": "Move lines up",
              "type": "command",
              "command": "editor.action.moveLinesUpAction"
            }
          ]
        },
        {
          "key": "K",
          "name": "Move lines up",
          "type": "transient",
          "command": "editor.action.moveLinesUpAction",
          "bindings": [
            {
              "key": "J",
              "name": "Move lines down",
              "type": "command",
              "command": "editor.action.moveLinesDownAction"
            },
            {
              "key": "K",
              "name": "Move lines up",
              "type": "command",
              "command": "editor.action.moveLinesUpAction"
            }
          ]
        },
        {
          "key": "R",
          "name": "Refactor",
          "type": "command",
          "command": "editor.action.refactor"
        },
        {
          "key": "U",
          "name": "To upper case",
          "type": "command",
          "command": "editor.action.transformToUppercase"
        },
        {
          "key": "d",
          "name": "+Delete",
          "type": "bindings",
          "bindings": [
            {
              "key": "w",
              "name": "Delete trailing whitespace",
              "type": "command",
              "command": "editor.action.trimTrailingWhitespace"
            }
          ]
        },
        {
          "key": "l",
          "name": "+Lines",
          "type": "bindings",
          "bindings": [
            {
              "key": "d",
              "name": "Duplicate lines down",
              "type": "command",
              "command": "editor.action.copyLinesDownAction"
            },
            {
              "key": "s",
              "name": "Sort lines in ascending order",
              "type": "command",
              "command": "editor.action.sortLinesAscending"
            },
            {
              "key": "D",
              "name": "Duplicate lines up",
              "type": "command",
              "command": "editor.action.copyLinesUpAction"
            },
            {
              "key": "S",
              "name": "Sort lines in descending order",
              "type": "command",
              "command": "editor.action.sortLinesDescending"
            }
          ]
        },
        {
          "key": "m",
          "name": "+Merge conflict",
          "type": "bindings",
          "bindings": [
            {
              "key": "b",
              "name": "Accept both",
              "type": "command",
              "command": "merge-conflict.accept.both"
            },
            {
              "key": "c",
              "name": "Accept current",
              "type": "command",
              "command": "merge-conflict.accept.current"
            },
            {
              "key": "i",
              "name": "Accept incoming",
              "type": "command",
              "command": "merge-conflict.accept.incoming"
            },
            {
              "key": "k",
              "name": "Compare current conflict",
              "type": "command",
              "command": "merge-conflict.compare"
            },
            {
              "key": "n",
              "name": "Next Conflict",
              "type": "command",
              "command": "merge-conflict.next"
            },
            {
              "key": "s",
              "name": "Accept selection",
              "type": "command",
              "command": "merge-conflict.accept.selection"
            },
            {
              "key": "B",
              "name": "Accept all both",
              "type": "command",
              "command": "merge-conflict.accept.all-both"
            },
            {
              "key": "C",
              "name": "Accept all current",
              "type": "command",
              "command": "merge-conflict.accept.all-current"
            },
            {
              "key": "I",
              "name": "Accept all incoming",
              "type": "command",
              "command": "merge-conflict.accept.all-incoming"
            },
            {
              "key": "N",
              "name": "Previous Conflict",
              "type": "command",
              "command": "merge-conflict.previous"
            }
          ]
        }
      ]
    },
    {
      "key": "z",
      "name": "+Zoom/Fold",
      "type": "bindings",
      "bindings": [
        {
          "key": "f",
          "name": "+Frame",
          "type": "transient",
          "bindings": [
            {
              "key": "+",
              "name": "Zoom in",
              "type": "command",
              "command": "workbench.action.zoomIn"
            },
            {
              "key": "-",
              "name": "Zoom out",
              "type": "command",
              "command": "workbench.action.zoomOut"
            },
            {
              "key": "0",
              "name": "Reset zoom",
              "type": "command",
              "command": "workbench.action.zoomReset"
            },
            {
              "key": "=",
              "name": "Zoom in",
              "type": "command",
              "command": "workbench.action.zoomIn"
            },
            {
              "key": "j",
              "name": "Zoom out",
              "type": "command",
              "command": "workbench.action.zoomOut"
            },
            {
              "key": "k",
              "name": "Zoom in",
              "type": "command",
              "command": "workbench.action.zoomIn"
            }
          ]
        },
        {
          "key": "i",
          "name": "+Image preview",
          "type": "transient",
          "bindings": [
            {
              "key": "+",
              "name": "Zoom in",
              "type": "command",
              "command": "imagePreview.zoomIn"
            },
            {
              "key": "-",
              "name": "Zoom out",
              "type": "command",
              "command": "imagePreview.zoomOut"
            },
            {
              "key": "=",
              "name": "Zoom in",
              "type": "command",
              "command": "imagePreview.zoomIn"
            }
          ]
        },
        {
          "key": "x",
          "name": "+Font",
          "type": "transient",
          "bindings": [
            {
              "key": "+",
              "name": "Zoom in",
              "type": "command",
              "command": "editor.action.fontZoomIn"
            },
            {
              "key": "-",
              "name": "Zoom out",
              "type": "command",
              "command": "editor.action.fontZoomOut"
            },
            {
              "key": "0",
              "name": "Reset zoom",
              "type": "command",
              "command": "editor.action.fontZoomReset"
            },
            {
              "key": "=",
              "name": "Zoom in",
              "type": "command",
              "command": "editor.action.fontZoomIn"
            },
            {
              "key": "j",
              "name": "Zoom out",
              "type": "command",
              "command": "editor.action.fontZoomOut"
            },
            {
              "key": "k",
              "name": "Zoom in",
              "type": "command",
              "command": "editor.action.fontZoomIn"
            }
          ]
        },
        {
          "key": ".",
          "name": "+Fold",
          "type": "bindings",
          "bindings": [
            {
              "key": "a",
              "name": "Toggle: around a point",
              "type": "command",
              "command": "editor.toggleFold"
            },
            {
              "key": "b",
              "name": "Close: all block comments",
              "type": "command",
              "command": "editor.foldAllBlockComments"
            },
            {
              "key": "c",
              "name": "Close: at a point",
              "type": "command",
              "command": "editor.fold"
            },
            {
              "key": "g",
              "name": "Close: all regions",
              "type": "command",
              "command": "editor.foldAllMarkerRegions"
            },
            {
              "key": "m",
              "name": "Close: all",
              "type": "command",
              "command": "editor.foldAll"
            },
            {
              "key": "o",
              "name": "Open: at a point",
              "type": "command",
              "command": "editor.unfold"
            },
            {
              "key": "r",
              "name": "Open: all",
              "type": "command",
              "command": "editor.unfoldAll"
            },
            {
              "key": "G",
              "name": "Open: all regions",
              "type": "command",
              "command": "editor.unfoldAllMarkerRegions"
            },
            {
              "key": "O",
              "name": "Open: recursively",
              "type": "command",
              "command": "editor.unfoldRecursively"
            }
          ]
        }
      ]
    },
    {
      "key": "D",
      "name": "+Diff/Compare",
      "type": "bindings",
      "bindings": [
        {
          "key": "c",
          "name": "Compare active file with clipboard",
          "type": "command",
          "command": "workbench.files.action.compareWithClipboard"
        },
        {
          "key": "m",
          "name": "Compare current merge conflict",
          "type": "command",
          "command": "merge-conflict.compare"
        },
        {
          "key": "s",
          "name": "Compare active file with saved",
          "type": "command",
          "command": "workbench.files.action.compareWithSaved"
        },
        {
          "key": "w",
          "name": "Toggle ignore trim whitespace",
          "type": "command",
          "command": "toggle.diff.ignoreTrimWhitespace"
        },
        {
          "key": "D",
          "name": "+Compare active file with",
          "type": "command",
          "command": "workbench.files.action.compareFileWith"
        }
      ]
    },
    {
      "key": "F",
      "name": "+Frame",
      "type": "bindings",
      "bindings": [
        {
          "key": "n",
          "name": "Duplicate workspace in new frame",
          "type": "command",
          "command": "workbench.action.duplicateWorkspaceInNewWindow"
        },
        {
          "key": "o",
          "name": "Switch frame",
          "type": "command",
          "command": "workbench.action.quickSwitchWindow"
        },
        {
          "key": "N",
          "name": "Open new empty frame",
          "type": "command",
          "command": "workbench.action.newWindow"
        }
      ]
    },
    {
      "key": "S",
      "name": "+Show",
      "type": "bindings",
      "bindings": [
        {
          "key": "d",
          "name": "Show debug console",
          "type": "command",
          "command": "workbench.debug.action.toggleRepl"
        },
        {
          "key": "e",
          "name": "Show explorer",
          "type": "command",
          "command": "workbench.view.explorer"
        },
        {
          "key": "g",
          "name": "Show source control",
          "type": "command",
          "command": "workbench.view.scm"
        },
        {
          "key": "n",
          "name": "Show notification",
          "type": "command",
          "command": "notifications.toggleList"
        },
        {
          "key": "o",
          "name": "Show output",
          "type": "command",
          "command": "workbench.action.output.toggleOutput"
        },
        {
          "key": "p",
          "name": "Show problem",
          "type": "command",
          "command": "workbench.actions.view.problems"
        },
        {
          "key": "r",
          "name": "Show remote explorer",
          "type": "command",
          "command": "workbench.view.remote"
        },
        {
          "key": "s",
          "name": "Show search",
          "type": "command",
          "command": "workbench.view.search"
        },
        {
          "key": "t",
          "name": "Show test",
          "type": "command",
          "command": "workbench.view.extension.test"
        },
        {
          "key": "x",
          "name": "Show extensions",
          "type": "command",
          "command": "workbench.view.extensions"
        }
      ]
    },
    {
      "key": "T",
      "name": "+UI toggles",
      "type": "bindings",
      "bindings": [
        {
          "key": "b",
          "name": "Toggle side bar visibility",
          "type": "command",
          "command": "workbench.action.toggleSidebarVisibility"
        },
        {
          "key": "c",
          "name": "Toggle centered layout",
          "type": "command",
          "command": "workbench.action.toggleCenteredLayout"
        },
        {
          "key": "i",
          "name": "Select icon theme",
          "type": "command",
          "command": "workbench.action.selectIconTheme"
        },
        {
          "key": "j",
          "name": "Toggle panel visibility",
          "type": "command",
          "command": "workbench.action.togglePanel"
        },
        {
          "key": "m",
          "name": "Toggle maximized panel",
          "type": "command",
          "command": "workbench.action.toggleMaximizedPanel"
        },
        {
          "key": "s",
          "name": "Select theme",
          "type": "command",
          "command": "workbench.action.selectTheme"
        },
        {
          "key": "t",
          "name": "Toggle tool/activity bar visibility",
          "type": "command",
          "command": "workbench.action.toggleActivityBarVisibility"
        },
        {
          "key": "z",
          "name": "Toggle zen mode",
          "type": "command",
          "command": "workbench.action.toggleZenMode"
        },
        {
          "key": "F",
          "name": "Toggle full screen",
          "type": "command",
          "command": "workbench.action.toggleFullScreen"
        },
        {
          "key": "T",
          "name": "Toggle tab visibility",
          "type": "command",
          "command": "workbench.action.toggleTabsVisibility"
        }
      ]
    },
    {
      "key": "0",
      "name": "Focus on files explorer",
      "type": "command",
      "command": "workbench.files.action.showActiveFileInExplorer"
    },
    {
      "key": "1",
      "name": "Focus 1st editor group",
      "type": "command",
      "command": "workbench.action.focusFirstEditorGroup"
    },
    {
      "key": "2",
      "name": "Focus 2nd editor group",
      "type": "command",
      "command": "workbench.action.focusSecondEditorGroup"
    },
    {
      "key": "3",
      "name": "Focus 3rd editor group",
      "type": "command",
      "command": "workbench.action.focusThirdEditorGroup"
    },
    {
      "key": "4",
      "name": "Focus 4th editor group",
      "type": "command",
      "command": "workbench.action.focusFourthEditorGroup"
    },
    {
      "key": "5",
      "name": "Focus 5th editor group",
      "type": "command",
      "command": "workbench.action.focusFifthEditorGroup"
    },
    {
      "key": "6",
      "name": "Focus 6th editor group",
      "type": "command",
      "command": "workbench.action.focusSixthEditorGroup"
    },
    {
      "key": "7",
      "name": "Focus 7th editor group",
      "type": "command",
      "command": "workbench.action.focusSeventhEditorGroup"
    },
    {
      "key": "8",
      "name": "Focus 8th editor group",
      "type": "command",
      "command": "workbench.action.focusEighthEditorGroup"
    }
  ]
}
```

</details>

<br />
