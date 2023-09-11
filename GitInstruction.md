# Работа с Git
![картинка](/git.jpeg)
## 1. Проверка наличия установленного Git
В терминале выполнить команду `Git --version`. Если Git установлен, то появится сообщение с версией программы. Иначе появится сообщение об ошибке.
## 2. Установка Git 
Загружаем последнюю версию Git с [сайта](https://git-scm.com/downloads). Устанавлваем с настройками по умолчанию.
## 3. Настройка Git 
При первом использовании Git необходимо представится. Для этого нужно ввести в терминале две команды:
```Bash
git config --global user.name "Ваше имя"
git config --global user.email "Ваш email"
```

## 4. Подготовка репозитория
Подготовка репозитория происходит с помощью выделенной команды, указанной ниже :
```Bash
git init
```
## 5. Создание коммита 
Для добавления изменений в commit выполняется команда
```Bash
git add <имя файла>
```
Для того чтобы создать коммит необходимо выполнить команду
```Bash
git commit -am "описание коммита"
```
Для того чтобы посмотреть коммиты необходимо ввести одну из команд
```Bash
git log
git log --oneline
git log --graph
```

## 6. Показать изменения файла

Чтобы посмотреть разницу между последней версией сохраненного файла и файлом из последнего коммита необходимо выполнить команду
```Bash
git diff
```

## 7. Создание ветки, переключение между ветками , переключение между коммитами, слияние и удаление ветки 

Чтобы создать ветку необходимо выполнить команду
```Bash
git branch <name_of_branch>
```
Чтобы переключиться между ветками необходимо выполнить команду
```Bash
git switch <name_of_branch>
```
Чтобы переключиться между коммитами необходимо выполнить команду
```Bash
git checkout <hash_of_commit>
```

Для слияние веток необходимо выполнить команду
```Bash
git merge <ветку_которую_надо_слить_к_текущей>
```

Для удаление ненужной ветки необходимо выполнить команду
```Bash
git branch -d branch_name
```


## 8. Работа с удаленными репозиториями

Удаленный репозиторий можно скопировать себе на компьютер с помощью команды
```Bash
git clone <адрес_репозитория_не_обязательно_удаленного>
```

Для того, чтобы отправить изменения в удаленный репозиторий в существующую ветку необходимо выполнить команду
```Bash
git push 
```

Для получения изменений с удаленного репозитория и слияние с локальной версией  необходимо выполнить команду
```Bash
git pull 
```

***Если вдруг Вы хотите сделать вклад в чужой проект необходимо правильно работать с чужим удаленным репозиторием. Сначала делаем форк и копируем удаленный репозиторий себе на компьютер, создаем тематическую ветку, в которой делаем изменения и загружаем эту ветку на удаленный репозиторий, затем делаем Pull request и описываем подробно изменения в проекте, которые предлагаете внести.***

## 9. Литература

С.Чакон, Б.Штрауб - Git для профессионального программиста (2016)

[сайт](https://git-scm.com/book/ru/v2)
