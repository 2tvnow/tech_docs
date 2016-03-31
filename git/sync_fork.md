同步Fork的專案
--------------

(1) remote加入fork專案的repo url，慣例是使用`upstream`這個名字 (第一次才需要)

```
git remote add upstream <fork_repo_url>
```

(2) fetch fork repo的最新支線變化

```
git fecth upstream
```

(3) rebase fork 專案的內容到目前branch，這邊假設使用develop branch

```
git checkout develop
git rebase upstream/develop
```

參考
- [Github - Syncing a fork](https://help.github.com/articles/syncing-a-fork/)
