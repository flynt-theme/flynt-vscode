# Flynt for VS Code

Warm tones. Zero visual noise. - [Flynt](https://flynt-theme.github.io/flynt) for [Visual Studio Code](https://code.visualstudio.com).

## Install

### From the Marketplace

Search for **Flynt** in the Extensions panel (`Cmd+Shift+X`) or install from the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=flynt-theme.flynt).

### From source

```sh
git clone https://github.com/flynt-theme/flynt-vscode
cd flynt-vscode
npm install
npm run package
code --install-extension flynt-0.1.0.vsix
```

## Activate

1. Open the command palette (`Cmd+Shift+P`)
2. Select **Preferences: Color Theme**
3. Choose **Flynt Dark** or **Flynt Light**

## Tips

**Disable rainbow brackets** - Flynt uses full-contrast punctuation. If you prefer that over bracket pair colorization:

```json
"editor.bracketPairColorization.enabled": false
```

## Building from source

Themes are generated from [`theme.json.tmpl`](theme.json.tmpl) using [strike](https://github.com/flynt-theme/strike).

```sh
brew tap flynt-theme/tap && brew install strike
strike build theme.json.tmpl --palette palette.json --out themes/
```

## License

MIT - [Flynt Theme](https://github.com/flynt-theme)
