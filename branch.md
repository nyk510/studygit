# 追跡しているブランチを知りたい

`git branch -vv`でブランチの詳細を確認できます。

```bash
nyker-goto@nykergoto-HPE-560jp:~/pydocs/practice_A$ git branch -vv
master      49bcb3e [origin/master] Change tutrial name make a new branch and push a remote repositry tutrial
* nykerbranch e7b7880 Add: nyker510_memo folder
```

['origin/~~']に書いてあるのが現在追跡しているリモートブランチ。この場合だとmasterは追跡しているブランチがあるけれど、nykerbranchは追跡してるブランチがない。
