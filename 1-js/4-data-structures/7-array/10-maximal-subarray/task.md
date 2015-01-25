# Подмассив наибольшей суммы

[importance 2]

На входе массив чисел, например: `arr = [1, -2, 3, 4, -9, 6]`.

Задача -- найти непрерывный подмассив `arr`, сумма элементов которого максимальна. 

Ваша функция должна возвращать только эту сумму.

Например:

```js
getMaxSubSum([-1, *!*2, 3*/!*, -9]) = 5 (сумма выделенных)
getMaxSubSum([*!*2, -1, 2, 3*/!*, -9]) = 6
getMaxSubSum([-1, 2, 3, -9, *!*11*/!*]) = 11 
getMaxSubSum([-2, -1, *!*1, 2*/!*]) = 3
getMaxSubSum([*!*100*/!*, -9, 2, -3, 5]) = 100
getMaxSubSum([*!*1, 2, 3*/!*]) = 6 (неотрицательные - берем всех)
```

Если все элементы отрицательные, то не берём ни одного элемента и считаем сумму равной нулю:

```js
getMaxSubSum([-1, -2, -3]) = 0
```

Постарайтесь придумать решение, которое работает за O(n<sup>2</sup>), а лучше за O(n) операций.