```
code .
git init
git add README.md
git add index.js
git add .tool-versions
git commit -m "first commit"
```
- Create repo on github: grebase
```
git remote add origin git@github.com:StefanWallin/grebase.git
git push -u origin main
open https://github.com/StefanWallin/grebase
```

```
git checkout -b emoji
```

**Edit 1: (emoji)**
```
console.log("Violets are 🔴,")
console.log("Roses are 🔵,")
```

```
git add -p
git commit -m "Use emojis for colors"
git push -u origin emoji
```
- Make PR
- Do not merge PR

```
git checkout main
```

**Edit 2: (main), on github**
```
console.log("Roses are red,")
console.log("Violets are blue,")
```

```
git add -p
git commit -m "Correct the poem"
git push
```

- open PR again - see conflict ("resolve conflict"-button)

```
git pull
git checkout emoji
git rebase -i main
  talk about the file
  talk about EDITOR
  pick
  :wq
```
- `git status`
- `git status -sb`
- Source tree
- **Edit 3: (emoji)**
- Resolve conflict
- Save file
- `git add index.js`
- `git rebase --continue`
