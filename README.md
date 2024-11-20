# Четвертое занятие


## Массивы.

### Проблема хранения коллекции данных.
```bash
На вход дается 35 оценок по математике учеников 9 "A" класса. 
Необходимо посчитать среднюю оценку в классе по математике.
```
<br />

### Создание массивов
```php
// через функцию array(...)
$marks1 = array(5, 3, 4, 3, 5, 4);

// через []
$marks2 = [5, 3, 4, 3, 5, 4];
```
<br />

### Доступ к элементам массива(чтение)
```php
echo $marks[0] . PHP_EOL;
echo $marks[1] . PHP_EOL;
echo $marks[2] . PHP_EOL;
echo $marks[3] . PHP_EOL;
echo $marks[4] . PHP_EOL;
```

<br />

### Размер массива
```php
echo count($marks);
```

### Перебор массива циклом
```php
for ($i = 1; $i < count($marks); $i++) {
    echo $marks[$i] . PHP_EOL;
}
```

### Ассоциативный массив
```php
$biography = [
    'name' => 'Franz',
    'surname' => 'Kafka',
    'birth_date' => 1883,
];

// Как перебрать ассоциативный массив?
echo $biography['name'] . PHP_EOL;
echo $biography['surname'] . PHP_EOL;
echo $biography['birth_date'] . PHP_EOL;
```

<br />

### Цикл foreach
```php
// Перебор значений
foreach ($biography as $value) {
    echo $value . PHP_EOL;
}

// Перебор ключей и значений
foreach ($biography as $key => $value) {
    echo "$key: $value" . PHP_EOL;
}
```

### Добавление нового элемента в массив
```php
$marks[] = 5; // в конец

$biography['birth_place'] = 'Praga'; // по ключу
```


### Доступ к элементам массива(запись)
```php
$marks[0] = 5;
$biography['name'] = 'John';
```

### Copy on write
```php
$a = [1, 2, 3]
$b = $a;

$a[] = 4;

echo $a . PHP_EOL;
echo $b . PHP_EOL;
```

### Многомерные массивы.
```php
```

<br />
<br />

### Задачи на уроке/Домашнее задание
1. Дан массив целых чисел. Посчитать сумму элементов массива.
2. Дан массив целых чисел. Посчитать среднее элементов массива.
3. [Разворот](https://acmp.ru/asp/do/index.asp?main=topic&id_course=2&id_section=10&id_topic=4)
4. [Количество элементов, больших предыдущего](https://informatics.msk.ru/mod/statements/view.php?id=208&chapterid=66#1)
5. [Переставить соседние элементы](https://informatics.msk.ru/mod/statements/view.php?id=208&chapterid=70#1)
6. [Количество элементов больших обоих соседей](https://informatics.msk.ru/mod/statements/view.php?id=208&chapterid=68#1)
7. Найти разность между максимальным и минимальным элементами массива
8. Поменять местами минимальный и максимальный элементы массива
9. Вывести элементы массива, которые больше среднего арифметического
10. Найти в массиве самую длинную последовательность, состоящую из одинаковых элементов
11. Дан массив целых чисел. Проверить, есть ли в нем одинаковые элементы.
12. Написать реализацию линейного поиска в массиве.
13. Написать реализацию пузырьковой сортировки.
---



### Материалы:
1. [Arrays](https://www.php.net/manual/en/language.types.array.php)
2. [Arrays Functions](https://www.php.net/manual/en/ref.array.php)