---
theme: gaia
marp: true
math: mathjax
size: 16:9
paginate: true
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.svg')
header: headerテキスト
footer: footerテキスト
---

<!-- _class: lead -->
<!-- _footer: "" -->

<!-- ↑のような "Directives" 構文の詳細は https://marpit.marp.app/directives を参照 -->

<style>
    <!-- 以降のページ全体に影響するスタイル変更のCSSは style ～ /style 内に書く -->
</style>

<style scoped>
    <!-- そのページのみに影響するスタイル変更のCSSは style scoped ～ /style 内に書く -->
</style>

![bg right:50% 80%](https://marp.app/assets/marp.svg)

# Marpサンプル

副題文字列

著者名など

---

# 見出し1
## 見出し2
### 見出し3

[CommonMarkの文法](https://commonmark.org/help/)がベースになっている

```markdown
# 見出し1
## 見出し2
### 見出し3

[CommonMarkの文法](https://commonmark.org/help/)がベースになっている
```

---

## 段落

1段落目1行目
1段落目2行目

2段落目1行目

```markdown
1段落目1行目
1段落目2行目

2段落目1行目
```

---

## 改ページ

```markdown
# 表紙

横罫線(`---`)でページを分割できます。

---
## 2頁目

2ページ目の内容

---
## 3頁目

...
```

---

## 箇条書き

* 箇条書き1
* 箇条書き2
* 箇条書き3

```markdown
* 箇条書き1
* 箇条書き2
* 箇条書き3
```

---

## 装飾

**太字** ~~取消線~~ <u>下線</u> <ruby>ルビ文字<rp>(</rp><rt>ruby string</rt><rp>)</rp></ruby>

```markdown
**太字** ~~取消線~~ <u>下線</u> <ruby>ルビ文字<rp>(</rp><rt>ruby string</rt><rp>)</rp></ruby>
```

---

## リンク・引用

> Based on CommonMark
> If you know how to write document with Markdown, you already know how to write a Marp slide deck.
> Marp's format is based on [CommonMark](https://commonmark.org/), a consistent Markdown specification.
> The only important difference is [a ruler --- for splitting pages](https://marpit.marp.app/markdown).

```markdown
> Based on CommonMark
> If you know how to write document with Markdown, you already know how to write a Marp slide deck.
> Marp's format is based on [CommonMark](https://commonmark.org/), a consistent Markdown specification.
> The only important difference is [a ruler --- for splitting pages](https://marpit.marp.app/markdown).
```

---

## コード

インラインのコード `print('Hello World')` と、文法ハイライト付きコードブロック

```python
print('Hello World')
```

~~~markdown
インラインのコード `print('Hello World')` と、文法ハイライト付きコードブロック

```python
print('Hello World')
```
~~~

---

## テーブル

|左寄せ見出し|中央寄せ見出し|右寄せ見出し|
|:--|:-:|--:|
|左|中央|右|
|左|中央|右|

```markdown
|左寄せ見出し|中央寄せ見出し|右寄せ見出し|
|:--|:-:|--:|
|左|中央|右|
|左|中央|右|
```

---

## 数式

文章中に挿入する $e=mc^2$ のようなインライン数式や、

$$B(x;a,b)=\int_0^xt^{a-1}(1-t)^{b-1}dt.$$

のようなブロック数式がある。

```markdown
文章の中に挿入する $e=mc^2$ のようなインライン数式や、

$$B(x;a,b)=\int_0^xt^{a-1}(1-t)^{b-1}dt.$$

のようなブロック数式がある。
```

---

## 画像

詳細は https://marpit.marp.app/image-syntax を参照

```markdown
* 画像を挿入
![](image.jpg)
* 画像の大きさを指定
![width:200px](image.jpeg)
![height:30cm](image.jpeg)
![w:32 h:32](image.jpeg)
* 背景画像を挿入
![bg](https://example.com/background.jpg)
* 背景画像を挿入(スライドサイズに合わせる)
![bg contain](https://example.com/background.jpg)
```

---

### 背景画像を右寄せにする

![bg right:40%](https://picsum.photos/720?image=3)

```markdown
![bg right:40%](https://picsum.photos/720?image=3)
```

---

### 横方向への分割

![bg](https://fakeimg.pl/800x450/012133/fff/?text=A)
![bg](https://fakeimg.pl/800x450/02314c/fff/?text=B)
![bg](https://fakeimg.pl/800x450/2e5366/fff/?text=C)

```markdown
![bg](https://fakeimg.pl/800x450/012133/fff/?text=A)
![bg](https://fakeimg.pl/800x450/02314c/fff/?text=B)
![bg](https://fakeimg.pl/800x450/2e5366/fff/?text=C)
```

---

### 縦方向への分割＋右寄せ

![bg right:20% vertical](https://fakeimg.pl/800x450/012133/fff/?text=A)
![bg](https://fakeimg.pl/800x450/02314c/fff/?text=B)
![bg](https://fakeimg.pl/800x450/2e5366/fff/?text=C)

```markdown
![bg right:20% vertical](https://fakeimg.pl/800x450/012133/fff/?text=A)
![bg](https://fakeimg.pl/800x450/02314c/fff/?text=B)
![bg](https://fakeimg.pl/800x450/2e5366/fff/?text=C)
```

---

## 絵文字

DiscordやSlackなどで使える絵文字の一部を `:alias_name:` のようにコロン文字で挟んだエイリアス名で使える
https://www.webfx.com/tools/emoji-cheat-sheet/

* :thinking: :zany_face: :thumbsup: :ok_hand: :pray: :poop: :see_no_evil: :hear_no_evil: :speak_no_evil:
* :heart: :fire: :boom: :money_with_wings: :exclamation: :end: :calling: :shield: :secret:

```markdown
* :thinking: :zany_face: :thumbsup: :ok_hand: :pray: :poop: :see_no_evil: :hear_no_evil: :speak_no_evil:
* :heart: :fire: :boom: :money_with_wings: :exclamation: :end: :calling: :shield: :secret:
```

