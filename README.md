# Скипты для правок электронного дневника школы

Скрипты из данного репозитория правят оценки, удаляют замечания и добавляют похвалу в электронном дневнике школы.

## Запуск

- Скачайте файл `scripts.py`.
- Из командной строки в директории электронного дневника - запустите shell командой `python manage.py shell`.
- Чтобы запустить скрипты можно его целиком скопировать в shell, а можно положить файл с кодом рядом с `manage.py` и подключить через import:
    - Откройте любым редактором файл `scripts.py` - скопируйте вcё содержимое в shell.
    - Либо скопируйте файл `scripts.py` в корень дневника рядом с `manage.py`, введите в shell команду `from scripts import *`.

## Использование скриптов

- Доступны 3 функции для ввода в shell, для каждой функции необходимо заполнить данные и запустить:
    - `fix_marks('Заполнить ФИО ученика')` - исправляет все плохие оценки заданного ученика на 5.
    - `remove_chastisements('Заполнить ФИО ученика')` - удаляет все замечания.
    - `create_commendation('Заполнить ФИО ученика', 'Заполнить название предмета')` - создаёт похвалу в последнем уроке без похвалы.    
