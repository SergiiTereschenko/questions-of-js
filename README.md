# questions-of-god

###### Что выведется в консоль? Как добиться правильного вывода в консоль, не убирая setTimeout?
```js
for (var i = 0; i < 10; i++) {
  setTimeout(() => {
    console.log(i); // ?
  }, 0);
}
```
---
###### Что выведется в консоль?
```js
var a = b = {
  value: 1,
};

var b = {
  value: 2,
};

a.value = 3;

console.log(a.value); // ?
console.log(b.value); // ?
```

---

###### Что выведется в консоль?
```js
var a = {
  v: 1,
};

var b = {
  v: 2,
};

function logValue() {
  console.log(this.v);
}

logValue.bind(a).bind(b)(); // ?
```

---

###### Что такое call, apply, bind, зачем они нужны.

---

###### Напишите полифил функции bind.

--- 

###### Дан массив целых чисел, найдите наибольшее из них.

---

###### Даны два массива целых чисел, найдите общие элементы.

---

###### Напишите функцию, принимающую на вход строку и проверяющую, является ли эта строка палиндромом. Приведите несколько вариантов решения.

---

###### Напишите функцию, принимающую массив произвольных слов и на выходе дающую двумерный массив анаграмм:
```
['стол', 'барокко', слот', 'кот', 'кошка', 'ток', 'коробка']
// ->
[
  ['стол', 'слот'],
  ['кот', 'ток'],
  ['барокко', 'коробка'],
]
```

---

###### Есть два класса: принтер с методом print() и сканер с методом scan(). Нужно получить класс МФУ, имеющий оба этих метода.

---

###### Напишите функцию, принимающую на вход время (в любом формате) и возвращающую угол между стрелками аналоговых часов.

---

###### Дано поле морского боя с размеченными на нём кораблями. Спроектируйте решение для подсчёта количества кораблей на этом поле.

---

###### Напишите функцию для сложения чисел, поддерживающую неограниченное количество вызовов:
```js
sum(2)(3)(); // -> 5
sum(1)(2)(3)(4)(); // -> 10
```

---

### Напишите функцию, которая принимает массив с неограниченной вложенностью и делает из него плоский массив:
```js
[1, [2, [3, 4], 5], 6, [7]]
// ->
[1, 2, 3, 4, 5, 6, 7]
```

---

###### Чем поведение скрипта с атрибутом defer отличается от async?

---

###### Есть массив с адресами картинок. Как загрузить все картинки и выполнить какую-либо операцию после окончания загрузки всех картинок?

---

###### Дан односвязный список. Напишите функцию, которая вернёт значение n-ого с конца списка элемента.
```js
{
  value: 0,
  next: {
    value: 5,
    next: {
      value: 2,
      next: null,
    },
  },
};
```

---

###### Расскажите всё, что вы знаете о событиях в JS.

---

###### В соцсети выложили фото котят, под ним динамически добавляются комментарии. У каждого комментария есть кнопка «лайк», при нажатии на которую нужно отправлять запрос к АПИ. Как эффективно реализовать сценарий с нажатием кнопки?

---

###### Как расположить элемент по центру экрана с помощью CSS (назовите все известные вам варианты).

---

###### Опишите процесс отрисовки страницы браузером.

---

###### Дана строка с последовательностью скобок разного вида (`[], ()`). В строке также могут быть и не скобки. Написать метод, который вернёт `true`, если вложенность скобок и их закрытость не нарушена.

---

###### Дан длинный метод, без комментариев, написанный как будто после страшного бодуна. Задача: разобраться что этот метод делает и переписать его так, чтобы там было не 30 строк, а где-то 5-6. И желательно при этом не проиграть в производительности. Мне попалась своеобразная реализация `String.findLastIndex`, которая находит индекс одного из двух, переданных в аргументах, char-ов с конца.

---

###### Вечерняя задача на смекалку: напишите функции cons, car и cdr с интерфейсом как на скриншоте, не используя никакие средства языка, кроме функций (нельзя использовать ни переменные, ни условия, ни что-то другое).
```js
function cons(a, b) {
  /* ... */
}

function car(pair) {
  /* ... */
}

function cdr(pair) {
  /* ... */
}

car(cons('a', 'b')); // 'a'
cdr(cons('a', 'b')); // 'b'
cdr(cdr(cons('a', cons('b', 'c')))); // 'c'
```

---
