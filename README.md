Веб-сайт интернет-магазина

Сайт включает каталог товаров с детальными описаниями, изображениями и ценами. Пользователи могут просматривать информацию о товарах, редактировать её, а также добавлять или удалять товары в зависимости от их уровня доступа.
Раздел с блогом позволяет публиковать статьи, а также редактировать и удалять их. Также настроен счётчик просмотров.
Для корректного функционирования приложения необходимо установить следующие зависимости:
[tool.poetry.dependencies]
python = "^3.12"
psycopg2-binary = "^2.9.9"
black = "^24.4.2"
pillow = "^10.3.0"
ipython = "^8.25.0"
articles = "^0.1.0"
article = "^0.1.1"
django = "4.2.2"
nullable = "^0.2.0"


Установка и запуск приложения
Для установки и запуска веб-сайта интернет-магазина выполните следующие шаги:

Клонируйте репозиторий:
git clone https://github.com/Altair-prog/d221v2.git

Перейдите в каталог проекта:
cd d221v2

Создайте виртуальное окружение и активируйте его:
python -m venv venv
source venv/bin/activate  # На Windows используйте: venv\Scripts\activate

Установите зависимости с помощью Poetry:
Убедитесь, что Poetry установлен. Если нет, установите его следуя инструкциям на официальном сайте Poetry.

Затем выполните:
poetry install

Выполните миграции базы данных:
python manage.py migrate

Запустите сервер разработки:
python manage.py runserver

После выполнения этих шагов приложение будет доступно по адресу http://localhost:8000
