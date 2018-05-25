# market-form-flask
Интернет магазин на flask. Реализованы страницы отображения списка товаров и отображения информации о товаре. Может использоваться как прототип интернет магазина или в учебных целях.

## Структура проекта

 - **market-form-flask/market.py** - основной модуль, в котором описана обработка url
 - **market-form-flask/models.py** - модуль с описанием моделей ORM, в нём же инициализируется sqlalchemy
 - **market-form-flask/settings.py** - модуль, занимающийся разборкой конфига
 - **market-form-flask/create_example_base.py** - приложение, инициализирующее тестовую БД
 - **market-form-flask/template/** - шаблоны на jinja2
 - **market-form-flask/static/** - статика
 - **market-form-flask/static/images_product/** - изображения товаров (используется только для упрощения проекта, изображения лучше хранить на внешнем сервисе и обращаться к ним по url)
 - **market-form-flask/flask-market.conf** - пример конфигурационного файла (**ВАЖНО:** актуальный конфиг должен располагаться в **/etc/flask-market.conf**)


## Запуск


Для отладки можно пользоваться встроенным во flask http-сервером
```
python market.py
```
Однако при реальном использовании подумайте над запуске приложения через uwsgi.
