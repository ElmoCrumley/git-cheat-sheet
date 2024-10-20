## Git cheat sheet

### Регулярно используемые команды:
---
pwd - *показать путь к рабочей(текущей) папке(директории). Пример:* $ pwd
ls - *показать файлы и папки* *(флаг* -а *для скрытых файлов). Пример:* $ ls; $ ls -a
cd - *переместиться в указанную папку. Пример:* $ cd ~/folder/folder2; $ cd following_folder/folder/folder2
   - *переместиться на уровень выше. Пример:* $ cd ..
touch - *создать файл. Пример:* $ touch test.txt; $ touch README.md; $ touch test.txt README.md another_file.txt	
mkdir - *создать директорию (флаг -p для структуры). Пример:* $ mkdir folder; $ mkdir -p folder/folder2
mv - *переместить файлы и/или папки в указанную директорию. Пример:* $ mv file.txt following_folder/folder
cat - *прочитать файл (вывести содержимое в командной строке). Пример:* $ cat file.txt
rm - *удалить файл и/или директорию со всеми файлами в ней (удаление минуя корзину). Пример:* $ rm file.txt; $ rm -r folder
&& - *объеинение команд. Пример:* $ mkdir folder && cd folder && touch file.txt

### Часто используемые клавиши:
---
tab или tab+tab - *после частичного ввода команды или названия директории, дописывает за пользователя или выводит список доступных*
ctrl+insert - *скопировать из командной строки выделенное*
shift+insert - *вставить текст в командную строку*
↑, ↓ - *история введённых команд*

### Настройка и использование git и gitHub:
---
config - *внесение данных автора, вносящего данные.*
         *Пример:* $ git config --global user.name "Name"; $ git config --global user.email username@post.ru
init - *сделать текущую папку локальным(на компьютере) репозиторием. Пример:* $ git init
rm .git - *разгитить папку. Она перестанеть быть репозиторием. Пример:* $ rm -rf .git
     -r - *позволяет удалять папки вместе с их содержимым*
     -f - *программа не задаст уточняющие вопросы*
status - *проверка состояния репозитория. Пример:* $ git status
add - *передача текущих изменений в файл(ах)е в список изменений. Пример:* $ git add -all; $ git add file.txt
commit - *создание сущности из списка изменений в файл(ах)е (флаг -m оставляет сообщение). Пример:* $ git commit -m 'Мой первый коммит!'
log - *просмотр списка commit-ов (журнала записей). Пример:* $ git log

Чтобы не возникало ошибок при регистрации на сайте GitHub, лучше использовать почту @gmail.com
Repositories / New / Repository name / Create repository - создать репозиторий на сайте GitHub

ls - *проверка наличия ключей в текущей директории. Пример:* $ ls -la .ssh/
   - *если есть неопознанные ключи, лучше удалить*
ssh-keygen - *генерация SSH-пары ключей. Пример:* $ ssh-keygen -t ed25519 -C "электронная почта GitHub"
           - *при возникновении ошибки:* $ ssh-keygen -t rsa -b 4096 -C "электронная почта GitHub"
           - *далее указать место хранения ключей нажав enter, сохранив ~/, либо указать путь

Settings / SSH and GPG keys /  New SSH key 
    / Title(название ключа) / Key type (Authentication Key) 
    / Key (ключ из id_rsa.pub или id_ed25519.pub) / Add SSH key

ssh -T git@github.com - *проверка ключа (проверка ключа сайта GitHub "SHA256" по ссылке:* [ссылка](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/githubs-ssh-key-fingerprints)

Repositories / SSH / скопировать git@github.com:

remote - *привязка удалённого репозитория к локальному. Пример:* $ git remote add origin git@github.com:
       - *проверка связки репозиториев. Пример:* $ git remote -v
push - *загрузка содержимого локального репозитория на github. Пример:* $ git push -u origin main
     - *далее можно испльзовать просто git push. Пример:* $ git push







