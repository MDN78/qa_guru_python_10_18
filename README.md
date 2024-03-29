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

1. Установка poetry через `powershell` командой

```commandline
(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -
```

2. Далее надо прописать в windows в `PATH` путь к poetry, сохранить и закрыть терминал открыть новый
3. Посмотреть версию poetry коммандой `poetry --version`
4. Команда `poetry config --list` показывает настройки проекта
5. Чтобы виртуальная среда всегда формировалась в самом проекте - надо задать параметр командой  
   `poetry config virtualenvs.in-project true`

Команды:

```
poetry --version  
poetry new my-package - новый проект  
poetry shell - активация виртуального окружения  
poetry init  - инициализация текущего проекта  
poetry install - установка всего проекта и зависимостей
poetry add --dev pylint
poetry update - обновление проекта
poetry add requests pendulum - добавить пакет
poetry remove pendulum -  удаление зависимости
poetry show - 
poetry show --tree - 
poetry show pendulum` - указать установленные зависимости
```



После скачивания проекта на локальную машину, установка зависимостей командой `poetry install`  
Бывает после копирования проекта на локальную машину нужно указать путь до `poetry.exe` - PyCharm попросит сделать это  
   