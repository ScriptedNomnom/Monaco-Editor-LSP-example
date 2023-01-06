> **Note**
> A lot of dependencies have changed and I don't have the capcity to keep this repo up to date. Maybe it will still be useful as a starting point.

# Monaco Lua Example

An example setup using sumneko's [Lua Language Server](https://github.com/sumneko/lua-language-server/) and JohnnyMorganz's [StyLua](https://github.com/JohnnyMorganz/StyLua) together with [Monaco Editor](https://github.com/microsoft/monaco-editor).

If you use linux or mac, please go to launch.ts under the src inside server folder and you see this:
- resolve(process.cwd(), 'lua-language-server/.bin/Windows/lua-language-server')
Please change Windows to others like "Mac" or "Linux" depending on what os you use.

## Features

- ✨ Syntax Highlighting
- 🚀 Autocompletion
- 🌝 EmmyLua
- ✔️ Linting
- 🦀 Formatting (via wasm)
- ⚡ Vite based client

## Info

- Right now I've tested the lua language server only on linux.
- The language server uses port `8080`, so make sure this port is free or change the port in `client/src/main.ts` and `server/src/main.ts`
- This is an npm workspaces setup, so you can run alle npm scripts inside the repository's root folder.

## Get started

Clone this repository and run run `npm install`.

## Development

Run `npm run dev` and visit `localhost:3000`.

## Production

Run `npm run build`. To start the language server run `npm run server-start`.

## Credits

- sumneko's [Lua Language Server](https://github.com/sumneko/lua-language-server/)
- JohnnyMorganz's [StyLua](https://github.com/JohnnyMorganz/StyLua)
- Typefox's [monaco-languageclient](https://github.com/TypeFox/monaco-languageclient) and [vscode-ws-jsonrpc](https://github.com/TypeFox/vscode-ws-jsonrpc)
- CodinGame's [monaco-jsonrpc](https://github.com/CodinGame/monaco-jsonrpc)
