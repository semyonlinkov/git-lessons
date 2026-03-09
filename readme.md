## Git команды
### Начальные настройки
`git init` - создание репозитория  

`git config --global user.email "you@example.com"` - указываем нашу почту в конфиге  
`git config --global user.name "Your Name"` - указываем имя в конфиге  
> `--global` - флаг устанавливает значения для вей системы, так же есть флаги `--global` и `--local`

`git branch -M main` - переименовывает master ветку в main  

`git remote add origin https://github.com/semyonlinkov/git-lessons.git` - привязывает к текущему проекту ссылку на гитхаб куда мы будем пушить коммиты под названием origin  

`git config --list` - выводит настройки из файла всех вайлов config  
> `cat .git/config` - config файл в локальной директории  
> `cat ~/.gitconfig` - config в глобале  

`git config --global alias.c 'config --global'` - создаем простой алиас  
> `git c --list` - алиас команды `config --global`  
> `git config alias.test '!git ...; !git ...'` - создание наскольких алиасов вызываемых поочередно  

`git config -h` - показывает все опции команды config  
> `git help config` - более подробная информация о коммандах config  
---

### Создаем и пушим первый коммит
`git status` - показывает промежуточные состояния текущего проекта  
`git add .` - меняет статус всех файлов в рабочей папке на Staged  
`git reset HEAD .idea` - убирает из статуса stage каталог .idea  
> `git add -force .idea/project.iml` - игнорирует .gitignore (сокращенно флаг -f)  
`git commit -m "first commit"` - создает коммит с сообщением (флаг -m) "first commit"  
`git push -u origin main` - пушим проэет на удаленный репозиторий origin в ветку main  
> При последующих пушах можно иcпользовать короткую команду `git push`  

### Git show
`git show 75a8 --pretty=fuller` - комманда показывает данные коммита например автора коммита и коммитера (75a8 - не менее 4-х нач. символов id коммита или текущий коммит, если не указывать id)  
`git commit --author='John Doe <john@me.com>' --date='...'` - поменять автора коммита

