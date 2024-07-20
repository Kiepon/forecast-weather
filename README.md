# 

Прогноз погоды

Реализовал следующее:

Приложение, он же сайт, который может спрогнозировать погоду введенного города в формочку.

Для создания этого сайта я использовал ЯП Python на его фреймворке Django, подключил API ключи Яндекса и сервиса dadata, но о нем чуть позже.
Ключи яндекса были необходимы для поиска данных прогноза погоды в определенном регионе.
Вводя в поле формы название города и нажатию кнопки я получаю прогноз на 7 дней.

Из дополнительного - я реализовал автодополнение с использованием API ключа сервиса dadata.ru
Он позволяет по минимально введенным данным в поле отобразить какое-то значение, которое, возможно, хотел ввести пользователь.


Запуск проекта

Инструкция предназначена для windows и git bash и windows<br/>

1. Клонируйте репозиторий и откройте его в любом удобном для вас редакторе:

```
git clone https://github.com/Kiepon/forecast-weather.git
```

2. Установите виртуальное окружение:
```

Git bash:

python -m venv your_venv

Windows:

python -m venv your_venv
``` 

3. Активируйте виртуальное окружение:
```
Git bash:
source venv/Scripts/activate

Windows:
your_venv/Scripts/activate

```

4. Установите зависимости из файла requirements.txt:
```

Windows and git bash:
pip install -r requirements.txt
```

4. Сделайте миграции:
```

Git bash and windows:
python manage.py migrate
```

5. Используйте команду createsuperuser для создания администратора в админ панели:
```

git bash and windows:
python manage.py createsuperuser
```

6. В папке с файлом manage.py запустите сервер, выполнив команду:
```
python manage.py runserver
```
