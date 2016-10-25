# Step by step

Initialize git flow
```
git flow init
```

Finish feature myapi
```
git checkout feature/myapi
git flow feature finish myapi
```

Finish feature home-list
```
git checkout feature/home-list
git flow feature finish home-list
```

Finish feature home-newsletter
```
git checkout feature/home-newsletter
git flow feature finish home-newsletter
```

Rename branch release to release/0.2.0
```
git branch -m release/0.2.0
git branch -a
git push origin :release
git push origin release/0.2.0
```

Finish release 0.2.0
```
git flow release finish 0.2.0
```

Delete hotfix commit and create real hotfix
```
git checkout master
git push origin +8b85867:master
git checkout 8240c47
git checkout -b hotfix/0.2.1
git flow hotfix finish 0.2.1
```
