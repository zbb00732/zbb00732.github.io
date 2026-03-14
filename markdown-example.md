# Markdownサンプル

## 見出し

```markdown
# レベル1
## レベル2
### レベル3
#### レベル4
##### レベル5
###### レベル6
```
# レベル1
## レベル2
### レベル3
#### レベル4
##### レベル5
###### レベル6

---

## 強調

```markdown
**太字**

__太字__

*斜体*

_斜体_

***太字斜体***

___太字斜体___

~~~打ち消し線~~~

<ins>挿入文</ins>

<sup>上付き</sup>文字

<sub>下付き</sub>文字
```

**太字**

__太字__

*斜体*

_斜体_

***太字斜体***

___太字斜体___

~~打ち消し線~~

<ins>挿入文</ins>

<sup>上付き</sup>文字

<sub>下付き</sub>文字

## 文章の引用

```markdown
> 引用文の段落
>
> 引用文の段落

> 引用文
> > 引用文の引用文
> > > 引用文の引用文の引用文
```

> 引用文の段落
>
> 引用文の段落

> 引用文
> > 引用文の引用文
> > > 引用文の引用文の引用文

## コードのインライン引用

```markdown
文章内でコマンドをインライン引用する場合は`git status`のようにする。
```

文章内でコマンドをインライン引用する場合は`git status`のようにする。

## コードのブロック引用

コードのブロック引用をコードのブロック引用で表現するのは上手くいかなさそうなので、文章で説明する。

「\`\`\`」というバッククォートで囲むとコードのブロック引用になる。

\`\`\`  
\# レベル1見出し  
\## レベル2見出し  
\### レベル3見出し  
\`\`\`

開始バッククォート直後にコード種別を記述するとシンタックスハイライトが有効になるかもしれない（対応状況による）

\`\`\`markdown  
\# レベル1見出し  
\## レベル2見出し  
\### レベル3見出し  
\`\`\`

## 色

インライン引用で色指定するとサンプルカラーも表示される。

色  | 書式      | サンプル
--- | --------- | ---
HEX | `#RRGGBB` | `#0969DA`
RGB | `rgb(R,G,B)` | `rgb(9, 105, 218)`
HSL | `hsl(H,S,L)` | `hsl(212, 92%, 45%)`

## リンク

別ドメインの完全URLの他、GitHubの相対リンクや、ページ内アンカーも設定できる。

```markdown
[example.com](https://example.com)

[コードのブロック引用](#コードのブロック引用)
```

[example.com](https://example.com)

[コードのブロック引用](#コードのブロック引用)

ページ内アンカーは`#見出し文字列`という形式で指定する。空白文字は`-`に置き換えられ、それ以外の記号（アポストロフィや感嘆符、疑問符など）は取り除かれる。

```markdown
# This'll be a _Helpful_ Section About the Greek Letter Θ!

[This'll be a _Helpful_ Section About the Greek Letter Θ!](#thisll-be-a-helpful-section-about-the-greek-letter-Θ)
```

## リスト

```markdown
1. First list item
   - First nested list item
     - Second nested list item
```

1. First list item
   - First nested list item
     - Second nested list item

順序ありリストも順序なしリストも、ネストするなら文字列の開始位置までインデントするのが無難。

```markdown
100. First list item
     - First nested list item
       - Second nested list item
```

## 注釈

```markdown
Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

[^1]: My reference.
[^2]: To add line breaks within a footnote, add 2 spaces to the end of a line.  
This is a second line.
```

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

[^1]: My reference.
[^2]: To add line breaks within a footnote, add 2 spaces to the end of a line.  
This is a second line.

## アラート

```markdown
> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.
```

> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.
