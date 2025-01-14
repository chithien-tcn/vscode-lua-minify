# Lua Minify

This extension helps you to minify on-the-fly any Lua source file.

![Version](https://vsmarketplacebadge.apphb.com/version-short/informagico.vscode-lua-minify.svg)
![Installs](https://vsmarketplacebadge.apphb.com/installs/informagico.vscode-lua-minify.svg)
![Rating](https://vsmarketplacebadge.apphb.com/rating-star/informagico.vscode-lua-minify.svg)

## Feature

- [x] Minify the whole file
- [x] Minify selected code
- [x] Generate minified .min.lua file

## Usage

Use the command *`Lua Minify: Minify`* to process current open file

![vscode-lua-minify](https://github.com/informagico/vscode-lua-minify/blob/master/images/vscode-lua-minify.gif?raw=true)

Use the command *`Lua Minify: Minify Selection`* to process current selection

Use the command *`Lua Minify: Generate .min file`* to process current open file and create a minified separate version

## Settings

From `0.7.0` new settings has been added to support multiple functionalities.

- `flavour`: Identify which package is going to be used to minify the code. Possible values: "luamin" (default), "lua-format" [`lua-format` supports Luau]
- `renameVariables`: Available only if 'lua-format' is selected. Defines if the variables should be renamed
- `renameGlobals`: Available only if 'lua-format' is selected. Defines if the globals should be renamed
- `solveMath`: Available only if 'lua-format' is selected. Defines if the math should be solved

Here an example of `settings.json` file:

```json
"vscode-lua-minify": {
  "flavour": "lua-format",
  "renameVariables": false,
  "renameGlobals": false,
  "solveMath": false,
}
```

## Contributions

Feel free to contribute improving this extension and [let me know](https://github.com/informagico/vscode-lua-minify/issues) if you find a bug.

---

### Thanks

A huge thanks to Mathias Bynens ([@mathiasbynens](https://github.com/mathiasbynens)) for building up [luamin](https://github.com/mathiasbynens/luamin) that I used as core for this extension.
A huge thanks also to Herrtt ([@Herrtt](https://github.com/Herrtt)) for building up [lua-format](https://github.com/Herrtt/luamin.js) that I used as core for this extension.
