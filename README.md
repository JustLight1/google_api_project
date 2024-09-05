<div align=center>
    
# Training Google API

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

</div>

## Описание проекта

Данный проект умеет:

1. Авторизовать приложение в сервисном аккаунте.
2. Создавать документы с таблицами на сервисном аккаунте.
3. Выдавать права доступа к созданным документам.
4. Читать содержимое таблиц.
5. Редактировать значения таблиц.
6. Получать список документов с гугл-диска сервисного аккаунта и фильтровать эти документы по типу.
7. Удалять документы с гугл-диска сервисного аккаунта.
8. Управлять приложением через аргументы командной строки.

## Технологии

- Python 3.10.11
- google-api-python-client 2.45.0

## Запуск проекта

1. Cклонировать проект:

```bash
git clone git@github.com:JustLight1/google_api_project.git
```

2. Создать виртуальное окружение и активировать:

```bash
python -m venv venv
source venv/Scripts/activate - windows
```

3. Установить библиотеки из файла requirements.txt:

```bash
pip install -r requirements.txt
```

4. Перейти в директорию travel_budget для дальнейшей работы:

```bash
cd travel_budget
```

5. Создать файл .env и заполнить его по примеру из файла .env.example

## Пример работы

Проект может работать в разных режимах с разными аргументами:

```bash
usage: main.py main.py [-h] [-c CREATE] [-cl] [-i ID] [-ls] [-u UPDATE]
options:
  -h, --help                    show this help message and exit
  -c CREATE, --create CREATE    Создать файл - введите "имя, бюджет"
  -cl, --clear_all              Удалить все spreadsheets
  -i ID, --id ID                Указать id spreadsheet
  -ls, --list                   Вывести все spreadsheets
  -u UPDATE, --update UPDATE    Обновить данные таблицы
```

1. Получить файлы:

```bash
python main.py -ls
```

2. Создать файл

```bash
python main.py -c "Греция, 70000"
```

3. Удалить все файлы

```bash
python main.py -cl
```

4. Обновить данные (дополнить) определенного файла

```bash
python main.py -i ID_таблицы -u "Транспорт, Билеты на самолёт, 2, 15000, =2*15000"
```

## Автор:

**Форов Александр**

[![Telegram Badge](https://img.shields.io/badge/-Light_88-blue?style=social&logo=telegram&link=https://t.me/Light_88)](https://t.me/Light_88) [![Gmail Badge](https://img.shields.io/badge/forov.py@gmail.com-c14438?style=flat&logo=Gmail&logoColor=white&link=mailto:forov.py@gmail.com)](mailto:forov.py@gmail.com)
