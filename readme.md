# Git комманды

---

## Начальные настройки
`git init` - инициализация проекта

`git config --global user.email "you@example.com"` - указываем нашу почту в конфиге
`git config --global user.name "Your Name"` - указываем в конфиге имя

`git config --list` - выводит настройки из файла config 

`git remote add origin https://github.com/semyonlinkov/git-lessons.git` - привязывает к текущему проекту ссылку на гитхаб куда мы будем пушить коммиты под названием origin

`git add .` - меняет статус всех файлов в рабочей папке на Staged
`git branch -M main` - переименовывает master ветку в main
`git commit -m "first commit"` - создает коммит с сообщением (флаг -m) "first commit"
`git push -u origin main` - пушим проэет на удаленный репозиторий origin в ветку main

---