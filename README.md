# Howl notation support in Atom

Howl is a symbolic notation for the C# programming language 〜

```
‒ ㅇ Encloses(Rep ⧕) → ⦿.b❙ ☰ ⧕.b❙ ? ✗ : ⦿.b.∋(⧕.b);
```

C# equiv:

```cs
public bool Encloses(Rep that)
    => this.b.Length == that.b.Length ? false
    : this.b.Contains(that.b);
```

This package provides:

- A set of snippets; C# in, Howl out. For example typing `public partial class` outputs `‒ᴾ ○`
- Syntax highlighting

## Development notes

For development this can be cloned to `~/.atom/packages`

After updating the grammar and up to npm, update `tree-sitter-howl` version in `package.json` then:

```bash
cd ~/.atom/packages/language-howl
apm install
```

Use `⌘ + SHIFT + P` and `rel` to reload the package.

When all good `apm publish [major/minor/patch]` (automatically pushes)
