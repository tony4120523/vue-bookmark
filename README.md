### deploy github pages
```
npm run build
```
commit dist on branch master, git subtree push
```
git subtree push --prefix dist origin gh-pages
```