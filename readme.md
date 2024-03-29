# Вступительный контест Backend-разработка на Java, весна 2024

## 1 задание
Львенок Максим использует в качестве паролей только последовательности из цифр.
Все пароли Максим хранит в одном текстовом файле в формате «code[DIGITS]», где вместо [DIGITS]
подставляются цифры очередного пароля. Кроме записей паролей, в этом файле содержатся другие
строчные латинские буквы, которые должны помогать Льву вспоминать, от чего тот илиной пароль.
Однажды Максим решил разобраться в своих паролях и распечатать свой файл. Он не хочет печатать
этот файл в явном виде с паролями, так как это не безопасно.
Помогите Львенку и напишите программу, которая заменит все вхождения паролей в файле (вместе
cо словом code) на «???» (три символа вопроса).

### Формат входных данных  
В первой и единственной строке входных данных дано содержимое текстового файла. Текстовый
файл содержит только строчные латинские буквы и цифры. Гарантируется, что текстовый файл
содержит не больше 10° символов.

### Формат выходных данных  
Выведите содержимое файла с паролями, в котором вместо каждого пароля будут выведены три
вопросительных знака.

## Примеры данных

### Пример 1  
    
    Ввод                            Вывод
    a1b2c3                          a1b2c3

### Пример 2

    Ввод                            Вывод 
    code12345                       ???

### Пример 3

    Ввод                            Вывод
    aaacodebcode1code2code3bbb      aaacodeb?????????bbb

### Пример 4

    Ввод                            Вывод
    code999andcodec1andcocode888    ???andcodec1andco???

## 2 задание
Заяц Миша очень любит читать, поэтому на новый год ему подарили n книг.

Михаил хочет сложить компактно все подаренные книги в несколько стопок. Заяц считает, что книги
сложены в стопки красиво, если в каждой стопке все книги имеют одинаковую высоту.

Миша хочет сложить книги в минимальное число стопок так, чтобы книги были сложены красиво.
Помогите ему и найдите, как нужно сложить книги в стопки.

### Формат входных данных
В первой строке входных данных дано целое число п - число книг, подаренных Зайцу

Во второй строке дано п целых чисел x1,... , xn - высоты книг

### Формат выходных данных
В первой строке вывода напечатайте одно число к - минимальное число стопок книг.

Во второй строке выведите высоты стопок книг в порядке неубывания.

### Замечание  
Обратите внимание, что в ответе нужно вывести высоты стопок книг, а не высоты книг в стопках.

В первом примере из условия Миша может сложить книги в две стопки, высота каждой из стопок
будет равна 1.

Во втором примере из условия Миша может сложить книги в три стопки: в первой будут одна книга с
высотой 1, во второй одна книга с высотой 3, в третьей - две книги с высотой 2.

## Примеры данных

### Пример 1

    Ввод            Вывод
    2               2
    1 2             1 1
    
### Пример 2

    Ввод            Вывод
    4               3
    1 2 2 3         1 1 2

### Пример 3

    Ввод            Вывод
    5               2
    5 4 4 5 5       2 3 

## 3 задание
Костя ответственно относится к подаркам для своих друзей. В этот раз он решил сделать п подарков
своими руками для своих лучших друзей.

Для изготовления подарков он заказал материалы, причём материал для подарка і придёт в день di.
Также Костя знает, что на изготовление подарка і нужно потратить с; дней. Костя трудолюбивый,
поэтому в один день может готовить любое число подарков (даже все).

Готовые подарки Костя планирует отправить почтой. Чтобы подарок і успел дойти до нового года, его
нужно отправить не позднее дня s1. Кроме того, на почте действует ограничение: можно отправлять
не больше одной посылки в один день.

Помогите Косте понять, успеет ли он приготовить и отправить все подарки так, чтобы они дошли до
получателей вовремя.

### Формат входных данных
В первой строке входных данных дано число п - число подарков, которое планирует приготовить
Костя (1 S n 105).

В следующих п строках дана информация про каждый из подарков. Описание подарка і состоит из
трех целых положительных чисел di, c; и s; - день, в который доставят материалы для изготовления
подарка, время, необходимое на приготовление подарка, и день, до которого должен быть отправлен
подарок, чтобы он успел дойти (1 di, ci, 8i 103).

### Формат выходных данных
Выведите «YES» (без кавычек), если Костя успеет приготовить и отправить все подарки вовремя, или
«NO» (без кавычек) в противном случае.

### Замечание
В первом тесте из условия Костя может отправить первый подарок в третий день, второй - в шестой
день, а третий - в пятый.

## Примеры данных
### Пример 1

    Ввод            Вывод
    3               Yes
    1 2 4
    3 2 8
    2 3 7

### Пример 2

    Ввод            Вывод
    4               No
    1 1 4
    1 1 4
    1 1 4
    1 1 4

### Пример 3

    Ввод            Вывод
    4               Yes
    1 2 4
    1 2 7
    2 2 4
    3 1 5