## Ошибка программы расчета бонуса при использовании данных типа double ##

Проверена функциональность программы, разрабатанной на языке JAVA, и используемой для расчета бонуса новым клиентам.
Ссылка на программу: https://github.com/vovaanik/JAVA-DZ-2-2-code/blob/master/Main.java

## В работе программы выявлена ошибка, составлен баг-репорт. ##

1. Описываемая программа запускалась в оболочке JetBrains\IntelliJ IDEA Community Edition 2020.2.
2. Действия проводились с переменными класса " double ".
3. Проводилось позитивное функциональное тестирование на соответствие ожидаемого результата реальному.
4. Тестировалась функция расчета бонуса с использованием оператора "+", а именно:

К переменной класса double со значением 0.3 с помощью оператора "+" добавлялась переменная класса double со значением 0.6. 
* Вместо ОЖИДАЕМОГО РЕЗУЛЬТАТА: 0.9 получился ФАКТИЧЕСКИЙ РЕЗУЛЬТАТ: 0.8999999999999999. 

* Таким образом, в данной программе обнаружен БАГ, на что составлен соответствующий баг-репорт.
* Ссылка на баг-репорт: https://github.com/vovaanik/JAVA-2-2-Newest/issues/1

### ВЫВОД: в коде программы необходимо устранить ошибку, приводящую к расхождению в количестве знаков после запятой. ###

Тестирование производилось в следующем окружении:

WINDOWS 10 x 64 

Java jdk-11.0.8.10

IntelliJ IDEA Community Edition 2020.2

GIT Version 2.28.0
