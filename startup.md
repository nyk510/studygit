
# このファイルについて
Jupyer上でmarkdownを書く上でやっておいたら便利なことをまとめます。

# 覚えておくと便利な事
## コマンド
`esc`を押すことでコマンドモードになります.
(コマンドモードかどうかは右上に鉛筆アイコンが出ているかどうかで判断できます

* `h`:コマンドのヘルプを表示します。だいたいここ見ればいける。

ちなみにヘルプを見ながらでも背景でコマンドは実行されるので、最初はヘルプを見ながら実験するのがいいと思う。  
以下は大事なコマンド

1. `x`:cut-cell セルの切り取り
2. `z`:セルの状態をundo
1. `V`:切り取ったセルを貼り付け。`shift+V`で選択セルの上に貼り付ける
2. `a`,`b`:insert-new-cell above(a) or below(b) (選択されているセルの上下に新しいセルを挿入）
3. `d + d`:delete-cell. Dを二回押す。
1. `Enter`: Cellの編集モードに入る
1. `M`: Cellをmarkdownにする
1. `Y`: Cellをcodeモードにする

# 便利な道具たち

## Markdonwの書き方
Markdownはイージーにhtmlを書ける記法のことだと思ってだいたい合ってると思います。  
コマンド等をまとめてくれているサイトを参照しておきます。

>Markdonw-CheatSheet:  
>https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
>
>Markdown: Syntax
>http://daringfireball.net/projects/markdown/syntax.php

参照先を見なくても、このDocumentをEnterして中身を見ればだいたいわかると思います。

数式もlatexでかけるので、行内に $\sin(x),\int_{-1}^1 \tanh(x)$ とか

$$
\begin{align}
S_n &= \sum_{n=1}^{N} n^2 \\
    &= \frac{1}{6} n(n+1)(2n+1)
\end{align}
$$

なんてことも出来ます。かっこいいね。

## マークアップ（css）の設定変更

最初の状態だと、h1,h2タグあたりが見にくくてしょうがないので色と大きさを変えるといいかもしれません。
変更のためにはcostom.cssをいじります。

参考：http://stackoverflow.com/questions/32156248/how-do-i-set-custom-css-for-my-ipython-ihaskell-jupyter-notebook
>I think the path to your custom.css should be:
```
~/.ipython/profile_default/static/custom/custom.css
```
>custom folder instead of css folder.

### 注意
Jupyterを使ってる時は、costom.cssの場所が違います。
/.ipythonではなく、/.jupyter以下にあるcostomフォルダ内のcssを変更しないと駄目。

例：僕が今使ってるcostom.cssの設定
```css
/*
Placeholder for custom user CSS

mainly to be overridden in profile/static/custom/custom.css

This will always be an empty file in IPython
*/
.CodeMirror{
  font-family: Consolas,meiryo;
}
.cm-s-default .cm-header{
    color: #45495D;
}
.cm-header {
    color: #45495D;
    line-height:130%;
}
.cm-header-1 {
    font-size: 120%;
}
.cm-header-2 {
    font-size: 120%;
}
.cm-header-3 {
    font-size: 120%;
}
.cm-header-4 {
    font-size: 120%;
}
.cm-header-1, .cm-header-2, .cm-header-3, .cm-header-4, .cm-header-5, .cm-header-6 {
    font-weight: bold;
    font-family: Arial,meiryo;
}
.rendered_html code{
    font-family:Consolas;
    padding: 2px 4px;
    font-size: 90%;
    color: #c7254e;
    background-color: #f9f2f4;
    border-radius: 2px;
}
.rendered_html pre {
    display: block;
    padding: 8.5px;
    font-size: 12px;
    line-height: 1.42857143;
    word-break: break-all;
    word-wrap: break-word;
    color: #333333;
    background-color: #f5f5f5;
    border: 1px solid #cccccc;
    border-radius: 2px;
}
.rendered_html pre > code {
  color: #333;
  font-size: 100%;
  padding: 0;
  background-color: transparent;
}
```
## markdown形式での保存
File>Download as>.mdで保存を選択

# やりたいこと
情報共有をみんなで簡単にできるようになりたい。
せっかく勉強するのなら、後で見返したり、コメント残したり、あとアルゴリズムの説明とかするときは数式も使いたい


```python

```
