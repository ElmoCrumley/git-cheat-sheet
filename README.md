## Git cheat sheet

### Регулярно используемые команды:
pwd - *показать путь к рабочей(текущей) папке(директории). Пример:* $ pwd <br>
ls - *показать файлы и папки* *(флаг* -а *для скрытых файлов). Пример:* $ ls; $ ls -a <br>
cd - *переместиться в указанную папку. Пример:* $ cd ~/folder/folder2; $ cd following_folder/folder/folder2 <br>
cd - *переместиться на уровень выше. Пример:* $ cd .. <br>
touch - *создать файл. Пример:* $ touch test.txt; $ touch README.md; $ touch test.txt README.md another_file.txt <br>
mkdir - *создать директорию (флаг -p для структуры). Пример:* $ mkdir folder; $ mkdir -p folder/folder2 <br>
mv - *переместить файлы и/или папки в указанную директорию. Пример:* $ mv file.txt following_folder/folder <br>
cat - *прочитать файл (вывести содержимое в командной строке). Пример:* $ cat file.txt <br>
rm - *удалить файл и/или директорию со всеми файлами в ней (удаление минуя корзину). Пример:* $ rm file.txt; $ rm -r folder <br>
&& - *объеинение команд. Пример:* $ mkdir folder && cd folder && touch file.txt <br>

### Часто используемые клавиши:
tab или tab+tab - *после частичного ввода команды или названия директории, дописывает за пользователя или выводит список доступных* <br>
ctrl+insert - *скопировать из командной строки выделенное* <br>
shift+insert - *вставить текст в командную строку* <br>
↑, ↓ - *история введённых команд* <br>

### Настройка и использование git и gitHub:
config - *внесение данных автора, вносящего данные.* <br>*Пример:* $ git config --global user.name "Name"; $ git config --global user.email username@post.ru <br>
init - *сделать текущую папку локальным(на компьютере) репозиторием. Пример:* $ git init <br>
rm .git - *разгитить папку. Она перестанеть быть репозиторием. Пример:* $ rm -rf .git <br>
rm -r - *позволяет удалять папки вместе с их содержимым* <br>
rm -f - *программа не задаст уточняющие вопросы* <br>
status - *проверка состояния репозитория. Пример:* $ git status <br>
add - *передача текущих изменений в файл(ах)е в список изменений. Пример:* $ git add -all; $ git add file.txt <br>
commit - *создание сущности из списка изменений в файл(ах)е (флаг -m оставляет сообщение). Пример:* $ git commit -m 'Мой первый коммит!' <br>
log - *просмотр списка commit-ов (журнала записей). Пример:* $ git log <br>

Чтобы не возникало ошибок при регистрации на сайте GitHub, лучше использовать почту @gmail.com <br>
Repositories / New / Repository name / Create repository - создать репозиторий на сайте GitHub <br>

ls - *проверка наличия ключей в текущей директории. Пример:* $ ls -la .ssh/ <br>
ls - *если есть неопознанные ключи, лучше удалить* <br>
ssh-keygen - *генерация SSH-пары ключей. Пример:* $ ssh-keygen -t ed25519 -C "электронная почта GitHub" <br>
ssh-keygen - *при возникновении ошибки:* $ ssh-keygen -t rsa -b 4096 -C "электронная почта GitHub" <br>
ssh-keygen - *далее указать место хранения ключей нажав enter, сохранив ~/, либо указать путь <br>

Settings / SSH and GPG keys /  New SSH key / Title(название ключа) / Key type (Authentication Key) / Key (ключ из id_rsa.pub или id_ed25519.pub) / Add SSH key <br>

ssh -T git@github.com - *проверка ключа (проверка ключа сайта GitHub "SHA256" по ссылке:* [ссылка](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/githubs-ssh-key-fingerprints) <br>

Repositories / SSH / скопировать git@github.com: <br>

remote - *привязка удалённого репозитория к локальному. Пример:* $ git remote add origin git@github.com: <br>
remote - *проверка связки репозиториев. Пример:* $ git remote -v <br>
push - *загрузка содержимого локального репозитория на github. Пример:* $ git push -u origin main <br>
push - *далее можно испльзовать просто git push. Пример:* $ git push <br>

Дополнительная информация:

Хеш — идентификатор коммита. Хеширование - способ преобразовать набор данных, получить из этого "отпечаток". Свойства хэша: данные хэшируются одинаково; изменеие хэша сильное даже при незначительных изменениях.
Описание лога - хэш, автор, дата, сообщение.





