# Flow bug: LSP dismisses unused suppress_comment warnings (v0.117

Prerequisites:
* Have VS Code installed with the Flow extension.

Steps to reproduce:

1. Run `yarn install` to install dependencies.
2. Run `code .` to open up VS code to this workspace.
3. Open `src.js` and wait for Flow server to start up.
4. Notice that `// $FlowFixMe` is underlined with a warning.
5. Add a space to the end of the file.
6. Notice that the warning disappears.

