## Основные команды при использовании GIT

> **git init** - *инициализация локального репозитория*

> **git checkout** - *переход от одного коммита к другому*

> **git status** - *получение информации от git о значении текущего состояния*

> **git add -a** *-автоматическое добавление к отслеживанию данного файла*

> **git log** *-Посмотреть журнал изменений*

> **git commit -m “message”** *-создание коммита*

> **git checkout master** *- вернуться к актуальному состоянию и продолжить работу*

> **git diff** *-увидеть разницу между текущим файлом и закоммиченным файлом*

## Основные команды второго семинара по Git

>**git branch <название ветки>** - *создать новую ветку*

>**git log --oneline --**- *коротенький журнал*

>**git merge --abort**- *отменить слияние, которое прошло с конфликтом*

>**git checkout -b deleting_info** - *создаёт новую ветку и переходит на неё*

>**git branch -d <название ветки>** – *удалить ветку*

>**git commit -am “message”** – *добавление файлов в отслеживание и создание коммита*

>**git mv text.txt test_new.txt** - *переименовывание файла «text.txt» в «test_new.txt» и проиндексировать это изменение*

>**git branch -r** - *показывает удаленные ветки*

>**git branch lost_branch <№последнего коммита>** - *создает новую ветку от указанного коммита в текущей ветке*

>**git commit --amend -c <commit ID>** - 
*данная команда поможет изменить имя других коммитов*

>**git commit --amend -m "Новое название коммита"** - *для того что бы изменить имя последнего коммита*

>**git merge bugFix** - *помогает влить в активную ветку изменения из ветки featurebugFix*
![Merge](Merge.svg)

>**git archive -o ./project.zip HEAD** - *создать архив с файловой структурой проекта по указанному пути (состояние репозитория, соответствующее указателю HEAD)

## Основные команды 3 семинара по Git 

>**git clone** - *Клонирует репозиторий с гитхаба в локальный репозиторий по ссылке*

>**git pull** - *для извлечения и загрузки содержимого из удаленного репозитория и немедленного обновления локального репозитория этим содержимым*

>**git fetch** - *загружает коммиты, файлы и ссылки из удаленного репозитория в ваш локальный репозиторий*

>**git push**- *используется для выгрузки содержимого локального репозитория в удаленный репозиторий. Она позволяет передать коммиты из локального репозитория в удаленный, эта команда симметрична команде git fetch*

## Дополнительные команды для работы с Git 

>**git reset** - *отменяет изменения, перенося ссылку на ветку назад, на более старый коммит. Это своего рода "переписывание истории". git reset перенесёт ветку назад, как будто некоторых коммитов вовсе и не было.*
![Reset](Reset.svg)

>**git rm** - *удаляет файл из отслеживания в репозитории*

>**git revert** - *Чтобы отменить изменения и поделиться отменёнными изменениями с остальными, надо использовать git revert*
>>*Reset отлично работает на локальных ветках, в локальных репозиториях. Но этот метод переписывания истории не сработает на удалённых ветках, которые используют другие пользователи*
![Revert](Revert.svg)

>**git rebase [name]** - *копирует набор коммитов и переносит их в другое место. Преимущество rebase в том, что c его помощью можно делать чистые и красивые линейные последовательности коммитов. История коммитов будет чище, если вы применяете rebase*
![Rebase](Rebase.svg.svg)

>**git cherry-pick C2 C4** - *это очень простой и прямолинейный способ сказать, что ты хочешь копировать несколько коммитов на место, где сейчас находишься (HEAD)*
![Cherry-pick](Cherry-pick1.svg)
![Cherry-pick](Cherry-pick2.svg)

>**git rebase -i [name]** - *git cherry-pick применяется, когда точно известно, какие коммиты нужны (и известны их точные хеши). Но, в случае, когда точно не известно какие коммиты нужны можно использовать интерактивный rebase — лучший способ отобрать набор коммитов для rebase*
![-i Rebase](iRebase1.svg)
![-i Rebase](iRebase2.svg)
