# GitHub Linguist

[**WEB**](https://tomashubelbauer.github.io/github-linguist)

GitHub uses Linguist, a "language savant" library for detecting languages in a repository
and rendering the language statistics bar on the repository page.

## Marking for inclusion

I have a lot of MarkDown-only repositories which serve as reference for me and I don't like
how in repository lists and in the repository page they show no language bar.

This is possible to fix using `.gitattributes`:

https://github.com/github/linguist#documentation

```ini
*.md linguist-documentation=false linguist-detectable=true
```

## Marking for exclusion

Sometimes the repository may include source code of dependencies or tools which are not to
be treated as the source code of the repository itself.

```ini
tool/* linguist-vendored
```

## To-Do
