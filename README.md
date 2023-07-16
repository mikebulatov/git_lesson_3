# Инструкция по работе Git
- ## Установка [git](https://git-scm.com/) и [Visual Studio Code](https://code.visualstudio.com/)
1. Установка git проводится коммандой: `sudo apt install git`
2. Установка Visual Studio Code проводится коммандой: `sudo apt install code`
- ## Настройка Visual Studio Code
1. Запускаем Visual Studio Code: *Нажимаем меню->програмирование->![icon](visual-studio-code.png)Visual Studio Code*
2. Русифицируем Visual Studio Code: *Открываем магазин расширений->ищем расширение "Russian language pack"> жмем кнопку "install"*
- ## Создание репозитория в git
1. Создаем каталог для репозитория
2. Запускаем Visual Studio Code и открываем в нем это каталог
3. Открываем Терминал в Visual Studio Code: *Нажимаем вид->Терминал*
4.  Запускаем комманду `git config --global user.email "you@example.com"` ___указав вместо you@example.com свой email___ затем комманду `git config --global user.name "Ваше Имя" ` ___указав всвоё имя вместо соотвесвующих слов___
5. Инициализируем каталог как репозиторий git коммандой: `git init`
6. Проверяем состояние репозитория коммандой: `git status`
7. Создаем файл проекта например "README.md" и добавляем его к отслеживаемым коммандой: `git add README.md`
8. Создаём первый (инициализационный) коммит(виксирование,сохранение) коммандой: `git commit -m "Описание коммита"` указав описание сохранения вместо соотвесвующих слов___
- ## Создание коммитов и сохранеие изменений файлов репозитория git
1. После изменеия любого файла или создании нового необходимо выполнять комманду: `git add filename`
2. После венсение и фиксации всех изменений создаем коомит коммандой: `git commit -m "Описание коммита"` указав описание сохранения вместо соотвесвующих слов___

- ## Переключени между коммитами в git
1. Для получения списка всех созданных коммпитов необходимо выплнить комманду: `git log` Если коммитов много то можно их вывести в кратком виде командой: `git log --oneline`
2. Чтобы перключится на нужный нам коммит необходимо выполняить комманду: `git checkout` указав после неё идентификатор коммиита(или первые 4 симовала идентификатора)
3. Чтобы вернутс в последний коммит необходимо выполняить комманду: `git checkout master`, master - это название текущей ветки
4. Альетнативное отображени всех коммитов и сияний веток выполняется коомандой: `git log --graph`

- ##  Исключения файлов из репозитория git
1. Создаём в репозитории файл с иминем `.gitignore`
2. Добавялем это файл к репозиторию коммандой: `.gitignore`
3. Записываем в файл `.gitignore` имена файлов для исключения в каждой строке отдельное имя файла


- ## Работа с Ветками в git

1. Для получения списка всех созданных веток необходмио выполнить комманду: `git branch` 
1. Для созданныия новой ветки необходмио выполнить комманду: `git branch` указав после неё название ветки
2. Чтобы перключится на нужную нам ветку необходимо выполняить комманду: `git checkout` указав после неё название ветки
3. Чтобы вернутс в последний коммит в ветке также нужно выполняить комманду: `git checkout` указав после неё название ветки 
4. Чтобы слить ветки нужно из основной веки выполняить комманду: `git merge ` указав после неё название вливаемой ветки
5. Чтобы удалить ветку  ветки нужно из основной веки выполняить комманду: `git branch -d ` указав после неё название удаляемой ветки
- ## Рубота с удаленными реозиториями



- ## Справочник комманд git

| Комманда | Описание | Пример исользования|
| ----------- | ----------- |----------- |
| git commit -m | зодание коммита |`git commit -m "комментарий"` |
| git diff | Просмотр изменений до коммита|`git diff` |
| git commit --amend -m  | Изменение последнего коммита |`git commit --amend -m "Uкомментарий"` |
| git init   | инициализация репозитория |`git init` |
| git add    | добавление файла к репозиторию  |`git add README.md` |
| git status | сосотояние репозитория |`git status` |