# Инструкция для работы с Git и удалёнными репозиториями

<!-- Warning! All changes are made in English. I guess they will be more distictive this way and also I'll be able to practice my English so. -->

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

## Rewriting the last commit
somtimes you realy need to rewrite the last commit without adding a new one
 
in order to rewrite it, use the attribute __--amend__ with the command __commit__ 

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием.

using the "*--oneline*" attribute with this command is **more** a convenient way of using it. 

## Ветки в Git

In easy words, GIT branch is the local copy of the main codebase which will have the changes of the new feature or bug fix, which will later be merged with the main codebase once after verified.

### Создание ветки

<center><image src="https://i.pinimg.com/originals/c7/d0/f9/c7d0f9e0b031d7f3b9dbf5eeb9ae3e28.png" alt="Git branching"> </center>

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Branch switching

to switch between branches use git switch "name branch"


<center><image src="https://res.cloudinary.com/practicaldev/image/fetch/s--pFnrRUS---/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://thepracticaldev.s3.amazonaws.com/i/4ydntxifxpmmcxjyjyxr.png" > GIT Switching </center>

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"

# Synchronization to GitHub

## git clone

to download existing repository, *git clone* command is used

Example: *git clone __GitHub link__* 

It'll download a pointed repo to your folder

## git pull

This command downloads all changes to your repo and tries to merge them

## git push 

This command uploads your repo version to remoute repo

**! requires the authorisation at first using!*

## pull request

This command is to suggest changes to existing project of another author

 All changes should be suggested through another new branch: 
* do "fork" for the repo
* git clone of YOUR repo version
* create a new branch and change it
* commit changes
* upload it to your GitHub
* on GitHub site push "pull request" button. 


## to push a new branch to the existing git project special attributes should be used

the command is  __"git push --set-upstream origin (current branch name)"__  