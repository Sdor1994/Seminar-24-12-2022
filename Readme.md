# Инструкции по работе с Git

## Что такое Git?
**Git** - это наиболее популярная реализация распределенной сиситемы контроля версий. Самая популярная реализация "Git"- это [GitHub](https://github.com/)

## Подготовка репозитория
Для инициализации репозитория нам необходимо открыть зарание созданную пустую папку в программе и прописать в терминале команду "git init". после этого Git начнет отслеживать все изменения в данной папке. 
 
## Создания "коммитов"
### Добваление файла к коммиту
Для добавления файла к будущему коммиту используется команда "git add". Для этого в термирнале с папкой необходимо написать "git add <название файла>".

## Создания "коммита"
Для создания коммита используеться команда 'git commit". Для этого в терминале с папкой репозиторием необходимо написать "git commit -m <сообщение к коммиту>". Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО!!!***.

## Журнал изменений
Для просмотра журнала изменений используеться команта "git log". Для этого в терминале с папкой-репозиторием необходимо написать "git log".

## Перемещение между коммитов
Для перемещения на предыдущие коммиты используется команда "git checkout". Для этого необходимо в журнале изменений, как показано в предыдущей части, найти необходимо коммит и его номер. После чего в терминале с папкой-репозиторием написать команду "git checkout <номер коммита>". После применения этой команды Вы попадете в состояние **Detached head*, в котором никакие изменения фиксироваться не будут. Для возврата в обычное состояние необходимо написать команду "git checkout master".

## Ветки в Git
Имя основной ветки Git-проекта по умолчанию — master. Находясь на основной ветке мы создаем ответвление с помощью команды "git branch <НазваниеВетки>". После чего для продолжения работы на вновь созданой ветке нам необходимо, перейти на нее при помощи команды "git checkout <НазваниеВетки>".

## Слияние Fork и разрешение конфликтов
Для слияния текущей ветки с какой-либо другой используется команда
"git merge имя_ветки".
В результате выполнения этой команды в текущей ветке появится новый коммит. Этот коммит будет иметь два предка – последние коммиты обоих веток, участвующих в слиянии. Содержимое этого коммита будет включать содержимое коммитов обоих веток.

## Удаление Fork
Для удаления веток необходимо воспользоваться командой Git branch -d <НазваниеВетки>.

