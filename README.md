# multi-github-ssh
vim ~/.ssh/config
```config
Host github.com
  AddKeysToAgent yes
  IdentityFile ~/.ssh/exponent-mac-pro-github

Host personalgithub.com
  HostName github.com
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/anuraagbarde@gmail.com_github_rsa
```

```bash
ssh-add ~/.ssh/anuraagbarde@gmail.com_github_rsa

ls 
anuraagbarde@gmail.com_github_rsa     exponent-mac-pro-github
anuraagbarde@gmail.com_github_rsa.pub exponent-mac-pro-github.pub
known_hosts config


ssh-add -l
ssh-add ~/.ssh/anuraagbarde@gmail.com_github_rsa
ssh -T git@personalgithub.com
```



# cursor settings
```bash
~/Library/Application Support/Cursor/User/settings.json
```

```json
{
  "editor.fontSize": 17,
  "editor.fontFamily": "MesloNGS NF, Menlo, Monaco, 'Courier New', monospace",
  "terminal.integrated.fontFamily": "MesloLGS NF",
  "terminal.integrated.fontSize": 15,
  "workbench.colorTheme": "Default Dark+",
  "workbench.activityBar.orientation": "vertical",
  "workbench.editor.wrapTabs": true,
  "python.analysis.typeCheckingMode": "basic",
  "python.analysis.autoFormatStrings": true,
  "python.analysis.autoImportCompletions": true,
  "python.analysis.inlayHints.callArgumentNames": "all",
  "python.analysis.inlayHints.functionReturnTypes": true,
  "python.analysis.inlayHints.pytestParameters": true,
  "python.analysis.inlayHints.variableTypes": true,
  "editor.cursorBlinking": "phase",
  "editor.formatOnSave": true,
  "redhat.telemetry.enabled": false,
  "diffEditor.ignoreTrimWhitespace": false,
  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "markdown.preview.doubleClickToSwitchToEditor": false,
  "git.confirmSync": false,
  "git.enableSmartCommit": true,
  "cursor.composer.collapsePaneInputBoxPills": true,
  "cursor.composer.shouldChimeAfterChatFinishes": true,
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "githubPullRequests.pullBranch": "never",
  "workbench.colorCustomizations": {
    "editor.background": "#19191c"
  },
  "cursorpyright.analysis.autoImportCompletions": true,
  "cursorpyright.analysis.inlayHints.callArgumentNames": "all",
  "cursorpyright.analysis.inlayHints.functionReturnTypes": true,
  "cursorpyright.analysis.inlayHints.variableTypes": true,
  "cursorpyright.analysis.typeCheckingMode": "basic",
  "terminal.integrated.profiles.osx": {
    "bash": {
      "path": "bash",
      "args": [
        "-l"
      ],
      "icon": "terminal-bash"
    },
    "zsh": {
      "path": "zsh",
      "args": [
        "-l"
      ]
    },
    "fish": {
      "path": "fish",
      "args": [
        "-l"
      ]
    },
    "tmux": {
      "path": "tmux",
      "icon": "terminal-tmux"
    },
    "pwsh": {
      "path": "pwsh",
      "icon": "terminal-powershell"
    }
  },
  "terminal.integrated.defaultProfile.osx": "zsh"
}

```
