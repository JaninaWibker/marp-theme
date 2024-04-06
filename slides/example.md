---
_class: lead
class:
paginate: true
_paginate: skip
---

![bg left:40% 80%](https://marp.app/assets/marp.svg)

# **Marp**

Markdown Presentation Ecosystem

https://marp.app/

---

# How to write slides

Split pages by horizontal ruler (`---`). It's very simple! :satisfied:

```markdown
# Slide 1

foobar

---

# Slide 2

foobar
```

---

<!--
_class: invert
-->

# Dark mode

By adding the `.invert` class you switch to dark mode.

To do this for a single slide add this:

```html
<!--
_class: invert
-->
```

This can be done with frontmatter as well on the first slide, the html comment is the variant which can be placed on any slide.

---

# Basic building blocks

- an unordered list
- with a few items

1. an ordered list
2. with a few items

- [x] checkmarks
- [ ] work too

---

<!--
_class: invert
-->

# Basic building blocks

- an unordered list
- with a few items

1. an ordered list
2. with a few items

- [x] checkmarks
- [ ] work too

---

normal text
**bold text**
*italic text*

superscript: a^1^
subscript: b~2~

underline: _test_

strikethrough: ~~test~~

mark: ==test==

---

We got support for latex math mode:

$$
\sum_{j=0}^{m} b_j \cdot F_p(j)
  = \fcolorbox{var(--color-highlight-secondary)}{transparent}{$\displaystyle{  b_0 \cdot \sum_{l=0}^{n_p} f^{(l)}(0)  }$}
  + \fcolorbox{var(--color-accent)}{transparent}{$\displaystyle{  \sum_{j=1}^{m} b_j \cdot \sum_{l=0}^{n_p} f^{(l)}(j)  }$}
$$

You can reference css variables with KaTeX as well:

```latex
\fcolorbox{var(--color-highlight-secondary)}{transparent}{
  the content
}
```

---

<!--
header: 'A header!'
footer: 'A footer!'
-->

# Header and Footer

Add a header or footer using
- `header` (global until overwritten),
- `_header` (local),
- `footer` (global until overwritten), or
- `_footer` (local)

in the frontmatter / html comment.

---

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

---

<!--
_class: lead
-->

# Title slides

*Add `_class: lead`* to a slide to make it a title slide

---

<!--
_class: invert
-->

> blockquote

|             |          Grouping           ||
First Header  | Second Header | Third Header |
 ------------ | :-----------: | -----------: |
Content       |          *Long Cell*        ||
Content       |   **Cell**    |         Cell |
                                              
New section   |     More      |         Data |
And more      | With an escaped '\\|'       ||

---

<!--
_footer: ''
-->

# Light mode code block

```js
module.exports = function leftpad(str, len, ch) {
  str = String(str);
  var i = -1;

  if (!ch && ch !== 0) ch = ' ';

  len = len - str.length;

  while (i++ < len) {
    str = ch + str;
  }
  return str;
}
```

---

<!--
_class: invert
_footer: ''
-->

# Dark mode code block

```js
module.exports = function leftpad(str, len, ch) {
  str = String(str);
  var i = -1;

  if (!ch && ch !== 0) ch = ' ';

  len = len - str.length;

  while (i++ < len) {
    str = ch + str;
  }
  return str;
}
```

---

<!--
_class: lead
-->

# Page numbers

*See how you can control page numbers*

---

# Page numbers

Use `_paginate: true | false | skip | hold` to control how page numbers are displayed.

`_paginate: true` shows the page number and increments it

---

# Page numbers

Use `_paginate: true | false | skip | hold` to control how page numbers are displayed.

`_paginate: false` hides the page number but still increments it

---

# Page numbers

Use `_paginate: true | false | skip | hold` to control how page numbers are displayed.

`_paginate: skip` hides the page number and doesn't increment it

<br />
<br />

> You can use this for the title slide

---

# Page numbers

Use `_paginate: true | false | skip | hold` to control how page numbers are displayed.

`_paginate: hold` shows the page number without incrementing it

---

<!--
_paginate: hold
_footer: See? the page number didn't change
-->

# Page numbers

Use `_paginate: true | false | skip | hold` to control how page numbers are displayed.

`_paginate: hold` shows the page number without incrementing it

<br />

> **Animations**: Duplicate slide, add/change content on the second slide. Both slides share the same page number

---

<!--
_class: lead
_header: ''
_footer: ''
-->

# You can even use videos

*See next slide, only works in the browser*

---

<!--
_header: ''
_footer: ''
_paginate: false
-->

![this is a video](https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4)
