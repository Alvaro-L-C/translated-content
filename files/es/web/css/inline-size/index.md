---
title: inline-size
slug: Web/CSS/inline-size
translation_of: Web/CSS/inline-size
---
{{CSSRef}}{{SeeCompatTable}}

La propiedad de [CSS](/es/docs/Web/CSS) **`inline-size`** define el tamaño horizontal o vertical de un bloque de elementos, dependiendo del modo de escritura. Esto corresponde ya sea a la propiedad {{cssxref("width")}} o {{cssxref("height")}}, dependiendo del valor de {{cssxref("writing-mode")}}.

{{EmbedInteractiveExample("pages/css/inline-size.html")}}

## Sintaxis

```css
/* <length> values */
inline-size: 300px;
inline-size: 25em;

/* <percentage> values */
inline-size: 75%;

/* Keyword values */
inline-size: 25em border-box;
inline-size: 75% content-box;
inline-size: max-content;
inline-size: min-content;
inline-size: available;
inline-size: fit-content;
inline-size: auto;

/* Global values */
inline-size: inherit;
inline-size: initial;
inline-size: unset;
```

Si el modo de escritura es verticalmente orientado, el valor de `inline-size` se relaciona con la altura del elemento; de lo contrario, se relaciona con el ancho del elemento. Una propiedad relacionada es {{cssxref("block-size")}}, que define la otra dimensión del elemento.

{{cssinfo}}

### Valores

La propiedad `inline-size` toma los mismos valores de las propiedades {{cssxref("width")}} y {{cssxref("height")}}.

### Sintaxis formal

{{csssyntax}}

## Ejemplo

### Contenido HTML

```html
<p class="exampleText">Example text</p>
```

### Contenido CSS

```css
.exampleText {
  writing-mode: vertical-rl;
  background-color: yellow;
  inline-size: 110px;
}
```

{{EmbedLiveSample("Ejemplo")}}

## Especificación

| Especificación                                                                                                       | Estado                                           | Comentario          |
| -------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------ | ------------------- |
| {{SpecName("CSS Logical Properties", "#logical-dimension-properties", "inline-size")}} | {{Spec2("CSS Logical Properties")}} | Definición inicial. |

## Compatibilidad en navegadores

{{Compat("css.properties.inline-size")}}

## Mira también

- Las propiedades físicas mapeadas: {{cssxref("width")}} y {{cssxref("height")}}
- {{cssxref("writing-mode")}}
