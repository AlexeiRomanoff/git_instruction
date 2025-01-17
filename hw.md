# <center>**Команды Git**</center>

>Каждому разработчику необходим навык владения специализированным ПО по контролю версий. Git - одна из самых распростанненых программ для обеспечения упомянутого функционала. Рассмотрим несколько терминальных команд данного ПО.
<hr>

Для начала, установите установите на Ваш компьютер [VSCode](https://code.visualstudio.com/download). <br> он нам понадобиться для более удобной работы с Git. <br>

Ознакомьтесь с инструкцией по установке 
[Git](https://git-scm.com/book/ru/v2/Введение-Установка-Git) и установите Git на Ваш компьютер. <br>
Если возникнут сложности с установкой, используйте этот 
[видеоролик](https://yandex.ru/video/preview/11299384617156771124).<br>

<hr>

<center>Рассмотрим несколько терминальных команд, используемых в Git!

<u><b>Основные терминальные команды:</b></u></center>
* **git --version** - команда проверяет, верно ли настроен Git. Если выдала версию ПО, то все ОК;
* **git init** -  инициализирует выбранню папку в качестве репозитория;
* **git add filename.md** - добавляет файл для отслеживания изменений;
* **git log** - отображдает журнал сохранненых версий;
* **git commit -m "Your_comments_on_updates"** - делает для проекта снимок текущего состояния изменений, добавленных в раздел проиндексированных файлов. Команда может быть использована с дополнительным параметром **-m "..."**, что бы Вы могли оставить комментарий к изменениям;
* **git status** - проверяет текущее состояние репозитория, с её помощью можно убедиться, что команда *git add* добавила нужные изменения.
* **git diff** - представляет собой многоцелевую команду Git, которая инициирует функцию сравнения источников данных Git — коммитов, веток, файлов и т.д.;
* **git checkout** - позволяет переключаться между последними коммитами веток;
* **git checkout master (или main)** - возвращаемся к самой актуальной версии файла на текущий момент;
* **ls -hidden или ls -h** показывает скрытые каталоги в репозитории, в MAC применяется **ls -a**.

>> Мы рассмотрели с Вами лишь некоторые основные команды, которые широко используются для работы с функцией контроля версий. Рекомендуем Вам самостоятельно заниматься и изучать виды и типы команд, для повышения личных компетенций.

<hr>
<center><br><u><b>Работа с ветками Git:</b></u><br><br></center>

* **git branch** - покажет какие ветки есть и отметит (*) ту, на которой мы находимся сейчас;
* **git branch имя_ветки** - создает новую ветку;
* **git checkout -b имя_ветки**  - создает новую ветку и сразу перемещает в нее;
* **git checkout имя_ветки** - переключает нас на указанную ветку;
* **git log --graph** - покажет изменения в ветках;
* **git branch -D имя_ветки** - удалит указанную ветку.
* **git merge имя_ветки** - объединяет указанную ветку с той, в которой мы сейчас находимся (например с веткой "master").<br><br>

<hr>

<center><u><b><br>Работа с удаленным репозиторием:</b></u></center><br>

* **git remote add origin URL** - создает новое подключение к существующему по URL-адресу удаленному репозиторию (например на GitHub).<br><br>
* **git clone** - команда клонирования репозитория - используется для первоначального копирования репозитория, т.е. для создания копии на вашей машине, когда у вас вообще ничего нет - скачает всю информацию.<br><br>
* **git branch -M main** - переименовывает ветку master на локальном репозитории в main, что бы при выгрузке была синхронизация (с GitHub).<br><br>
* **git pull** - Эта команда позволяет скачать все 
из текущего репозитория и автоматически сделать merge с нашей версией.<br><br>
* **git push -u origin main** - отправляет (пушит) репозиторий с компьютера на удаленный. При первом её использовании нужна
авторизация. <br><u>Доп.параметры команды:</u><br>
_origin_ - имя удаленного репозитория;<br>
_main_ - это ветка удаленного репозитория;<br>
_-u_ - это ключ, который устанавливает связь с веткой main, указывается единожды.<br>

>>Fork - так называют клон-версию репозитория, в котором вносятся изменения. В дальнейшем их будут сравнивать с оригинальным.
**pull request** -команда в GitHub, которая отправит на рассмотрение автору репозитория те изменения, которые были внесены в версию Fork и выгружены с локального компьютера на удаленный Fork-репозиторий.

<hr>