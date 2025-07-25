---
title: <gradient>
slug: Web/CSS/gradient
page-type: css-type
browser-compat: css.types.gradient
sidebar: cssref
---

The **`<gradient>`** [CSS](/en-US/docs/Web/CSS) [data type](/en-US/docs/Web/CSS/CSS_Values_and_Units/CSS_data_types) is a special type of {{cssxref("&lt;image&gt;")}} that consists of a progressive transition between two or more colors.

{{InteractiveExample("CSS Demo: &amp;lt;gradient&amp;gt;")}}

```css interactive-example-choice
background: linear-gradient(#f69d3c, #3f87a6);
```

```css interactive-example-choice
background: radial-gradient(#f69d3c, #3f87a6);
```

```css interactive-example-choice
background: repeating-linear-gradient(#f69d3c, #3f87a6 50px);
```

```css interactive-example-choice
background: repeating-radial-gradient(#f69d3c, #3f87a6 50px);
```

```css interactive-example-choice
background: conic-gradient(#f69d3c, #3f87a6);
```

```html interactive-example
<section class="display-block" id="default-example">
  <div id="example-element"></div>
</section>
```

```css interactive-example
#example-element {
  min-height: 100%;
}
```

A CSS gradient has [no intrinsic dimensions](/en-US/docs/Web/CSS/image#description); i.e., it has no natural or preferred size, nor a preferred ratio. Its concrete size will match the size of the element to which it applies.

## Syntax

The `<gradient>` data type is defined with one of the function types listed below.

### Linear gradient

Linear gradients transition colors progressively along an imaginary line. They are generated with the {{cssxref("gradient/linear-gradient", "linear-gradient()")}} function.

### Radial gradient

Radial gradients transition colors progressively from a center point (origin). They are generated with the {{cssxref("gradient/radial-gradient", "radial-gradient()")}} function.

### Conic gradient

Conic gradients transition colors progressively around a circle. They are generated with the {{cssxref("gradient/conic-gradient", "conic-gradient()")}} function.

### Repeating gradient

Repeating gradients duplicate a gradient as much as necessary to fill a given area. They are generated with the {{cssxref("gradient/repeating-linear-gradient", "repeating-linear-gradient()")}}, {{cssxref("gradient/repeating-radial-gradient", "repeating-radial-gradient()")}}, and {{cssxref("gradient/repeating-conic-gradient", "repeating-conic-gradient()")}} functions.

## Interpolation

As with any interpolation involving colors, gradients are calculated in the alpha-premultiplied color space. This prevents unexpected shades of gray from appearing when both the color and the opacity are changing. (Be aware that older browsers may not use this behavior when using the [transparent keyword](/en-US/docs/Web/CSS/named-color#transparent).)

## Formal syntax

{{csssyntax}}

## Examples

### Linear gradient example

A linear gradient.

```html hidden
<div class="linear-gradient">Linear gradient</div>
```

```css hidden
div {
  width: 240px;
  height: 80px;
}
```

```css
.linear-gradient {
  background: linear-gradient(
    to right,
    red,
    orange,
    yellow,
    green,
    blue,
    indigo,
    violet
  );
}
```

{{EmbedLiveSample('Linear_gradient_example', 240, 120)}}

### Radial gradient example

A radial gradient.

```html hidden
<div class="radial-gradient">Radial gradient</div>
```

```css hidden
div {
  width: 240px;
  height: 80px;
}
```

```css
.radial-gradient {
  background: radial-gradient(red, yellow, rgb(30 144 255));
}
```

{{EmbedLiveSample('Radial_gradient_example', 240, 120)}}

### Conic gradient example

A conic gradient example.

```html hidden
<div class="conic-gradient">Conic gradient</div>
```

```css hidden
div {
  width: 200px;
  height: 200px;
}
```

```css
.conic-gradient {
  background: conic-gradient(pink, coral, lime);
}
```

{{EmbedLiveSample('Conic_gradient_example', 240, 240)}}

### Repeating gradient examples

Repeating linear and radial gradient examples.

```html hidden
<div class="linear-repeat"></div>
<span>Repeating linear gradient</span>
<hr />
<div class="radial-repeat"></div>
<span>Repeating radial gradient</span>
<hr />
<div class="conic-repeat"></div>
<span>Repeating conic gradient</span>
```

```css hidden
div {
  display: inline-block;
  width: 240px;
  height: 80px;
}

span {
  font-weight: bold;
  vertical-align: top;
}
```

```css
.linear-repeat {
  background: repeating-linear-gradient(
    to top left,
    pink,
    pink 5px,
    white 5px,
    white 10px
  );
}

.radial-repeat {
  background: repeating-radial-gradient(
    lime,
    lime 15px,
    white 15px,
    white 30px
  );
}

.conic-repeat {
  background: repeating-conic-gradient(lime, pink 30deg);
}
```

{{EmbedLiveSample('Repeating_gradient_examples', 240, 300)}}

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [Using CSS gradients](/en-US/docs/Web/CSS/CSS_images/Using_CSS_gradients)
- Gradient functions: {{cssxref("gradient/linear-gradient", "linear-gradient()")}}, {{cssxref("gradient/repeating-linear-gradient", "repeating-linear-gradient()")}}, {{cssxref("gradient/radial-gradient", "radial-gradient()")}}, {{cssxref("gradient/repeating-radial-gradient", "repeating-radial-gradient()")}}, {{cssxref("gradient/conic-gradient", "conic-gradient()")}}, {{cssxref("gradient/repeating-conic-gradient", "repeating-conic-gradient()")}}
- [CSS Basic Data Types](/en-US/docs/Web/CSS/CSS_Values_and_Units/CSS_data_types)
- [CSS values and units](/en-US/docs/Web/CSS/CSS_Values_and_Units) module
- [Learn: Values and Units](/en-US/docs/Learn_web_development/Core/Styling_basics/Values_and_units)
