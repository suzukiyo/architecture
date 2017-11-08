## rebase
`git rebase master`

## rebase conflict
`git rebase --continue `

## merge -> rebase
```
1. merge以降にコミットしたものを別ブランチに退避
2. git reset --hard {ハッシュ番号} でmergeを取り消し
3. git pull --rebase でmergeでなくrebaseにする
4. 退避したものをcherrypickでもってくる
5. git rebase -i HEAD~n
```

## git stash

Confirm: 確認する
`git stash list`

Save: 退避する
`git stash save`

apply: 復活する
`git stash apply`

drop: 削除する
`git stash drop stash@{0}`

POP: 復活＆削除する
`git stash pop`
