# Взаимодействие с API Evernote

Сервис предназначен для работы с приложением [Evernote](https://evernote.com). Для работы необходимо зарегистрироваться на сайте и запросить API Key.

## Как установить

1. Полученные после регистрации персональные данные присвоить переменным окружения в файле `.env`:

```python    
    EVERNOTE_CONSUMER_KEY = Ваш EVERNOTE_CONSUMER_KEY
    EVERNOTE_CONSUMER_SECRET = Ваш EVERNOTE_CONSUMER_SECRET
    EVERNOTE_PERSONAL_TOKEN - Ваш EVERNOTE_PERSONAL_TOKEN    
```
Python3 должен быть уже установлен.

2. Установить зависимости.
Используйте pip (или pip3, есть конфликт с Python2) для установки зависимостей:
```
pip install -r requirements.txt
```

### Как использовать

1. Файл add_note2journal.py - используется для добавления записей в журнал:
- получает данные пользователя Evernote и его записи;
- добавляет новую запись.

  Для запуска нужно указать дату в качестве аргумента:
```
python add_note2journal.py 'YYYY-MM-DD'
```

2. Файл dump_inbox.py - используется для вывода текста записей:
- получает данные пользователя Evernote;
- выводит текст его записей по заданному параметру - количество записей.

  Для запуска нужно указать количество записей в качестве аргумента:
```
python dump_inbox.py 'количество записей'
```

3. Файл list_notebooks.py - используется для вывода списка записей:
- получает данные пользователя Evernote;
- выводит список его записей.

  Запустить командой:
```
python list_notebooks.py
```

## Цель проекта
Код написан в образовательных целях на онлайн-курсе для веб-разработчиков https://dvmn.org
