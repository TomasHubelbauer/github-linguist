# GitHub MarkDown Savant

GitHub uses Linguist, a "language savant" library for detecting languages in a repository
and rendering the language bar on the repository GitHub page.

I have a lot of MarkDown-only repositories which serve as reference for me and I don't like
how in repository lists and on the repository page they show no language bar.

It seems that may be possible to fix using `.gitattributes`:

https://github.com/github/linguist#documentation

```ini
README.md linguist-documentation=false
```

Does this repo have a language bar? No? Then it didn't work. It does? Awesome.

- [ ] Find out (low priority background process, might take a while)
