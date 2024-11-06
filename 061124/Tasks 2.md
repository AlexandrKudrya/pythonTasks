## Задача 1: Исцезнувшее сокровище
Вы — пиратский капитан, который ищет древние сокровища капитана "Бритая борода", самого умного пирата до нашей эры! У вас есть две карты: 
- На одной список всех острово, которые Бритая голова посетил;
- А на второй все острова, которые он завоевал. 
И был лишь 1 остров, который он посетил, но не смог завоевать. **Вот он нам и нужен!**
Напишите программу, чтобы определить, какой элемент отсутствует во втором списке номеров островов.
```python
pythonКопировать код# Пример ввода:
original_islands = [1, 2, 3, 4, 5]
lost_islands = [2, 3, 1, 5]
# Пример вывода:
# Исчезнувший остров: 4
```
**Что используется:** `set`, `-` 
## Задача 2: Команда высадки
Нужно выбрать тех, кто идёт с вами на остров. Всех брать нельзя, но все хотят, ведь кто идёт за сокровищами, получает их больше. 
Вы, как капитан, решаете сделать волевое решение: всять каждого третьего! 

У вас есть список имён, нужно выбрать каждого третьего из списка.
```python
# Пример ввода:
people = ["Анна", "Борис", "Виктор", "Галя", "Дима", "Елена", "Женя"]
# Пример вывода:
# Команда высадки: ['Виктор', 'Дима', 'Женя']

```
**Что используется:** `срезы списков`
## Задача 3: Испытание первое - лестница
Вы входите в пещеру с кладом. Пред вами предстаёт первое испытание капитана Бритая Борода: Лестница джокушка-ловушкера. 

Какие-то ступени с ловушками, а какие-то безопасны. И над каждой ступенью есть цифра. Как гласит первая подсказка Бритой бороды:
"Эт, того, ну короче, если чётная ступенька с чётной цифрой, то наступать можно, а если нет, то нельзя. А, да, и если нечётная с нечётной, то тоже можно, совсем забыл". 

Дан список цифр над ступеньками, нужно вывести безопастные. 

```python
# Пример ввода:
steps = [2, 2, 3, 5, 9, 6, 6, 8]
# Пример вывода:
# Нормальные ступеньки: 
[2, 3, 9, 6, 8]
```
**Что используется:** `for`, `range`, `if`, `%`
##  Задача 4: Испытание второе - лабиринт
После спуска по лестице вы входите в лабиринт. В нём множество пронумерованных проходов. Но вы знаете, что идити надо так, чтобы номер прохода не уменьшался. 

Вам нужно найти все проходы, которые идут подряд в порядке возрастания. Напишите программу, которая определяет самую длинную последовательность возрастающих чисел.
```python
# Пример ввода:
path_numbers = [1, 2, 5, 3, 4, 6, 7, 2, 8]
# Пример вывода:
# Как надо идти: [1, 2, 5, 6, 7, 8]
```
**Что используется:** `for`, `range`, `if`, `>`
##  Задача 5: Испытание третье - пароль
И вот вы на пороге сокровищницы Бритой головы. Но проблема: тут есть пароль! Хорошо, что рядом вы нашли список с паролями, но их слишком много, чтобы вы могли перебрать все. 

Тут вы вспонинаете, что Бритая Голова был очень умён, поэтому стал бы использовать только надёждный пароль:
- В надёжном пароле есть как минимум 1 буква
- В надёжном пароле есть цифра;
Напишите программу, чтобы проверить, какие пароли соответствуют требованиям.
```python
# Пример ввода:
passwords = ["abc", "abc123", "123", "password"]
# Пример вывода:
# Надёжные пароли: ['abc123']

```
**Что используется:** `for`, `.isalpha`, `.isdigit`
## Задача 6*: Злые аборигены
Вы победно выходите с сокровищами, но там вас встречают злобные аборигены, нужно договариваться! Но у них свой странный язык: 
- Каждое слово имеет начало, которое совпадает с первой половиной слова из списка Аба, а конец совпадает со второй половиной из списка из Ага. 
- Либо наоборот - начало из Ага, конец из Аба
Вам известны оба словаря, нужно получить 2 списока слов: 
1. начала из Аба, конец из Ага
2. начала из Ага, конец из Аба

```python
Aba = ['Альфа', 'Бета', 'Гамма']
Aga = ['Космос', 'Вселенная', 'Магнит']

# Скрещенные слова
['Алмос', 'Бетанная', 'Гамнит']

# Обратные слова
['Косфа', 'Вселета', 'Магма']
```
**Что используется:** `for`, `срезы списков`, `\\`