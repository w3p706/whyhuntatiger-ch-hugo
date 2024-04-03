# With Github (as of 04-2024)


## Local

```
./bin/act/act --secret-file .secrets
```

Or published with Github actions


## Old:
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


Init CI/CD:
* Create repo für compiled website
* Change submodule URL to `url = ../tiger-photo.git`
* Settings > CI/CD > Variables Set:
    * SSH_KNOWN_HOSTS
    * SSH_PRIVATE_KEY
* In the public website repo add Deploy Keys  "ci-runner-deploy-key" with write access

