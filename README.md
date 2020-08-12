# Howl notation support in Atom

Howl is the symbolic notation for C# programming. This package provides input support and syntax highligting for Howl in Atom.

## Prerequisites

Windows [DOCUMENT]
macOS Mojave [DOCUMENT]
macOS Catalina [DOCUMENT]

## Making yourself at ease

If you are using Unity 3D, hiding metafiles and other nonsense may be a good idea.
Here is a [config template] [ADD] you may use.

Ensure you have selected 'hide ignored names' in the tree-view package (`Atom > [Settings or prefs] > Packages > Tree-view`).

## For developers

The package may be cloned to `~/.atom/packages`

After updating the grammar and up to npm, update `tree-sitter-howl` version in `package.json` then:

```bash
cd ~/.atom/packages/language-howl
apm install
```

Use `⌘ + SHIFT + P` and `rel` to reload the package.

When all good commit and `apm publish [major/minor/patch]`
