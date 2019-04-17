## ✨ Лаба 4. Суперачивка. Спрогнозировать отток клиентов банка по историческим данным (увеличенная точность)

##### [![New Professions Lab — Big Data 9](extra/images/npl7.svg)](https://github.com/newprolab/content_bigdata9)

### Дедлайн

⏰ Четверг, 25 апреля 2019 года, 23:59.

### Задача

В [Лабе 4](lab04.md) `ROC AUC = 0.75` не должен был вызвать проблем. Давайте немного усложним задачу, увеличив этот порог. «Немного» — потому что и новый порог — не максимально возможный, а мы не хотим устраивать из этой лабы чемпионат.

Изначально, этот датасет был представлен как задача для одного из хакатонов по анализу данных. Один из участников сообщил, что AUC = 0.83 достигается тоже быстро, а вот дальше начинается работа. Хороший результат — выше 0.85. В нашем случае, у нас нет скрытого тестового сета, поэтому вы, наверняка, переобучитесь и сможете показать даже и более высокий score. Но, всё-таки, если получите его — напишите в #labs в слаке :)

**Новый порог: получите ROC AUC не ниже 0.83.**

### Обработка данных на вход

Вам понадобится тот же датасет, что и в [Лабе 4](lab04.md). Напомним:

* `lab04_train.csv` — тренировочная выборка с известными значениями оттока.
* `lab04_test.csv` — проверочная выборка, вероятности оттока для которой вам и надо предсказать.

### Обработка данных на выход

Выходной файл должен быть расположен в корне вашей домашней директории в файле `lab04s.csv` (обратите внимание на `s`). Файл должен содержать два поля, разделённых табом, а также шапку: `id	target`.

* Поле `id` — идентично тому, что представлено в `laba04_test.csv`.
* Поле `target` — **вероятность** оттока в пределах `[0, 1]`.

**Для успешного выполнения ачивки вы должны получить ROC AUC не меньше 0.83.**

### Проверка

Проверка осуществляется [автоматическим скриптом](http://lk.newprolab.com/lab/laba04s) из Личного кабинета.