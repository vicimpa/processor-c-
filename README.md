### Описание языка

Этот язык программирования предназначен для выполнения простых арифметических операций, работы с памятью и управления потоком выполнения с помощью меток и условий. Он имеет следующие основные компоненты:

1. **Память**:
   - Память представлена массивом `memory` размером 32 элемента (`float memory[32]`).
   - Курсор `cursor` указывает на текущую позицию в памяти.

2. **Команды**:
   - Команды определены в виде строк и выполняют различные операции. Вот список поддерживаемых команд:

### Основные команды
- **:** - Перемещает курсор на указанную позицию в памяти.
  - **Синтаксис:** `: <позиция>`
  - **Пример:** `: 5` перемещает курсор на пятую позицию.

- **=** - Записывает указанное значение в текущую позицию памяти.
  - **Синтаксис:** `= <значение>`
  - **Пример:** `= 10` записывает значение 10 в текущую позицию.

### Арифметические операции
- **+** - Добавляет указанное значение к текущему значению в памяти.
  - **Синтаксис:** `+ <значение>`
  - **Пример:** `+ 5` добавляет 5 к текущему значению.

- **-** - Вычитает указанное значение из текущего значения в памяти.
  - **Синтаксис:** `- <значение>`
  - **Пример:** `- 3` вычитает 3 из текущего значения.

- *** - Умножает текущее значение в памяти на указанное значение.
  - **Синтаксис:** `* <значение>`
  - **Пример:** `* 2` умножает текущее значение на 2.

- **/** - Делит текущее значение в памяти на указанное значение.
  - **Синтаксис:** `/ <значение>`
  - **Пример:** `/ 4` делит текущее значение на 4.

- **^** - Возводит текущее значение в памяти в указанную степень.
  - **Синтаксис:** `^ <значение>`
  - **Пример:** `^ 3` возводит текущее значение в степень 3.

- **%** - Вычисляет остаток от деления текущего значения в памяти на указанное значение.
  - **Синтаксис:** `% <значение>`
  - **Пример:** `% 2` вычисляет остаток от деления на 2.

### Математические функции
- **sin** - Вычисляет синус текущего значения в памяти.
  - **Синтаксис:** `sin`
  - **Пример:** `sin` вычисляет синус текущего значения.

- **cos** - Вычисляет косинус текущего значения в памяти.
  - **Синтаксис:** `cos`
  - **Пример:** `cos` вычисляет косинус текущего значения.

- **tan** - Вычисляет тангенс текущего значения в памяти.
  - **Синтаксис:** `tan`
  - **Пример:** `tan` вычисляет тангенс текущего значения.

- **atan** - Вычисляет арктангенс текущего значения в памяти.
  - **Синтаксис:** `atan`
  - **Пример:** `atan` вычисляет арктангенс текущего значения.

- **rand** - Генерирует случайное число и записывает его в текущую позицию памяти.
  - **Синтаксис:** `rand`
  - **Пример:** `rand` генерирует случайное число.

- **floor** - Приводит текущее значение в памяти к наименьшему целому числу.
  - **Синтаксис:** `floor`
  - **Пример:** `floor` округляет текущее значение вниз.

- **round** - Приводит текущее значение в памяти к ближайшему целому числу.
  - **Синтаксис:** `round`
  - **Пример:** `round` округляет текущее значение до ближайшего целого.

- **ceil** - Приводит текущее значение в памяти к наибольшему целому числу.
  - **Синтаксис:** `ceil`
  - **Пример:** `ceil` округляет текущее значение вверх.

### Условные операторы
- **lt** - Если текущее значение в памяти меньше указанного, выполняет следующую строку, иначе пропускает.
  - **Синтаксис:** `lt <значение>`
  - **Пример:** `lt 10` проверяет, меньше ли текущее значение 10.

- **gt** - Если текущее значение в памяти больше указанного, выполняет следующую строку, иначе пропускает.
  - **Синтаксис:** `gt <значение>`
  - **Пример:** `gt 5` проверяет, больше ли текущее значение 5.

- **lte** - Если текущее значение в памяти меньше или равно указанному, выполняет следующую строку, иначе пропускает.
  - **Синтаксис:** `lte <значение>`
  - **Пример:** `lte 8` проверяет, меньше или равно ли текущее значение 8.

- **gte** - Если текущее значение в памяти больше или равно указанному, выполняет следующую строку, иначе пропускает.
  - **Синтаксис:** `gte <значение>`
  - **Пример:** `gte 3` проверяет, больше или равно ли текущее значение 3.

- **eq** - Если текущее значение в памяти равно указанному, выполняет следующую строку, иначе пропускает.
  - **Синтаксис:** `eq <значение>`
  - **Пример:** `eq 7` проверяет, равно ли текущее значение 7.

- **neq** - Если текущее значение в памяти не равно указанному, выполняет следующую строку, иначе пропускает.
  - **Синтаксис:** `neq <значение>`
  - **Пример:** `neq 7` проверяет, не равно ли текущее значение 7.

### Управление потоком
- **(** - Устанавливает метку на текущей строке программы.
  - **Синтаксис:** `( <метка>`
  - **Пример:** `( 1` устанавливает метку 1.

- **)** - Переходит к строке программы, помеченной указанной меткой.
  - **Синтаксис:** `) <метка>`
  - **Пример:** `) 1` переходит к метке 1.

- **dump** - Выводит всю память в консоль для отладки.
  - **Синтаксис:** `dump`
  - **Пример:** `dump` выводит текущее состояние памяти.

- **exit** - Завершает выполнение программы.
  - **Синтаксис:** `exit`
  - **Пример:** `exit` завершает программу.

### Примеры программ

#### Пример 1: Простая арифметика
```cpp
: 0
= 10
: 1
= 20
: 2
+ m0
* m1
```
Эта программа:
1. Перемещает курсор на позицию 0 и записывает туда значение 10.
2. Перемещает курсор на позицию 1 и записывает туда значение 20.
3. Перемещает курсор на позицию 2, добавляет значение из ячейки 0 и умножает на значение из ячейки 1.

#### Пример 2: Условное выполнение
```cpp
: 0
= 5
: 1
lt 10
= 100
: 2
gt 10
= 200
```
Эта программа:
1. Перемещает курсор на позицию 0 и записывает туда значение 5.
2. Перемещает курсор на позицию 1 и проверяет, меньше ли текущее значение 10. Если да, то записывает 100 в текущую позицию.
3. Перемещает курсор на позицию 2 и проверяет, больше ли текущее значение 10. Если да, то записывает 200 в текущую позицию.

#### Пример 3: Использование меток
```cpp
: 0
= 1
( 1
: 1
+ 1
lt 10
) 1
exit
```
Эта программа:
1. Перемещает курсор на позицию 0 и записывает туда значение 1.
2. Устанавливает метку 1 на текущей строке.
3. Перемещает курсор на позицию 1 и добавляет 1 к текущему значению.
4. Проверяет, меньше ли текущее значение 10. Если да, то переходит к строке, помеченной меткой 1.
5. Завершает выполнение программы.

### Заключение

Этот язык программирования предоставляет базовые возможности для выполнения арифметических операций, работы с памятью и управления потоком выполнения с помощью меток и условий. Он может быть полезен для обучения основам интерпретации и создания простых языков программирования.