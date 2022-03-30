# Array  

Об’єкт Array, як і масиви в інших мовах програмування, дозволяє зберігати колекцію кількох елементів під одним ім’ям змінної та має члени для виконання загальних операцій з масивом.

## Опис
У JavaScript масиви не є примітивами, а є об’єктами масиву з такими основними характеристиками:  
- Масиви JavaScript можна змінювати і можуть містити поєднання різних типів даних. (Якщо ці характеристики небажані, використовуйте натомість типізовані масиви).
- Масиви JavaScript не є асоціативними масивами, тому доступ до елементів масиву неможливий за допомогою рядків як індексів, але доступ до них має бути за допомогою цілих чисел як індексів.
- Масиви JavaScript мають нульовий індекс: перший елемент масиву має індекс 0, другий — індекс 1 і так далі — і останній елемент має значення властивості довжини масиву мінус 1.
- Операції копіювання масиву JavaScript створюють неглибокі копії. (Усі стандартні вбудовані операції копіювання з будь-якими об’єктами JavaScript створюють неглибокі копії, а не глибокі копії).

## Конструктор (Constructor)
Array()  
Створює новий обєкт масив.

## Статичні властивості (Static properties)
get Array[@@species]  
Повертає конструктор масиву.

## Статичні методи (Static methods)
Array.from()  
Створює новий екземпляр масиву з об’єкта, подібного до масиву, або об’єкта, який можна повторювати.  
Array.isArray()  
Повертає true, якщо аргумент є масивом, або false в іншому випадку.  
Array.of()  
Створює новий екземпляр масиву зі змінною кількістю аргументів, незалежно від кількості чи типу аргументів.  

## Властивості сущності (Instance properties)
Array.prototype.length  
Відображає число елементів у масиві.  
Array.prototype[@@unscopables]  
Містить імена властивостей, які не були включені в стандарт ECMAScript до версії ES2015 і які ігноруються з метою зв’язування операторів.  

## Методи сущності (Instance methods)
- Array.prototype.at()  

- Array.prototype.concat()  

- Array.prototype.copyWithin()  

- Array.prototype.entries()  

- Array.prototype.every()  

- Array.prototype.fill()  

- Array.prototype.filter()  

- Array.prototype.find()  

- Array.prototype.findIndex()  

- Array.prototype.flat()  

- Array.prototype.flatMap()  

- Array.prototype.forEach()  

- Array.prototype.groupBy()  

- Array.prototype.groupByToMap()  

- Array.prototype.includes()  

- Array.prototype.indexOf()  

- Array.prototype.join()  

- Array.prototype.keys()  

- Array.prototype.lastIndexOf()  

- Array.prototype.map()  

- Array.prototype.pop()  

- Array.prototype.push()  

- Array.prototype.reduce()  

- Array.prototype.reduceRight()  

- Array.prototype.reverse()  

- Array.prototype.shift()  

- Array.prototype.slice()  

- Array.prototype.some()  

- Array.prototype.sort()  

- Array.prototype.splice()  

- Array.prototype.toLocaleString()  

- Array.prototype.toString()  

- Array.prototype.unshift()  

- Array.prototype.values()  

- Array.prototype[@@iterator]()  
