---
title: Emoji Support
date: 2026-03-19
author: JenkinsAbuser
description: Guia de uso de emojis en Hugo
isStarred: true
draft: false

--- 

Los emojis pueden habilitarse en un proyecto de Hugo de varias maneras.

<!--more--> 

La función [`emojify`](https://gohugo.io/functions/emojify/) se puede llamar directamente en las plantillas o en [Inline Shortcodes](https://gohugo.io/templates/shortcode-templates/#inline-shortcodes). 

Para habilitar los emojis globalmente, establezca `enableEmoji` en `true` en el `hugo.toml` de su sitio. Puede escribir códigos abreviados de emoji directamente en los archivos de contenido; por ejemplo.

`:see_no_evil:` :see_no_evil: `:hear_no_evil:` :hear_no_evil: `:speak_no_evil:` :speak_no_evil:

¡Me encanta Hugo! 😁

La [Emoji cheat sheet](http://www.emoji-cheat-sheet.com/) es una referencia útil para los códigos abreviados de emoji.

***

**N.B.** Los pasos anteriores habilitan los caracteres y secuencias de emoji del estándar Unicode en Hugo, sin embargo, la representación de estos glifos depende del navegador y de la plataforma. Para estilizar los emojis, puede utilizar una fuente de emojis de terceros o una pila de fuentes; por ejemplo.

{{< highlight css >}}
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
