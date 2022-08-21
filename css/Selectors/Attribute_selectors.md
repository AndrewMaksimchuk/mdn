# Селектор атрибутів

Селектор атрибутів CSS зіставляє елементи на основі наявності або значення певного атрибута.

```
/* <a> elements with a title attribute */
a[title] {
  color: purple;
}

/* <a> elements with an href matching "https://example.org" */
a[href="https://example.org"] {
  color: green;
}

/* <a> elements with an href containing "example" */
a[href*="example"] {
  font-size: 2em;
}

/* <a> elements with an href ending ".org" */
a[href$=".org"] {
  font-style: italic;
}

/* <a> elements whose class attribute contains the word "logo" */
a[class~="logo"] {
  padding: 2px;
}
```

## Синтаксис
`[attr]`  
Представляє елементи з назвою атрибута attr.

`[attr=значення]`  
Представляє елементи з назвою атрибута attr, значення якого точно дорівнює значенню.

`[attr~=значення]`  
Представляє елементи з іменем атрибута attr, значенням якого є список слів, розділених пробілами, одне з яких точно є значенням.

`[attr|=значення]`  
Представляє елементи з іменем атрибута attr, значення якого може бути точно значенням або може починатися зі значення, одразу після якого йде дефіс, - (U+002D). Його часто використовують для збігів субкодів мови.

`[attr^=value]`  
Представляє елементи з іменем атрибута attr, значення якого має префікс (передує) значенню.

`[attr$=value]`  
Представляє елементи з іменем атрибута attr, значення якого суфіксується (за яким йде значення).

`[attr*=значення]`  
Представляє елементи з іменем атрибута attr, значення якого містить принаймні одне значення в рядку.

`[значення оператора attr i]`  
Додавання i (або I) перед закриваючою дужкою призводить до порівняння значення без урахування регістру (для символів у діапазоні ASCII).

`[attr operator value s]` Експериментальний  
Додавання s (або S) перед закриваючою дужкою призводить до порівняння значення з урахуванням регістру (для символів у діапазоні ASCII).

## Приклади
```
a {
  color: blue;
}

/* Internal links, beginning with "#" */
a[href^="#"] {
  background-color: gold;
}

/* Links with "example" anywhere in the URL */
a[href*="example"] {
  background-color: silver;
}

/* Links with "insensitive" anywhere in the URL,
   regardless of capitalization */
a[href*="insensitive" i] {
  color: cyan;
}

/* Links with "cAsE" anywhere in the URL,
with matching capitalization */
a[href*="cAsE" s] {
  color: pink;
}

/* Links that end in ".org" */
a[href$=".org"] {
  color: red;
}

/* Links that start with "https" and end in ".org" */
a[href^="https"][href$=".org"] {
  color: green;
}

/* All divs with a `lang` attribute are bold. */
div[lang] {
  font-weight: bold;
}

/* All divs without a `lang` attribute are italicized. */
div:not([lang]) {
  font-style: italic;
}

/* All divs in US English are blue. */
div[lang~="en-us"] {
  color: blue;
}

/* All divs in Portuguese are green. */
div[lang="pt"] {
  color: green;
}

/* All divs in Chinese are red, whether
   simplified (zh-CN) or traditional (zh-TW). */
div[lang|="zh"] {
  color: red;
}

/* All divs with a Traditional Chinese
   `data-lang` are purple. */
/* Note: You could also use hyphenated attributes
   without double quotes */
div[data-lang="zh-TW"] {
  color: purple;
}

/* Case-sensitivity depends on document language */
ol[type="a"] {
  list-style-type: lower-alpha;
  background: red;
}

ol[type="b" s] {
  list-style-type: lower-alpha;
  background: lime;
}

ol[type="B" s] {
  list-style-type: upper-alpha;
  background: grey;
}

ol[type="c" i] {
  list-style-type: upper-alpha;
  background: green;
}

```