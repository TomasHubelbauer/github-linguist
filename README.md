# GitHub Linguist MarkDown

GitHub uses Linguist, a "language savant" library for detecting languages in a repository
and rendering the language bar on the repository GitHub page.

I have a lot of MarkDown-only repositories which serve as reference for me and I don't like
how in repository lists and in the repository page they show no language bar.

This is possible to fix using `.gitattributes`:

https://github.com/github/linguist#documentation

```ini
*.md linguist-documentation=false linguist-detectable=true
```
