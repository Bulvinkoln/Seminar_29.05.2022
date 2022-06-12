# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов

### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## Ветки в Git

### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"

## Удалённые репозитории

### Создание удалённого репозитория

Для того, чтобы создать удалённый репозиторий необходимо в своём аккаунте нажать *Repositories* далее *New*/ Присвоить имя репозиторию и нажать *Create repository*


### Клонирование репозитория

Делается со своего аккаунта. Необходимо выбрать репозиторий и нажать зелёную кнопку *Code*. Далее скопировать URL. Потом в терминале написать: *git clone "здесь должен быть скопированнный со своего аккаунта в github код"*

Далее при работе мы используем две команды: *git pull* и  *git push*.

*git push* отправляет изменения, которые мы произвели в нашем локальном репозитории, в удалённый.

*git pull* вытягивает изменения, которые произведены на удалённом репозитории в наш локальный репозиторий.


### pull request или как предложить свои изменения в чужой удалённый репозиторий


* Сначала заходим на github в репозиторий, которому мы решили помочь); 
* Нажимаем кнопку *Fork*. Программа создала нам копию этого репозитория в нашем аккаунте;
* Делаем *git clone* в терминале. Клонируется версия из нашего аккаунта. Первоначальный репозиторий остаётся без изменений;
* Создаем новую ветку и только в НЕЕ вносим свои изменения;
* Фиксируем изменения (делаем коммиты);
* Отправляем свою версию в свой аккаунт GitHub командой git push;
* На сайте GitHub нажимаем кнопку *pull request*.
Тем самым мы отправили в аккаун, которому хотели помочь, свою версию чего-либо, далее хозяин аккаунта может либо принять наше предложение, либо оставить свои репозиторий без нашей помощи).
