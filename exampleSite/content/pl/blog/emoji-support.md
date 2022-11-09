---
author: "Hugo Authors"
title: "Wsparcie emoji"
date: 2021-07-15
description: "Przewodnik w używaniu emoji w Hugo"
tags: ["emoji"]
thumbnail: https://picsum.photos/id/1050/400/250
---

Emoji można dodać do projektu Hugo na wiele sposobów.

<!--more-->


Funkcja [`emojify`](https://gohugo.io/functions/emojify/) może zostać wywołana bezpośrednio w szablonie lub za pomocą [Inline Shortcodes](https://gohugo.io/templates/shortcode-templates/#inline-shortcodes).

Aby włączyć emoji globalnie, ustaw parametr `enableEmoji` na `true` w pliku [konfiguracyjnym](https://gohugo.io/getting-started/configuration/) swojej strony, po czym możesz używać emoji shorthand codes w treści swoich plików; np.

<p><span class="nowrap"><span class="emojify">🙈</span> <code>:see_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙉</span> <code>:hear_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙊</span> <code>:speak_no_evil:</code></span></p>
<br>

[Emoji cheat sheet](http://www.emoji-cheat-sheet.com/) jest przydatnym odnośnikiem dotyczącym emoji shorthand codes.

---

**N.B.** Powyższe kroki umożliwiają zastosowanie standardowych emoji Unicode Standard, ale ich renderowanie może zależeć od przeglądarek internetowych i platform. Aby wystylizować swoje emoji możesz użyć czcionki emoji; np.

{{< highlight html >}}
.emoji {
font-family: Apple Color Emoji, Segoe UI Emoji, NotoColorEmoji, Segoe UI Symbol, Android Emoji, EmojiSymbols;
}
{{< /highlight >}}

{{< css.inline >}}

<style>
.emojify {
	font-family: Apple Color Emoji, Segoe UI Emoji, NotoColorEmoji, Segoe UI Symbol, Android Emoji, EmojiSymbols;
	font-size: 2rem;
	vertical-align: middle;
}
@media screen and (max-width:650px) {
  .nowrap {
    display: block;
    margin: 25px 0;
  }
}
</style>

{{< /css.inline >}}
