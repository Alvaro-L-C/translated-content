---
title: Document.images
slug: Web/API/Document/images
---
{{ ApiRef("DOM") }}

## Summary

`document.images` retorna uma coleção de [imagens](/pt-BR/docs/DOM/Image) do documento HTML.

## Sintaxe

```
var htmlCollection = document.images;
```

## Exemplo

```js
var ilist = document.images;

for(var i = 0; i < ilist.length; i++) {
    if(ilist[i].src == "banner.gif") {
        // found the banner
    }
}
```

## Notas

`document.images.length` – propriedade, retorna o número de imagens na página.

`document.images` é parte do DOM HTML, e só trabalho com documentos HTML.

## Especificação

- [DOM Level 2 HTML: HTMLDocument.images](http://www.w3.org/TR/DOM-Level-2-HTML/html.html#ID-90379117)
