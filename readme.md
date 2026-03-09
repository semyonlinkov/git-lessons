## Git комманды
### Начальные настройки
`git init` - инициализация проекта<br/>

`git config --global user.email "you@example.com"` - указываем нашу почту в конфиге<br/>
`git config --global user.name "Your Name"` - указываем имя в конфиге

`git branch -M main` - переименовывает master ветку в main<br/>

`git remote add origin https://github.com/semyonlinkov/git-lessons.git` - привязывает к текущему проекту ссылку на гитхаб куда мы будем пушить коммиты под названием origin<br/>

`git config --list` - выводит настройки из файла config<br/>

---

### Пушим коммит
`git add .` - меняет статус всех файлов в рабочей папке на Staged<br/>
`git commit -m "first commit"` - создает коммит с сообщением (флаг -m) "first commit"<br/>
`git push -u origin main` - пушим проэет на удаленный репозиторий origin в ветку main<br/>
 > В последующем можно иcпользовать короткую команду `git push`

---