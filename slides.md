---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: true
# some information about the slides, markdown enabled
info: |

  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS
css: unocss
---

# slidevで発表を楽にしよう

---

# 本日の流れ

- slidevって何？
- インストールしてみよう（デモ）
- VSCodeの拡張機能をいれてみよう
- スライドを作ってみよう

---

# slidevって何？


- 📝 Markdownベース - お気に入りのエディタとワークフローを使用
- 🧑‍💻 デベロッパーフレンドリー - ビルトインのシンタックスハイライト、ライブコーディングなど
- 🎨 豊富なテーマ - テーマはnpmパッケージで共有・利用が可能
- 🌈 スタイリッシュ - Windi CSS オンデマンドユーティリティ、 使いやすい埋め込まれたスタイルシート
- 🤹 インタラクティブ - Vueコンポーネントをシームレスに埋め込み
- 🎙 プレゼンターモード - 別のウィンドウ、スマートフォンでさえもスライドを操作
- 🎨 描画 - スライドに描画し、注釈をつける
- 🧮 LaTeX - LaTeX数式のビルトインサポート
- 📰 図形 - 説明と合わせて図形を作成
- 🌟 アイコン - どんなアイコンセットからでも、直接アイコンにアクセス
- 💻 エディタ - 統合されたエディタとVS Code拡張機能
- 🎥 レコーディング - ビルトインのレコーディングとカメラビュー
- 📤 ポータブル - PDF、PNG、またはホスト可能なSPAにエクスポート
- 🛠 自由に開発可能 - Viteプラグイン、Vue components、どんなnpmパッケージも使用可能

---

## インストールしてみよう

<br>

```
$ npm init slidev
```

---

## VSCodeの拡張機能をいれてみよう

![slidev_vscode](/slidev_vscode.png)

---

## 日本語ドキュメント

https://ja.sli.dev/guide/

---
layout: center
---

## スライドを作ってみよう

---

# デモ

```go
package main

import "fmt"

func main() {
  fmt.Printf("Hello World\n")
}
```

---

## 複数行の文章

１行目
<br>
２行目
<br>
１行目
２行目にしたい
<br>

- ああああああ
- ああああああ
- ああああああ

```ts
console.log("demo")
```

---

# コードハイライト

```go {5-7}
package main

import "fmt"

func main() {
  fmt.Printf("Hello World\n")
}
```


lineNumbers: true で行数表示。デフォルトfalse
```
---
lineNumbers: true
---
```

---

## 画像表示

<style>
img {
  width: 20%;
}
</style>

画像だよ
![image](/download.png)
<!-- <img src="/download.png" /> -->

---
layout: center
---

##

```
---
layout: center
---
```

<style>
img {
  width: 20%;
}
</style>

スライドごとにレイアウトを変えたい時

<!-- ![image](/download.png) -->
<img src="/download.png" />

---

## Presentation Mode

http://localhost:3030/presenter/

Presentation modeでNotesを表示しよう
<br>
Notesを書いておけば、そのままブログ記事にもしやすい

<!-- ここにNotesが表示されます -->

---

# Twitter埋め込み

<Tweet id="1598420090122379264" :scale="0.5"/>

---

# Youtube埋め込み

<iframe width="560" height="315" src="https://www.youtube.com/embed/_qXG06v8HAI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<br>

```
<iframe width="560" height="315" src="https://www.youtube.com/embed/_qXG06v8HAI"
title="YouTube video player"
frameborder="0" allow="accelerometer;
autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```

---
src: ./common.md
---

---

## 参考資料

<br>

- [Slidevを導入してMarkdownで美しいスライドを書こう - Qiita](https://qiita.com/loftkun/items/2fbeddc9449eb5d85dfd)

- [slidev-example/slides.md at main · loftkun/slidev-example](https://github.com/loftkun/slidev-example/blob/main/slides.md)

---

## 最後に
<br>

### 良いところ
- Markdownでかける
- コードハイライトがいい
- 一度、作るとスライドの使いまわしがしやすい
- テキストなのでバージョン管理しやすい

<br>

### 苦労したところ
- フォントサイズ、レイアウトにこだわりたい
<br>
HTML/CSS/Vueの知識があるとカスタマイズできる

