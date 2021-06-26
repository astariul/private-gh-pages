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

Then create a branch with only the generated content :

```console
cd ..
cp -r mkdocs_page/site ../site

git checkout --orphan mkdocs_page 
git rm --cached -r .
mv ..\site\* .
git add *
git commit -m ":memo: Add static site content"
git push --set-upstream origin mkdocs_page
```