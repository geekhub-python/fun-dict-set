## Задание 1

Напишите функцию sum_finder(sum=10), которая из произвольного входящего массива выберет все уникальные комбинации чисел, сумма которых равна sum.

Примеры:

```
In: sum_finder(7, 10, 2, 5, 3, sum=10 )  
Out: [( 10 ), ( 3, 7 ), ( 2, 3, 5 )]

In: sum_finder(7, 10, 2, 5, 3, 1, sum=10 )
Out:  [ ( 10 ), ( 3, 7 ), ( 2, 3, 5 ), ( 1, 2, 7 ) ]

In: sum_finder( 7, 10, 2, 5, 3, 3, sum=10 )
Out: [ ( 10 ), ( 3, 7 ), ( 2, 3, 5 ) ]

In: sum_finder(6, sum=10)
Out: [ ]
	
```

## Задание 2

Создайте латинско-английского словарь из англо-латинского.

Напишите функцию invert_vocabulary которая принимет произвольное количество описаний. В каждое описание записано сначала английское слово, затем отделённый пробелами дефис, затем разделённые запятыми с пробелами переводы этого английского слова на латинский. Все слова состоят только из маленьких латинских букв. Переводы отсортированы в лексикографическом порядке. Порядок следования английских слов в словаре также лексикографический.

Выведите соответствующий данному латинско-английский словарь, в точности соблюдая формат входных данных. В частности, первым должен идти перевод лексикографически минимального латинского слова, далее — второго в этом порядке и т.д. Внутри перевода английские слова должны быть также отсортированы лексикографически.


```
In: invert_vocabulary("apple - malum, pomum, popula", "fruit - baca, bacca, popum", "punishment - malum, multa")

Out: 
baca - fruit
bacca - fruit
malum - apple, punishment
multa - punishment
pomum - apple
popula - apple
popum - fruit

In: invert_vocabulary("school - schola")

Out: 
schola - school

In: invert_vocabulary("greet - empfangen, willkommen", "silicon - silicon", "welcome - willkommen")

Out:
empfangen - greet
silicon - silicon
willkommen - greet, welcome


In: invert_vocabulary("drxpeycnkp - fgoezltv, fgqedltc, fgqezltc, fsqezltc, tgqehltc", "oaxpeycnkp - fgqedltc, pgqezltu, tgqehltc", "yaxpefcnkr - fgqedltc, fgqezljc, fgqezlqc, fgqezltc, tgqehltc", "yaxpeycnkp - fgqedltc, fgqezlqc, fsqezltc", "yaxpeycnks - fgqedltc, fsqezltc, pgqezltu", "yaxteyckp - fgqedltc, fgqezljc, fgqezlqc, fsqezltc, pgqezltu")

Out: 
fgoezltv - drxpeycnkp
fgqedltc - drxpeycnkp, oaxpeycnkp, yaxpefcnkr, yaxpeycnkp, yaxpeycnks, yaxteyckp
fgqezljc - yaxpefcnkr, yaxteyckp
fgqezlqc - yaxpefcnkr, yaxpeycnkp, yaxteyckp
fgqezltc - drxpeycnkp, yaxpefcnkr
fsqezltc - drxpeycnkp, yaxpeycnkp, yaxpeycnks, yaxteyckp
pgqezltu - oaxpeycnkp, yaxpeycnks, yaxteyckp
tgqehltc - drxpeycnkp, oaxpeycnkp, yaxpefcnkr

```
