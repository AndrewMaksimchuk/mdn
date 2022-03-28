# Object.is()

Цей метод визначає чи два значення однакові чи різні.

## Синтаксис
```Object.is(value1, value2)```

## Параметри
```value1``` - перше значення для порівняння  
```value2``` - друге значення для порівняння

## Результат що повертає метод
Тип: Boolean  
Повідомляє коли два значення однакові чи різні.

## Опис
Два значення однакові якщо виконується одне із наступних:  
- обидва undefined
- обидва null
- обидва true або обидва false
- обидва типу String з однаковою довжиною з такими ж символами в тому самому порядку
- обидва один і той самий об`єкт(посилання в памяті)
- обидва типу Number та
    - обидва +0
    - обидва -0
    - обидва NaN
    - обидва не 0 та не NaN і мають однакове значення

## Приклади
```
Object.is(25, 25); // true
Object.is('foo', 'foo'); // true
Object.is('foo', 'bar'); // false
Object.is(null, null); // true
Object.is(undefined, undefined); // true
Object.is(window, window); // true
Object.is([], []); // false
const foo = {a: 1};
const bar = {a: 1};
Object.is(foo, foo); // true
Object.is(foo, bar); // false

Object.is(0, 0); // false
Object.is(+0, -0); // false
Object.is(-0, -0); // true
Object.is(0n, -0n); // true

Object.is(NaN, 0/0); // true
Object.is(NaN, Number.NaN); // true
```