# Инструкция по работе с Git

## Что такое Git?
*Git* - одна из реализации распределенных систем контроля версий, позволяющая организовать версионность, как локально, так и на удаленном сервере. Самая популярная платформа, реализующая *Git* - [GitHub](https://github.com)

## Подготовка репозитория
Для создание в папке репозитория, необходимо открыть эту папку в терминале и написать команду *git init*, после чего в этой папке создастся скрытая папка *.git*, и таким образом папка станет репозиторием

## Создание коммитов

### Просмотр состояния репозитория
Для просмотра состояния репозитория используется команда *git status*. В терминале с открытой папкой-репозиторием необходимо написать команду *git status*. В результате можно увидеть следующие выводы:
1. On branch *** nothing to commit - это означает нет активных изменений
2. Untracked file - это означает, что имеются файлы, не отслеживаемые системой контроля версий
...

### Добавление файла к коммиту
Для того, чтобы добавить файл к "сохранению", необходимо использовать команду *git add*. В терминале с открытой папкой-репозиторием необходимо написать *git add <название файла>*, и этот файл добавится к "сохранению"

### Создание фиксации
Для создания фиксации используется команда *git commit*. Для этого в терминале с папкой-репозиторием необходимо написать команду *git commit -m <сообщение к коммиту>*. Сообщение к коммиту писать **Обязательно**.

## Журнал изменений
Для просмотра историй изменений используется команда *git Log*. Для этого в терминале с папкой-репозиторием необходимо написать *git Log*, и Вы увидите список всех коммитов в этой веткек с описанием: имени, электронной почты, сообщением к коммиту и номер коммита.

## Перемещения между коммитами
Для перемещения между коммитами используется команда *git checkout*. Для этого в терминале с папкой-репозиторием необходимо написать *git checkout <номер коммита>*. Номер коммита берется из журнала изменений ветки.

## Ветки в git

## Слияние веток и решение конфликтов
Для того, чтобы слить ветки в одну, необходимо перейти в ветку, в которую хотите перенести изменения и использовать команду *git merge <название ветки из которой хотите перенести изменения>*. При слиянии веток может возникнуть конфликт, который необходимо исправить вручную, *добавить файл к коммиту* и *зафиксировать изменения*.

## Удаление веток