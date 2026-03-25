---
title: Guía de Sintaxis Markdown
date: 2026-03-19
author: JenkinsAbuser
description: Artículo de ejemplo que muestra la sintaxis básica de Markdown y el formato para elementos HTML.
isStarred: true
---

Este artículo ofrece un ejemplo de la sintaxis básica de Markdown que puede utilizarse en archivos de contenido de Hugo; además, muestra si los elementos HTML básicos están decorados con CSS en un tema de Hugo.
<!--more-->

## Encabezados

Los siguientes elementos HTML `<h1>`—`<h6>` representan seis niveles de encabezados de sección. `<h1>` es el nivel más alto mientras que `<h6>` es el más bajo.

# H1

## H2

### H3

#### H4

##### H5

###### H6

## Párrafo

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

¿Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## Imagen

Puedes usar la siguiente sintaxis para incluir una imagen. La ruta de la imagen debe ser relativa al archivo `index.md`.

```markdown
![Paisaje](1.jpg)
```

![Paisaje](1.jpg)

You can also include image from external sources.

```markdown
![Imagen](https://source.unsplash.com/random/600x400/?tech)
```

![Imagen](https://source.unsplash.com/random/600x400/?tech)
## Blockquotes

El elemento blockquote representa contenido que se cita de otra fuente, opcionalmente con una referencia que debe estar dentro de un elemento footer o cite, y opcionalmente con cambios en línea como anotaciones y abreviaturas.

### Cita en bloque sin atribución

Puedes usar sintaxis Markdown dentro de una cita en bloque, como **bold**,  _italics_, [enlaces](https://gohugo.io/), `codigo`.

Cita en bloque con atribución

No te comuniques compartiendo memoria, comparte memoria comunicándote.<br>
— <cite>Rob Pike</cite>


Tablas

Las tablas no forman parte de la especificación principal de Markdown, pero Hugo las admite de forma nativa.

   Nombre | Edad
--------|------
    Bob | 27
  Alice | 23

### Markdown dentro de tablas

| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |

## Bloques de código

### Bloque de código con backticks

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Documento HTML5 de ejemplo</title>
</head>
<body>
  <p>Prueba</p>
</body>
</html>
```

### Bloque de código con sangría de cuatro espacios

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

### Bloque de código con el shortcode interno de resaltado de Hugo

{{< highlight html >}}
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Documento HTML5 de ejemplo</title>
</head>
<body>
  <p>Prueba</p>
</body>
</html>
{{< /highlight >}}

### Código en línea

Usa la comilla invertida para referirte a una `variable` dentro de una frase.

