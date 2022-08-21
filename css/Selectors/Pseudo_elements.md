# Псевдоелементи

Псевдоелемент CSS – це ключове слово, додане до селектора, яке дозволяє стилізувати певну частину вибраного елемента(ів). Наприклад, `::first-line` можна використовувати для зміни шрифту першого рядка абзацу.

```
/* The first line of every <p> element. */
p::first-line {
  color: blue;
  text-transform: uppercase;
}
```
## Синтаксис
selector::pseudo-element {
  property: value;
}

У селекторі можна використовувати лише один псевдоелемент. Він має з’являтися після простих селекторів у операторі.  

## Алфавітний покажчик
Псевдоелементи, визначені набором специфікацій CSS, включають наступне:
```
    ::after (:after)
    ::backdrop
    ::before (:before)
    ::cue
    ::cue-region
    ::first-letter (:first-letter)
    ::first-line (:first-line)
    ::file-selector-button
    ::grammar-error Experimental
    ::marker
    ::part()
    ::placeholder
    ::selection
    ::slotted()
    ::spelling-error Experimental
    ::target-text
```