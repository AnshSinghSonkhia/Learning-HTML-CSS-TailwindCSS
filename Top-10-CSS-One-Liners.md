# Top 10 CSS One-Liners - <i>developedbyed</i>

## 1. Vertical Text
The `writing-mode` CSS property sets whether lines of text are laid out horizontally or vertically, as well as the direction in which blocks progress. <br>When set for an entire document, it should be set on the root element <br> (html element for HTML documents).
<p>This property specifies the block flow direction, which is the direction in which block-level containers are stacked, and the direction in which inline-level content flows within a block container. <br>Thus, it also determines the ordering of block-level content.</p>

> Syntax
```
writing-mode: vertical-lr;
```
---
> More Syntax
```
/* Keyword values */
writing-mode: horizontal-tb;
writing-mode: vertical-rl;
writing-mode: vertical-lr;

/* Global values */
writing-mode: inherit;
writing-mode: initial;
writing-mode: revert;
writing-mode: revert-layer;
writing-mode: unset;

```

[Detailed Reference Link](https://developer.mozilla.org/en-US/docs/Web/CSS/writing-mode)

## 2. Gap
The `gap` CSS property sets the gaps (gutters) between rows and columns. It is a shorthand for `row-gap` and `column-gap`.

> **Note** <br>
> The `grid-gap` is an alias for this property.
---

> Syntax
```
/* One <length> value */
gap: 20px;
gap: 1em;
gap: 3vmin;
gap: 0.5cm;

/* One <percentage> value */
gap: 16%;
gap: 100%;

/* Two <length> values */
gap: 20px 10px;
gap: 1em 0.5em;
gap: 3vmin 2vmax;
gap: 0.5cm 2mm;

/* One or two <percentage> values */
gap: 16% 100%;
gap: 21px 82%;

/* calc() values */
gap: calc(10% + 20px);
gap: calc(20px + 10%) calc(10% - 5px);

/* Global values */
gap: inherit;
gap: initial;
gap: revert;
gap: revert-layer;
gap: unset;
```
---

[Detailed Reference Link](https://developer.mozilla.org/en-US/docs/Web/CSS/gap)

## 3. Flip an Image

> Syntax
```
transform: scaleX(-1);
transform: scaleY(-1);
```
---

> More Syntax
```
/* Keyword values */
transform: none;

/* Function values */
transform: matrix(1, 2, 3, 4, 5, 6);
transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
transform: perspective(17px);
transform: rotate(0.5turn);
transform: rotate3d(1, 2, 3, 10deg);
transform: rotateX(10deg);
transform: rotateY(10deg);
transform: rotateZ(10deg);
transform: translate(12px, 50%);
transform: translate3d(12px, 50%, 3em);
transform: translateX(2em);
transform: translateY(3in);
transform: translateZ(2px);
transform: scale(2, 0.5);
transform: scale3d(2.5, 1.2, 0.3);
transform: scaleX(2);
transform: scaleY(0.5);
transform: scaleZ(0.3);
transform: skew(30deg, 20deg);
transform: skewX(30deg);
transform: skewY(1.07rad);

/* Multiple function values */
transform: translateX(10px) rotate(10deg) translateY(5px);
transform: perspective(500px) translate(10px, 0, 20px) rotateY(3deg);

/* Global values */
transform: inherit;
transform: initial;
transform: revert;
transform: revert-layer;
transform: unset;
```

[Detailed Reference Link](https://developer.mozilla.org/en-US/docs/Web/CSS/transform)

## 4. Smooth Scrolling

> Syntax
```
html{
    scroll-behavior: smooth;
}
```

## 5. Smooth Snaping

> Syntax
```
.container {
    overflow-x: scroll;
    scroll-snap-type: x proximity;
}

.container div {
    overflow-x: scroll;
    scroll-snap-align: center;
}
```

## 6. Resize Everything

> Syntax
```
.box {
    ...
    overflow: auto;
    resize: both;
}
```
---
```
resize: vertical;
resize: horizontal;
```

## 7. Truncate

> Syntax
```
.box p {
    max-width: 20rem;
    ...
    display: -webkit-box;
    -webkit-line-clamp: 3;       //To display only 3 lines at once
    -webkit-box-orient: vertical;
    overflow: hidden;
}
```

## 8. Text-Gradient

> Syntax
```
h1 {
    font-size: 10rem;
    background: linear-gradient(to right, rgb(67,124,205), rgb(69,214,202));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}
```

## 9. Object Fit

> Syntax
```
.box {
    background: white;
    width: 25rem;
    height: 40rem;
}

.box img {
    width: 100%;
    height: 100%;
    object-fit: cover;          // This is Object fit property.
}
```

## 10. Pointer Events & Animating Text

> Syntax
```
h1 {
    font-size: 10rem;
    ...
    pointer-events: none;
    opacity: 0
    animation: fade 1s ease-in 1s;
}

@keyframes fade {
    0% {
        opacity: 0;
    }
    100% {
        opacity: 1;
    }
}
```

> You can't animate element if you use &nbsp;&nbsp;  `display: none` &nbsp;&nbsp; property

<!-- YouTube Vidio Link - https://www.youtube.com/watch?v=Xc6G3oV24yE&t=5s -->