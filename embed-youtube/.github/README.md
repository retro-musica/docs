> ⚠️ **この説明内容は編集しないで下さい**
> <br>
> 編集者: 野中
# YouTube の埋め込み
YouTube をマークダウンファイルに埋め込むことはできません。リンクを貼ったり、画像に動画のリンクを貼ったりすることはできます。
<br>
それでもいい場合はそうして下さい。ここではマークダウンファイルを一旦 HTML ファイルに変換して、そこに YouTube を埋め込む方法を考えます。

---
YouTube などの動画を HTML ファイルに埋め込むのには、`iframe` タグをよく使います↓↓

```html
<iframe
        width="880"
        height="495"
        src="https://www.youtube-nocookie.com/embed/xdcSFVXd3MU"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen>
</iframe>
```
`test.md` というファイルを作りました。これを [markdowntohtml.com](https://markdowntohtml.com/) というウェブサイトで HTML ファイルに変換します。その結果が
<br>
`test.html` というファイルです。これに手を加えて `embed.html` というファイルにして、これを `index.html` として該当ディレクトリの
<br>
中に配置すれば完了です。比較: [test.html](https://retro-ongaku.github.io/docs/embed-youtube/test.html) → [embed.html](https://retro-ongaku.github.io/docs/embed-youtube/embed.html)
<br>
少し面倒臭いですが頑張って!! それから埋め込みを中央寄せしたいところですが、CSS も学習する必要が出てくるのでここでは割愛
<br>
(音楽サークルがウェブサイト作りをガチっても仕方ないですよね)
