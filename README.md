# hm9
1.) Самый первый шаг, это мы удаляем пустые строчки. Я сделал это в 2 этапа. 
Первый: использовал регулярное выражение: (^\s*\n*\r) и заменил все вхождения на (\0).
![Этап 1](https://github.com/drozdovnikita/hm9/blob/master/1.png)
Второй: теперь я удаляю пробелы между строчками. Для этого я использовал регулярное выражение: (\n) и заменил на (\0).
![Этап 2](https://github.com/drozdovnikita/hm9/blob/master/2.png)
Таким образом я удалил все пустые строчки.

2.) Для того, чтобы найти всех князей и города, имя и название которых оканчивается на "слав" я использовал регулярное выражение: (^|\s)+[А-Я][а-я]*(слав) Всего упоминаний о князьях нашел: 471
![](https://github.com/drozdovnikita/hm9/blob/master/3.png)
3.) Для того, чтобы найти все упоминания Новгорода, я использовал регулярное выражение: (^|\s)+[Н][а-я]*(город) Всего упоминаний Новгорода нашел: 32
![](https://github.com/drozdovnikita/hm9/blob/master/4.png)
