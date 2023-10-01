# Отчет по лабораторной работе № 1
## по курсу "Фундаментальная информатика"


Студент группы М80-108Б-23 Ганяк Александр Олегович

Работа выполнена 

Преподаватель: каф. 806 Севастьянов Виктор Сергеевич

1. **Тема**: Git, Github, Gitlab etc
2. **Цель работы**: научиться работать с Git, GitLab, а также делать отчет
3. **Задание (вариант №<номер варианта если есть>)**:
    завести репозиторий (общий под все лабораторные работы с отдельной папкой под каждую лр!) 
    отчет с листингом в Markdown (листинг - ctrl+c -> ctrl+v из терминала с форматированием в markdown)
    создать отдельную ветку в репозитории под задание
    создать коммит с листингом и отчетом
    смержить ветку в мейн
5. **Идея, метод, алгоритм решения задачи**: Изучили git команды для терминала => выполнили все задания
6. **Сценарий выполнения работы**: 
    1. Открыли терминал
    2. создали репозиторий (общий под все лабораторные работы с отдельной папкой под каждую лр!)
    3. написали отчет с листингом в Markdown
    4. создали отдельную ветку в репозитории под задание
    5. создали коммит с листингом и отчетом
    6. смержили ветку в мейн                             
6. **Протокол**:
```
arts@LemonCorp:~$ git
использование: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>] [--config-env=<name>=<envvar>]
           <command> [<args>]

Стандартные команды Git используемые в различных ситуациях:

создание рабочей области (смотрите также: git help tutorial)
   clone     Клонирование репозитория в новый каталог
   init      Создание пустого репозитория Git или переинициализация существующего

работа с текущими изменениями (смотрите также: git help everyday)
   add       Добавление содержимого файла в индекс
   mv        Перемещение или переименование файла, каталога или символьной ссылки
   restore   Восстановление файлов в рабочем каталоге
   rm        Удаление файлов из рабочего каталога и индекса

просмотр истории и текущего состояния (смотрите также: git help revisions)
   bisect    Выполнение двоичного поиска коммита, который вносит ошибку
   diff      Вывод разницы между коммитами, коммитом и рабочим каталогом и т.д.
   grep      Вывод строк, соответствующих шаблону
   log       Вывод истории коммитов
   show      Вывод различных типов объектов
   status    Вывод состояния рабочего каталога

выращивание, маркировка и правка вашей общей истории
   branch    Вывод списка, создание или удаление веток
   commit    Запись изменений в репозиторий
   merge     Объединение одной или нескольких историй разработки вместе
   rebase    Повторное применение коммитов над верхушкой другой ветки
   reset     Сброс текущего состояния HEAD на указанное состояние
   switch    Переключение веток
   tag       Создание, вывод списка, удаление или проверка метки, подписанной с помощью GPG

совместная работа (смотрите также: git help workflows)
   fetch     Загрузка объектов и ссылок из другого репозитория
   pull      Извлечение изменений и объединение с другим репозиторием или локальной веткой
   push      Обновление внешних ссылок и связанных объектов

«git help -a» и «git help -g» выводит список доступных подкоманд
и небольшую справку по понятиям. Смотрите «git help <понятие>»
или «git help <термин>» чтобы узнать больше о конкретной подкоманде
или понятии.
Смотрите «git help git» для получения общего обзора системы.
arts@LemonCorp:~$ ls
 snap   Видео   Документы   Загрузки   Изображения   Музыка   Общедоступные  'Рабочий стол'   Шаблоны
arts@LemonCorp:~$ cd Документы
arts@LemonCorp:~/Документы$ ls
f1.txt  f1.txt~  herniya  LemOS
arts@LemonCorp:~/Документы$ mkdir labspython
arts@LemonCorp:~/Документы$ ls
f1.txt  f1.txt~  herniya  labspython  LemOS
arts@LemonCorp:~/Документы$ cd 
herniya/    labspython/ LemOS/      
arts@LemonCorp:~/Документы$ cd labspython/
arts@LemonCorp:~/Документы/labspython$ git init
подсказка: Using 'master' as the name for the initial branch. This default branch name
подсказка: is subject to change. To configure the initial branch name to use in all
подсказка: of your new repositories, which will suppress this warning, call:
подсказка: 
подсказка: 	git config --global init.defaultBranch <name>
подсказка: 
подсказка: Names commonly chosen instead of 'master' are 'main', 'trunk' and
подсказка: 'development'. The just-created branch can be renamed via this command:
подсказка: 
подсказка: 	git branch -m <name>
Инициализирован пустой репозиторий Git в /home/arts/Документы/labspython/.git/
arts@LemonCorp:~/Документы/labspython$ git add *
arts@LemonCorp:~/Документы/labspython$ git commit -m "first lol"
[master (корневой коммит) bde2180] first lol
 1 file changed, 26 insertions(+)
 create mode 100644 lab-report.md
arts@LemonCorp:~/Документы/labspython$ git push
fatal: Не настроена точка назначения для отправки.
Либо укажите URL с помощью командной строки, либо настройте внешний репозиторий с помощью

    git remote add <имя> <адрес>

а затем отправьте изменения с помощью имени внешнего репозитория

    git push <имя>

arts@LemonCorp:~/Документы/labspython$ git branch -m main
arts@LemonCorp:~/Документы/labspython$ git push https://github.com/plzZarbotay/labs-py-vyc
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream https://github.com/plzZarbotay/labs-py-vyc main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

arts@LemonCorp:~/Документы/labspython$ git push --set-upstream  https://github.com/plzZarbotay/labs-py-vyc main
Username for 'https://github.com': plzZarbotay
Password for 'https://plzZarbotay@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/plzZarbotay/labs-py-vyc/'
arts@LemonCorp:~/Документы/labspython$ git clone https://github.com/plzZarbotay/labs-py-vyc
Клонирование в «labs-py-vyc»...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Получение объектов: 100% (3/3), готово.
arts@LemonCorp:~/Документы/labspython$ ls
lab-report.md  labs-py-vyc
arts@LemonCorp:~/Документы/labspython$ cd 
.git/        labs-py-vyc/ 
arts@LemonCorp:~/Документы/labspython$ cd labs-py-vyc/
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git commit -m "first lol"
Текущая ветка: main
Эта ветка соответствует «origin/main».

Неотслеживаемые файлы:
  (используйте «git add <файл>...», чтобы добавить в то, что будет включено в коммит)
	lab-report.md

индекс пуст, но есть неотслеживаемые файлы
(используйте «git add», чтобы проиндексировать их)
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git init
Переинициализирован существующий репозиторий Git в /home/arts/Документы/labspython/labs-py-vyc/.git/
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git add *
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git commit -m "first lol"
[main 80c0528] first lol
 1 file changed, 26 insertions(+)
 create mode 100644 lab-report.md
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git push 
Username for 'https://github.com': ^C
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git remote set-url origin https://giu/plzZarbotay/labs-py-vyc.git
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git push 
fatal: «https://gcu/plzZarbotay/labs-py-vyc.git/» недоступно: Could not resolve host: giu
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git remote set-url origin https://giu@github.com/plzZarbotay/labs-py-vyc.git
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git push 
Перечисление объектов: 4, готово.
Подсчет объектов: 100% (4/4), готово.
При сжатии изменений используется до 16 потоков
Сжатие объектов: 100% (3/3), готово.
Запись объектов: 100% (3/3), 1.51 КиБ | 1.51 МиБ/с, готово.
Всего 3 (изменений 0), повторно использовано 0 (изменений 0), повторно использовано пакетов 0
To https://github.com/plzZarbotay/labs-py-vyc.git
   38b9314..80c0528  main -> main
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$  git branch for_labs
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git add *
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git commit -m "first lol"
Текущая ветка: main
Эта ветка соответствует «origin/main».

нечего коммитить, нет изменений в рабочем каталоге
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git checkout -b for_labs
fatal: a branch named 'for_labs' already exists
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git checkout  for_labs
Переключились на ветку «for_labs»
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git add *
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git add *
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git commit -m "first for labs"
[for_labs c95a1bc] first for labs
 1 file changed, 26 insertions(+)
 create mode 100644 1/lab-report.md
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git push 
fatal: The current branch for_labs has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin for_labs

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ git push --set-upstream origin for_labs
Перечисление объектов: 4, готово.
Подсчет объектов: 100% (4/4), готово.
При сжатии изменений используется до 16 потоков
Сжатие объектов: 100% (2/2), готово.
Запись объектов: 100% (3/3), 337 байтов | 337.00 КиБ/с, готово.
Всего 3 (изменений 0), повторно использовано 0 (изменений 0), повторно использовано пакетов 0
remote: 
remote: Create a pull request for 'for_labs' on GitHub by visiting:
remote:      https://github.com/plzZarbotay/labs-py-vyc/pull/new/for_labs
remote: 
To https://github.com/plzZarbotay/labs-py-vyc.git
 * [new branch]      for_labs -> for_labs
branch 'for_labs' set up to track 'origin/for_labs'.
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ кBAA^C
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ 



```
8. **Замечания автора** по существу работы: Все было ровно!
9. **Выводы**: Лабораторная работа, конечно, понравилась! Вспомнили еще раз, как работать с git. Отработали поэтапно каждый этап. git- это круто:!
