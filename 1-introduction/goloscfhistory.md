# 🎯 golos.cf/history - Автономный, отказоустойчивый сервис для поиска, фильтрации и анализа любых событий в аккаунтах GOLOS/STEEM

Автор: [@vik](https://gpolos.io/@vik)

**Создан автономный инструмент для сканирования истории:**

### 📌[golos.cf/history](https://golos.cf/history/)

Его главное преимущество - автономность. Все вычисления происходят на стороне браузера, а значит вы можете просто скопировать html страницу и использовать ее даже если домен будет отключен.  
Опция выбора публичной ноды поможет переключаться между доступными нодами, в том числе использовать блокчейн STEEMIT

![](https://images.golos.io/DQmZ3WLeA1asMpHfn6diRxA2G36MUdjnUpa6rRhnCr5zQfc/Capture.PNG "golos.cf/history")

Приложение позволяет работать в нескольких режимах:

* Просмотр всей истории аккаунта
* Просмтор недавних операций
* Поиск недавних или всех операций содержащих ключевое слово \(в том числе наименование операций\)
* Поиск недавних или всех операций строго содержащих все указанные ключевые слова
* Поиск по множеству типов операций
 
  ![](https://images.golos.io/DQmdedKHLLXoWMSZBidyf24Rr6RhpV4vNYNzcaLFNpGmMRY/wide.gif "Опции golos.cf")

## Примеры использования

#### Поиск всех операций

[@ladyzarulem](https://golos.io/@ladyzarulem)как-то попросила меня рассказать о способе поиска авторских наград для аккаунта[@vp-liganovi4kov](https://golos.io/@vp-liganovi4kov)  
С помощью формы поиска это можно сделать так:

![](https://images.golos.io/DQmTdBFh1SmMhdfs2A7HE68GPKA3viCaHqL5EcwrccjzazT/2.PNG "2.PNG")

1. Указываем логин
2. Не указываем ключевые слова
3. Выбираем фильтр по операциям - Авторские награды
4. Отмечаем проверку всей истории

Поскольку выбрано сканирование всей истории аккаунта это займет некоторое время. Скорость обработки во многом зависит от скорости вашего соединения и мощности пк.  
![](https://images.golos.io/DQmeZHRb7oCXBhEVDxc5w1UAP1pdyob5Cg3nR4fXuHRYbzN/2.gif "2.gif")

Через 10-15 секунд мы получаем результаты

![](https://images.golos.io/DQmRTXArmEvBK3NonfZKWkghRxE37EwKL3bfEkqSfkHDN5J/3.PNG "3.PNG")

### Поиск определенной операции

Также задачу выше можно решить другим способом. Например нам нужно знать какая выплата была за пост`v-gostyakh-u-ligi-novichkov-avtor-lucisia-rasskazhet-o-tom-kak-dostich-postavlennykh-celei`

Заполним форму вот так:  
![](https://images.golos.io/DQmPKR63YZDcxMrxqLnzAtDpE6n6xLwXyVhyb3gNqUDfkBL/4.PNG "4.PNG")

Обратите внимание, что в поисковые запросы добавлен запрос`author_reward`и ссылка, а также отмечена опция`в операциях должны присутствовать все указанные ключевые слова`, в тоже время выбраны любые типы операций.  
Это значит, что во всех операциях аккаунта будут выбраны только авторские награды \(в них ключевое слово`author_reward`\) и содержащие ссылку на пост`v-gostyakh-u-ligi-novichkov-avtor-lucisia-rasskazhet-o-tom-kak-dostich-postavlennykh-celei`.

Нажимаем поиск - получаем искомую операцию:  
![](https://images.golos.io/DQmZH9ah2kbuTJ9ot5gzVgK2wd7LFFbVuu8mEMEiaxKAAwf/5.PNG "5.PNG")

Стоит понимать, что вместо`author_reward`и опции "Любые типы операций" можно было выбрать опцию "Авторские награды", но как альтернативный подход в ключевых словах можно использовать и наименование операций!

## Поиск платежей

Вчера antonkostroma просил найти меня его перевод для[@uplift](https://golos.io/@uplift), в мемо которого был значок`$`  
Как это можно сделать на примере формы:  
![](https://images.golos.io/DQmZoW1sEre31R9tyRzcn29iqVuEDppUCT7VzcdWY1BshCY/6.PNG "6.PNG")  
Поисковые запросы нужно вводить каждый с новой строки, мы ввели`uplift`и`$`, а также указали опцию`трансферы монет`.

Результат:  
![](https://images.golos.io/DQmeyqVAfaATUt757Bw5Swqhj5rp6aqGztYj5rondU2kLVZ/7.PNG "7.PNG")

### Поиск общих счетов на бирже

Популярный запрос, суть которого найти на[@bittrex](https://golos.io/@bittrex)все аккаунты с одинаковым memo, что будет значить, что средства с этих аккаунтов поступали на один и тот же счет на бирже.  
Пример использования:

Просканируем историю**insider**, выберем опцию`трансферы монет`и добавим ключевое слово`bittrex`  
![](https://images.golos.io/DQmPPEHbtsXKdqmWXP8xzfsFLUScZM6NiTfkzUrv9xq9o4e/8.PNG "8.PNG")

В результатах мы видим переводы на биржи с различиными memo  
![](https://images.golos.io/DQmVz1y9G8vm3Wi9k53RLq7YBab5hfuxJfwtHsXSzcb2xTd/9.PNG "9.PNG")  
Выберем одно из memo и снова откроем поиск по истории, но уже аккаунта**bittrex**

Логин**bittrex**поисковый запрос - memo которым пользуется**insider**, тип операций - трансферы монет.  
![](https://images.golos.io/DQmQuyEeg8k7DKkT1EfPBets9zYAcJCL4wKduwNWWjKu1bS/11.PNG "11.PNG")

В результатах мы увидим, что на этот счет в**bittrex**отправляли средства еще несколько аккаунтов на голосе  
![](https://images.golos.io/DQmb7giXqiCce9rVwEhj2RNFysfnbgPVYiQFKwA2hjiheUj/12.PNG "12.PNG")

---

#### Приведенные выше примеры лишь часть возможных комбинаций поиска и способов применения.

**Уверен форма будет полезна многим, поскольку отлично реализует функцию поиска операций выполнить которую вы так часто просили :\)**

---

Позднее будут добавлены:

* Стоп слова для исключения операций из поиска
  **\(✔️ Добавлено\)**
* Поиск по регулярным выражениям
* Версия с серверной акселерацией поиска
 
  Если у вас есть пожелания к функционалу - пишите в комментариях или в моем
  [**чате**](https://t.me/chain_cf)

---

## FAQ

> Вопрос: как найти все флаги выданные аккаунту?

Ответ:  
В поле поисковых запросов вводим

```
"author": "vik"
"weight": -

```

Отмечаем искать все слова  
Отмечаем поиск всех транзакций  
![](https://images.golos.io/DQmVHq257BuKJ5F5U57TZ3acsPCLswqMdrgSwqUnTAPu9im/image.png)

Жмем "поиск"...  
![](https://images.golos.io/DQmcHpDRyEbEqnkvGa3FwiiJMChtfuaWxUpCCGGD376neGZ/image.png)

---

Как видите - в операциях можно искать не только по словам, но и по фрагментам кода.`"weight": -`указан для поиска всех флагов. А чтобы найти например только 100%-ые, нужно вводить так:`"weight": -10000`



##### Добавлен новый функционал в[приложение для просмотра и поиска по истории аккаунтов - golos.cf/history](https://golos.io/ru--golos/@vik/golos-cf-history-avtonomnyi-otkazoustoichivyi-servis-dlya-poiska-filtracii-i-analiza-lyubykh-sobytii-v-akkauntakh-golos-steem)

### RAW содержимое блока

Нажмите на номер блока чтобы увидеть все его содержимое:  
![](https://images.golos.io/DQmf3G8eiGWTG8VJfAZLManwJamozrb79XgBrbzUvPTD5Yq/raw.gif "raw.gif")

### Возможность получить ссылку на отдельную транзакцию

У всех операций \(кроме виртуальных\) теперь есть прямая ссылка  
Это может быть полезно если вы хотите предъявить факты из транзакции другому пользователю.  
![](https://images.golos.io/DQmRgqTsYP9fzeXiPuXXxR472sfsgDQNuZLLykv7VdqMkUL/linktx.gif "linktx.gif")

### Формирование ссылки на поисковую комбинацию запросов

Если вам нужно часто проверять историю аккаунта на предмет каких-то определенных операций или нужно отправить ссылку с настроенным поисковым запросом другому пользователю - теперь это стало возможно!

Просто сформируйте свой запрос в форме  
Например я хочу посмотреть недавнее движение средств в моем аккаунте, но без переводов от[@robot](https://golos.io/@robot),[@dobrobot](https://golos.io/@dobrobot)и без мелких переводов`0.0**`монет  
Вбиваю логин vik, тип операций - трансферы монет, стоп слова:`"robot"`,`"dobrobot"`и`0.0`- поиск  
![](https://images.golos.io/DQmQJiGNWxyQzTkDf1DjGYFi4qk7yGdtww6PZezwoGyPU3f/2.gif "2.gif")

После этого в адресной строке сформировалась ссылка вида  
[https://golos.cf/history?login=vik&stop=](https://golos.cf/history?login=vik&stop=)"robot","dobrobot",0.0&keywords=&match=false&all=false&type=transfer  
ее можно использовать как закладку и открывать при необходимости проверить данные, либо передать другому пользователю, если хотите поделиться историей.

Перейдя по ссылке будет автоматически активирован поиск с учетом параметров в ней  
![](https://imgp.golos.io/0x0/https://s17.postimg.org/jvqqr8l3h/image.gif)

### Просмотр данных о постах \(Выплаты, апвоты\)

Если в истории аккаунта встречается операция комментария или поста - вы сможете открыть RAW данные и посмотреть выплаты, параметры, список апвотов и другие связанные с постом данные  
![](https://imgp.golos.io/0x0/https://s17.postimg.org/6dfpkfnlr/333.gif)

---

Напомню, что данная форма полностью автономна, работает на стороне браузера и ее можно использовать просто скопировав html.

В планах добавить "человеческие" описания к операциям для легкости восприятия данных широкой аудиторией.



> По материалам [статьи1](https://golos.io/ru--golos/@vik/golos-cf-history-avtonomnyi-otkazoustoichivyi-servis-dlya-poiska-filtracii-i-analiza-lyubykh-sobytii-v-akkauntakh-golos-steem) и [статьи2](https://golos.io/ru--golos/@vik/obnovlenie-golos-cf-history-novye-vozmozhnosti-dlya-poiska-i-analiza-istorii-akkauntov)
>
> Автор: @vik



