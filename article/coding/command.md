# ステップ数

## 複数

```sh
find . -name '*.java' -type f | xargs grep -Ev '^[[:space:]]*((/?\*.*/?)|(//.*))$' | wc -l
```

## 単一

```sh
grep -Ev '^[[:space:]]*((/?\*.*/?)|(//.*))$' hoge.txt | wc -l
```
