<!-- markdownlint-disable -->
<br />
<div align="center">
  <a href="https://github.com/mrcjkb/haskell-snippets.nvim">
    <img src="./logo.svg" alt="haskell-snippets.nvim">
  </a>
  <p align="center">
    <a href="https://github.com/mrcjkb/haskell-snippets.nvim/issues">Report Bug</a>
  </p>
  <p>
    <strong>
      My collection of Haskell snippets for <a href="https://github.com/L3MON4D3/LuaSnip">LuaSnip</a>.
      <br />
      Powered by <a href="https://github.com/nvim-treesitter/nvim-treesitter">tree-sitter</a> and LSP.
    </strong>
  </p>
  <h2>🦥</h>
</div>
<!-- markdownlint-restore -->

[![Neovim][neovim-shield]][neovim-url]
[![Lua][lua-shield]][lua-url]
[![Haskell][haskell-shield]][haskell-url]
[![Nix][nix-shield]][nix-url]

[![GPL2 License][license-shield]][license-url]
[![Issues][issues-shield]][issues-url]
[![Build Status][ci-shield]][ci-url]

## Quick Links

- [Installation](#installation)
- [Quick Setup](#quick-setup)
- [Snippets](#snippets)
- [Recommendations](#recommendations)
- [Contributing](./CONTRIBUTING.md)

## Installation

Use luarocks or your favourite plugin manager.

### Required

- `neovim >= 0.8`
- [`luasnip`](https://github.com/L3MON4D3/LuaSnip)

### Optional

- [`haskell-language-server`](https://haskell-language-server.readthedocs.io/en/latest/installation.html)
  and [`haskell-tools.nvim`](https://github.com/mrcjkb/haskell-tools.nvim)
  (some snippets work better with LSP).
- [`nvim-treesitter`](https://github.com/nvim-treesitter/nvim-treesitter)
  and the parser for haskell.

## Quick setup

Add the following to your LuaSnip setup.

```lua
local ls = require('luasnip')
ls.setup {
  -- Add your LuaSnip config
}
local haskell_snippets = require('haskell-snippets').all
ls.add_snippets('haskell', haskell_snippets, { key = 'haskell' })
```

> **Note**
>
> See also `:h haskell-snippets`

## Snippets

> **Note**
>
> The recording software [ttyrec](https://github.com/mjording/ttyrec)
> sometimes has some visual glitches.

### Pragmas

#### `haskell-snippets.pragmas.prag`

- Trigger: `prag`

![tty](https://github.com/mrcjkb/haskell-snippets.nvim/assets/12857160/ced58a75-ce1a-4a74-8d1f-8d715d68d81a)

#### `haskell-snippets.pragmas.lang`

- Trigger: `lang`

![tty](https://github.com/mrcjkb/haskell-snippets.nvim/assets/12857160/18bf238a-ea23-4206-97ab-421a7896bfd2)

#### `haskell-snippets.pragmas.discover`

- Trigger: `discover`

![tty](https://github.com/mrcjkb/haskell-snippets.nvim/assets/12857160/d80c6209-f324-4a1c-ae3c-9e4f1245a113)

#### `haskell-snippets.pragmas.nowarn`

- Trigger: `nowarn`

![tty](https://github.com/mrcjkb/haskell-snippets.nvim/assets/12857160/ba95a3cd-fc68-4adb-9011-82e39ffc742c)

### Module and imports

#### `haskell-snippets.module.mod`

- Trigger: `mod`

![tty](https://github.com/mrcjkb/haskell-snippets.nvim/assets/12857160/ade2cb77-10de-4183-bded-163caf3cc8f7)

#### `haskell-snippets.module.qual`

- Trigger: `qual`

![tty](https://github.com/mrcjkb/haskell-snippets.nvim/assets/12857160/2fbd5f6d-2c8b-4f8c-b1f1-39bc4bd8f549)

### Data and typeclasses

#### `haskell-snippets.data.adt`

- Trigger: `adt`

![tty](https://github.com/mrcjkb/haskell-snippets.nvim/assets/12857160/6a4fbc24-ab83-440a-971b-5d7373f52ce0)

#### `haskell-snippets.data.newtype`

- Trigger: `new`

![tty](https://github.com/mrcjkb/haskell-snippets.nvim/assets/12857160/769459ed-6149-4f84-bd97-60570749938f)

#### `haskell-snippets.data.rec`

- Trigger: `rec`

![tty](https://github.com/mrcjkb/haskell-snippets.nvim/assets/12857160/e633ee97-48ad-462e-949f-8c140f7bd086)

#### `haskell-snippets.data.cls`

- Trigger: `cls`
- [ ] TODO: Add gif

#### `haskell-snippets.data.ins`

- Trigger: `ins`
- [ ] TODO: Add gif

#### `haskell-snippets.data.constraint`

- Trigger: `=>`
- [ ] TODO: Add gif

### Functions

#### `haskell-snippets.functions.fun`

- Trigger: `fun`
- [ ] TODO: Add gif

#### `haskell-snippets.functions.func`

- Trigger: `func`
- [ ] TODO: Add gif

#### `haskell-snippets.functions.lambda`

- Trigger: `\`
- [ ] TODO: Add gif

### Expressions

#### `haskell-snippets.expressions.if_expr`

- Trigger: `if`
- [ ] TODO: Add gif

#### `haskell-snippets.expressions.if_expr_multiline`

- Trigger: `iff`
- [ ] TODO: Add gif

#### `haskell-snippets.expressions.case`

- Trigger: `case`
- [ ] TODO: Add gif

#### `haskell-snippets.expressions.lambdacase`

- Trigger: `\case`
- [ ] TODO: Add gif

### QuasiQuotes

#### `haskell-snippets.quasiquotes.qq`

- Trigger: `qq`
- [ ] TODO: Add gif

#### `haskell-snippets.quasiquotes.sql`

- Trigger: `sql`
- [ ] TODO: Add gif

## Contributing

All contributions are welcome!
See [CONTRIBUTING.md](./CONTRIBUTING.md).

## Recommendations

Here are some other plugins I recommend for Haskell development:

- [mrcjkb/haskell-tools.nvim](https://github.com/mrcjkb/haskell-tools.nvim):
  Toolset to improve the Haskell experience in Neovim.
- [luc-tielen/telescope_hoogle](https://github.com/luc-tielen/telescope_hoogle):
  Hoogle search.

<!-- MARKDOWN LNIKS & IMAGES -->
[neovim-shield]: https://img.shields.io/badge/NeoVim-%2357A143.svg?&style=for-the-badge&logo=neovim&logoColor=white
[neovim-url]: https://neovim.io/
[lua-shield]: https://img.shields.io/badge/lua-%232C2D72.svg?style=for-the-badge&logo=lua&logoColor=white
[lua-url]: https://www.lua.org/
[nix-shield]: https://img.shields.io/badge/nix-0175C2?style=for-the-badge&logo=NixOS&logoColor=white
[nix-url]: https://nixos.org/
[haskell-shield]: https://img.shields.io/badge/Haskell-5e5086?style=for-the-badge&logo=haskell&logoColor=white
[haskell-url]: https://www.haskell.org/
[issues-shield]: https://img.shields.io/github/issues/mrcjkb/haskell-snippets.nvim.svg?style=for-the-badge
[issues-url]: https://github.com/mrcjkb/haskell-snippets.nvim/issues
[license-shield]: https://img.shields.io/github/license/mrcjkb/haskell-snippets.nvim.svg?style=for-the-badge
[license-url]: https://github.com/mrcjkb/haskell-snippets.nvim/blob/master/LICENSE
[ci-shield]: https://img.shields.io/github/actions/workflow/status/mrcjkb/haskell-snippets.nvim/nix-build.yml?style=for-the-badge
[ci-url]: https://github.com/mrcjkb/haskell-snippets.nvim/actions/workflows/nix-build.yml
