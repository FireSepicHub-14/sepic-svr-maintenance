# Screen
> screenとは

consoleを分割できるやつです。(仮想端末を作成できる)<br>
なんか、コンテナみたいにできる..(語彙力の無さ)<br>
このドキュメントではよく使う操作のみの記述とし、詳細はほかの閲覧をお勧めする。
<br>
> 見出し
- [コマンド系](#コマンド系)
    - [よく使う引数チートシート](#よく使う引数チートシート)
    - [Screenの立ち上げと確認](#screenの立ち上げと確認)
    - [セッションのアタッチ](#セッションのアタッチ)
    - [セッションの強制アタッチと終了](#セッションの強制アタッチと終了)
        - [強制アタッチ](#強制アタッチ--下記の状況だと)
        - [強制終了](#強制終了)

- [ショートカットキー](#ショートカットキー)
- [個人的な優良なサイト](#個人的な優良なサイト)

<br>
<br><br>

## コマンド系
> #### よく使う引数チートシート

|引数|結果|
|----|----|
| -S xxx | xxxという名前の新しいセッションの立ち上げ(おすすめ)|
| -r xxx | xxxというセッションにアタッチ(入る)する|
| -X     | セッションに特定のコマンドを送る(後述)|
| -ls    | 今立ち上がっているセッションの一覧表示|

<br><br>


> #### Screenの立ち上げと確認
```
$ screen -S tmp1    // tmp1というセッションの立ち上げ 
$ screen -S tmp2
$ screen -ls        // -lsはディレクトリの検索と同じ
There are screens on:
    34806.tmp1	(Detached)
    34046.tmp2	(Detached)
```
<br><br>

> #### セッションのアタッチ
```
$ screen -S tmp1
$ screen -S tmp2
$ screen -ls
There are screens on:
    34806.tmp1	(Detached)
    34046.tmp2	(Detached)

$ screen -r tmp1                // tmp1にアタッチ
$ screen -ls
There are screens on:
    34806.tmp1	(Attached)      // 今ここにアタッチ中。デタッチは後述
    34046.tmp2	(Detached)
```
<br><br>


> #### セッションの強制アタッチと終了

screenを使って作業しているとたまにおかしくなる。<br>
どこからもアタッチしていないのに、アタッチ状態で入れなかったり、終了できなかったりすることがある。そんなときのためのドキュメントだ。

<br>

> ##### 強制アタッチ | 下記の状況だと
```
$ screen -ls
There are screens on:
    34806.tmp1	(Attached)      // どこかでアタッチ中。イミフ
    34046.tmp2	(Detached)

$ screen -d -r 34806            // 34806というのがtmp1のPIDとなる。
```
<br>

> ##### 強制終了
```
$ screen -ls
There are screens on:
    34806.tmp1	(Attached)      // このどうしようもないのをKillする
    34046.tmp2	(Detached)

$ screen -S tmp1 -X quit        // tmp1セッションをKill

$ screen -ls
There are screens on:
    34046.tmp2	(Detached)
```
<br><br><br>

## ショートカットキー
|キー|結果|
|-----|-----|
|ctrl+a d|アタッチ状態でctrl+aのちdを押下することでデタッチが可能|
|ctrl+a ?|ヘルプが見れる|
|ctrl+a [|コピーモード。バッファーの範囲内ならさかのぼれ、enterで元に戻れる。|

<br><br><br>

## 個人的な優良なサイト
[screenのコマンドの備忘録](https://qiita.com/mgoldchild/items/e336618487eb7d90f6d4) | Qiita<br>
[screenコマンドチートシート](https://qiita.com/mishiwata1015/items/0e26127cd1e774b2989a) | Qiita<br>
[_J Blog / セッション強制終了](https://jimsei.hatenablog.com/entry/20111022/1319286614) | HatenaBlog<br>
[screen - コマンド (プログラム) の説明 - Linux コマンド集 一覧表](https://kazmax.zpp.jp/cmd/s/screen.1.html) | kazmax
<br><br><br>

最終変更日: `2025/06/28 1820`<br>
最終変更者: `@FireSepicHub-14(@sou)`