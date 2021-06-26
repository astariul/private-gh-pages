Install mkdocs with :

```console
pip install mkdocs
```

---

Build the static page with (from this folder) :

```console
mkdocs build
```

---

Then create a branch with only the generated content (from the parent folder) :

```console
cp -r site ../../site

```