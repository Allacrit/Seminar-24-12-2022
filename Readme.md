# Инструкция по работе с Git.

## Что такое Git?

**Git** - это наиболее популярная реализация распределённой системы контроля версий. Самая популярная реализация **Git** - это [GitHub.](https://github.com/)

## Подготовка репозитория.
Для создания репозитория используется команда *git init*. Для этого необходимо в терминале перейти в пустую папку, где в будущем будет репозиторий. Затем в терминале с папкой написать команду *git init*. 

## Создание коммитов.

### Добавление файла к коммиту.
Для добавления файла к будущему коммиту используется команда *git add*. Для этого в терминале с папкой-репозиторием необходимо написать *git add <название файла>*.

### Создание коммита.
Для создания коммита используется команда *git commit*. Для этого в терминале с папкой-репозиторием необходимо написать *git commit <сообщение к коммиту>*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО!! И в ковычках!!!***. 

## Журнал изменений.
Для просмотра журнала изменений используется команда *git log*. Для этого в терминале с папкой-репозиторием необходимо написать *git log*.

## Перемещение между коммитами.
Для перемещения на предыдущие коммиты используется команда *git checkout*. Для этого необходимо в журнале изменений, как показано в предыдущей части, найти необходимый коммит и его номер. После чего в терминале с папкой-репозиторием написать команду *git checkout <номер коммита>*.
После применения этой команды Вы попадёте в состояние *Detached head*, в котором никакие измениения фиксироваться не будут. Для возврата в обычное состояние необходимо написать команду *git checkout master*.

## Ветки в Git.
Во время разработки новой функциональности считается хорошей практикой работать с копией оригинального проекта, которую называют веткой. Ветви имеют свою собственную историю и изолированные друг от друга изменения до тех пор, пока вы не решаете слить изменения вместе.

### Создание веток.
Для создания новой ветки используется команда *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать *git branch <название ветки>*.

### Перемещение между ветками.
Для перехода на другую ветку используется команда *git checkout*. Для этого в терминале с папкой-репозиторием необходимо написать *git checkout <название ветки>*. Для перехода на ветку, ветка должна быть ***создана***!!!

## Слияние веток и разрешение конфликтов.

### Слияние веток.
Для слияния веток используется команда *git merge*. Для этого в терминале с папкой-репозиторием необходимо написать *git merge <название ветки которую сливаем>. При этом необходимо находится в ветке в которой происходит слияние.

### Разрешение конфликтов.
При слиянии веток может возникнуть конфликт слияния, если были произведены изменения в двух слияемых ветках. Перед вами будет стоять выбор: Принять поступившие изменения, Оставить "старую" информацию, Принять обя варианта. Самым правильным будет принять оба варианта, выполнить корректировку после слияния веток, добавить в систему контроля версий данный файл и выполнить создание коммита.

## Удаление веток.
Для удаления веток используется команда *git branch -d*. Для этого в терминале с папкой-репозиторием необходимо написать *git branch -d <название ветки>*.
