## Семинарские занятия по теме git
_____

Цель: Нам нужно смержить ветки, выполнив следующие команды:

```
git init

git add .

git commit -m " test this app"

git remote add origin https://github.com/username/0-git-basic.git

git push  origin master


git branch hello

git checkout hello

git add .

git commit -m " add hello to hello"

git push  origin hello

git checkout master

git merge hello

git push  origin master
```

Создаем каталог на компьютере где будет лежать наш проект
 - ![image](img/1.png)

 Создаем файл README.md
 - ![image](img/2.png)

Заполняем файл рандомным текстом, чтобы он не был пустым

 - ![image](img/3.png)

 Сохраняем файл, иначе пустой файл не запушится в репозиторий
 - ![image](img/4.png)
 
 
 Коммитим изменения

 Равносильно двум подряд командам 
       git add
       git commit

 - ![image](img/-2024-02-07_17-43-59.png)

 - ![image](img/-2024-02-07_17-44-26.png)

 - ![image](img/-2024-02-07_17-44-57.png)
 - ![image](img/-2024-02-07_17-45-22.png)
 - ![image](img/-2024-02-07_17-47-11.png)

 Пушим в репозиторий (если до этого настроили github в vscode)
 - ![image](img/-2024-02-07_17-47-40.png)
 - ![image](img/-2024-02-07_17-49-29.png)
  
  Если vscode не настроен, то список репозиториев будет недоступен.

 - ![image](img/-2024-02-07_17-58-31.png)

  Тогда идём создавать репозиторий вручную на сайт githib.com
 - ![image](img/-2024-02-07_18-21-05.png)
 - ![image](img/-2024-02-07_18-21-25.png)


 - ![image](img/-2024-02-07_18-21-55.png)
 - ![image](img/-2024-02-07_18-22-29.png)
  
  Теперь выбираем из списка только что созданный репозиторий 
  
  
  
 В строке должны увидеть список своих репозиториев.
  Если списка нет, то настраиваем аутентификацию с github

  ```
  git config --global user.name "vladimir"
  git config --global user.email "email@address.com"
  ```

  и пушим в него


 - ![image](img/-2024-02-07_18-23-11.png)

Идём смотреть, что получилось. Обращаем внимание на ветку master
 - ![image](img/-2024-02-07_18-25-23.png)

Создаем файл hello.py
 - ![image](img/-2024-02-07_18-28-22.png)
 Создаем новую ветку (git branch hello), переключаемся на неё (git checkout hello) 
 - ![image](img/-2024-02-07_18-30-15.png)
 Пушим изменения в репозиторий ветку hello , наблюдаем что там на github
 - ![image](img/-2024-02-07_18-31-33.png)
 - ![image](img/-2024-02-07_18-31-53.png)
 - ![image](img/-2024-02-07_18-32-17.png)
 Переключаемся в ветку master (git checkout master)
 - ![image](img/-2024-02-07_18-32-59.png)
 - ![image](img/-2024-02-07_18-33-26.png)
 Сливаем ветку hello в master
 - ![image](img/-2024-02-07_18-34-03.png)


 - ![image](img/-2024-02-07_18-34-40.png)
 Пушим изменения ветки master
 - ![image](img/-2024-02-07_18-35-06.png)
 - ![image](img/-2024-02-07_18-35-27.png)
 Смотрим, что ветки слились
 - ![image](img/-2024-02-07_18-36-06.png)