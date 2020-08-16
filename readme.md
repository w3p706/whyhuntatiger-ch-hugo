

```
./bin/hugo new site businger.best
cd businger.best
git init
git submodule add https://github.com/themefisher/vex-hugo.git themes/vex-hugo
git remote add origin git@gitlab.com:w3p706/businger.best.git
git add .
git commit -m "Initial commit"
git push -u origin master
./bin/hugo serve
```