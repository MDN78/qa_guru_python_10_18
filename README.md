## Venv, Poetry и управление зависимостями проекта  
1. Поговорим подробнее о virtualenv и requirements.txt
2. Рассмотрим Poetry в качестве альтернативы, чем он лучше и какие задачи решает
3. Разберем файл pyproject.toml  

## Домашнее задание:  
Создайте проект, используя `poetry`. Заполните минимальную мета-информацию в `pyproject.toml`  
В зависимостях должны быть: `pytest`, `selene`  
В dev-зависимостях должен быть `pylint`  

## Справочная информация
[Документация по установке](https://python-poetry.org/docs/#installing-with-the-official-installer)  


Установка poetry через `powershell` командой   

(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -

Далее надо прописать в windows в PATH путь к poetry, сохранить

закрыть терминал открыть новый
далее можем посмотреть версию poetry коммандой 
poetry --version

команда poetry config --list показывает настройки проекта
чтобы виртуальная среда всегда формировалась в самом проекте - надо задать параметр командой
poetry config virtualenvs.in-project true




https://ru.hexlet.io/courses/python-setup-environment/lessons/start-with-poetry/theory_unit