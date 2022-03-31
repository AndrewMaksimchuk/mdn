# Object  

Клас Object представляє один із типів даних JavaScript. Він використовується для зберігання різноманітних колекцій ключів і більш складних сутностей. Об’єкти можна створювати за допомогою конструктора `Object()` або синтаксису ініціализатора/літерала об’єкта.  

## Опис

Майже всі об'єкти в JavaScript є екземплярами Object; типовий об’єкт успадковує властивості (включаючи методи) від Object.prototype, хоча ці властивості можуть бути затінені (він же перевизначені). Однак об’єкт може бути свідомо створений, для якого це не відповідає дійсності (наприклад, Object.create(null)), або він може бути змінений таким чином, що це більше не відповідає дійсності (наприклад, за допомогою Object.setPrototypeOf).  

Зміни в об'єкті-прототипі Object бачать усі об'єкти через ланцюжок прототипів, якщо властивості та методи, що підпадають під ці зміни, не змінюються далі вздовж ланцюжка прототипів. Це забезпечує дуже потужний, хоча й потенційно небезпечний механізм для зміни або розширення поведінки об’єкта.  

Конструктор Object створює обгортку об'єкта для заданого значення.  
- Якщо значення є нульовим або невизначеним, воно створить і поверне порожній об’єкт.
- Якщо значення вже є об’єктом, воно поверне значення.
- В іншому випадку він поверне об’єкт типу, який відповідає заданому значенню.  

При виклику в контексті без конструктора Object поводиться так само, як і new Object().  

## Видалення властивості з об’єкта

У самому об’єкті немає методу для видалення його власних властивостей (наприклад, Map.prototype.delete()). Для цього необхідно скористатися оператором delete.

## Конструктор
Об'єкт()
Створює новий об’єкт Object. Це обгортка для заданого значення.

## Статичні методи
Object.assign()  
Object.create()  
Object.defineProperty()  
Object.defineProperties()  
Object.entries()  
Object.freeze()  
Object.fromEntries()  
Object.getOwnPropertyDescriptor()  
Object.getOwnPropertyDescriptors()  
Object.getOwnPropertyNames()  
Object.getOwnPropertySymbols()  
Object.getPrototypeOf()  
Object.is()  
Object.isExtensible()  
Object.isFrozen()  
Object.isSealed()  
Object.keys()  
Object.preventExtensions()  
Object.seal()  
Object.setPrototypeOf()  
Object.values()  

## Властивості сущностей
Object.prototype.constructor  

Object.prototype.\_\_proto\_\_  


## Методи сущностей
Object.prototype.\_\_defineGetter\_\_()  

Object.prototype.\_\_defineSetter\_\_()  

Object.prototype.\_\_lookupGetter\_\_()  

Object.prototype.\_\_lookupSetter\_\_()  

Object.prototype.hasOwnProperty()  

Object.prototype.isPrototypeOf()  

Object.prototype.propertyIsEnumerable()  

Object.prototype.toLocaleString()  

Object.prototype.toString()  

Object.prototype.valueOf()  
