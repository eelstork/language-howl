# Howl notation support in Atom

Howl is the symbolic notation for C# programming. This package provides input support and syntax highligting for Howl in Atom.

## Prerequisite

Via node-gyp, this package requires Python and a native C++ toolchain. You may visit the [node-gyp](https://github.com/nodejs/node-gyp) homepage for details but, in short:

- On Windows, Visual Studio community edition (tried 2019, works) with C++ desktop dev workload. Alternatives yet perhaps this is the easy way.
- GCC on Linux
- XCode plus `xcode-select --install` in terminal for command line tools.

If you are not able to install the package, please open an issue.

## Making yourself at ease

- Hiding metafiles and other nonsense may be a good idea.
Here is a [config template] [ADD] you may use.
- Select 'hide ignored names' in the tree-view package (`Atom > [Settings or prefs] > Packages > Tree-view`).

## For developers

The package may be cloned to `~/.atom/packages`

After updating the grammar and up to npm, update `tree-sitter-howl` version in `package.json` then:

```bash
cd ~/.atom/packages/language-howl
apm install
```

Use `⌘ + SHIFT + P` and `rel` to reload the package.

When all good commit and `apm publish [major/minor/patch]`
