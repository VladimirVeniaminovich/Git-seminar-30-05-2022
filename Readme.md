# Инструкция по работе с git

## Подготовка репозитория
Для того, чтобы создать репозиторий используется команда *git init*. Для этого необходимо написать в терминале в папке будущего репозитория *git init*.
## Создание сохранений
Для создания сохранения необходимо использовать команду git commit. Для этого необходимо в терминале папки репозиторя написать ***git commit -m "подробное описание внесенных изменений".
## Добавление файла к коммиту
Для добавления файла к коммиту используется команда *git add*. Пишется она следующим образом *git add <имя файла>* в терминале в папке с созданным репозиторием
## Создание коммита
Для создания нового "сохранения" используется команда *git commit*. Используется она следующим образом: в терминале с папкой-репозиторием пишется *git commit -m <сообщение коммиту>*. Сообщение коммиту писать **ОБЯЗАТЕЛЬНО**!!!
## Перемещение между сохранениями
Для перемещения между сохранениями используется команда *git checkout*. Для того, чтобы переместиться на указанный коммит в терминале в папке с репозиторием пишем *git chechout <номер коммита>*. **Номер коммита** берется из журнала изменений, о котором сказано выше. После перемещения на указанный коммит мы попадаем в состояние *detached head*. Чтобы вернуться к обычной работе, необходимо написать *git checkout master*
## Журнал изменений
Для просмотра журнала изменений используется команда *git log*. Для этого в терминале в папке с репозиторием достаточно написать *git log*.
## Ветки в git
Ветки в git нужны, чтобы работать с "чистовиком" и "черновиками". Для того, чтобы создать новую ветку используется команда git branch. В терминале в папке с репозиторием, напишите git branch <название ветки>.
## Слияние веток и разрешение конфликтов
Для слияния двух веток используется команда git merge. Для её использования необходимо перейти в ту веку, куда Вы хотите сделать слияние, после чего в терминале в папке с репозиторием написать git merge <название сливаемой ветки>. Чаще всего слияние проиходит автоматически, но возможны КОНФЛИКТЫ. В таком случае, необходимо вручную получить желаемую версию файла и сделать коммит.
## Удаление веток
Для удаления ветки используется команда git branch -d. Для этого необходимо в папке с репозиторием в терминале написать git branch -d <название ветки>. Удаляемая ветка ОБЯЗАТЕЛЬНО должна быть СЛИТА.