## Запуск проекта
Для запуска проекта нужно собрать Docker образ:
```docker build -t nto .```
После этого образ может быть запустить:
```docker run -p 8000:8000 nto```
Проект будет доступен по адресу  `http://127.0.0.1:8000`

"Салют банк" представляет собой сайт банка, на котором можно посмотреть данные о курсах валют, ключевой ставке Центробанка и акциях разных компаний в реальном времени.
Состоит проект из страниц: Главная, Курс Валют, Акции и Кредит. На первых трех содержатся интерактивные графики, которые можно изменять, настраивая временной период и частоты измений.
На странице "Кредит" находится форма для заполнения, которая отправляет запрос обученной модельке, и выдает в ответ возможность получения кредита человеком по введенным данным.
Также отдельно существует REST API, который позволяет просматривать, добавлять, изменять и удалять данные по картам в этом банке.
