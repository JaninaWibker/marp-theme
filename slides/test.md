---
_class: lead
class:
paginate: true
_paginate: false
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

$$\sum^{n}_{i=1} A_i$$

- foo
- bar

1. first
2. second

- [ ] task list
- [x] task list

---

<!--
header: Some kind of header!
footer: A foot note!
_class: invert
-->

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

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
_class: invert
-->

## **Satz**: $e$ ist transzendent

$$
\sum_{j=0}^{m} b_j \cdot F_p(j)
  = \fcolorbox{var(--color-highlight-secondary)}{transparent}{$\displaystyle{  b_0 \cdot \sum_{l=0}^{n_p} f^{(l)}(0)  }$}
  + \fcolorbox{var(--color-accent)}{transparent}{$\displaystyle{  \sum_{j=1}^{m} b_j \cdot \sum_{l=0}^{n_p} f^{(l)}(j)  }$}
$$

$$
\fcolorbox{var(--color-accent)}{transparent}{$\displaystyle{
  \sum_{j=1}^{m} b_j \cdot \sum_{l=0}^{n_p} f^{(l)}(j) = 
  \sum_{j=1}^{m} b_j \cdot \sum_{l=p}^{n_p} a_{p,j,l} \cdot l!
}$}
$$


---

<!--
_footer: ''
_paginate: false
-->

![this is a video](https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4)
