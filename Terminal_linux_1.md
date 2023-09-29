## Linux terminal (GitBash) commands

1. Посмотреть где я - `pwd`
2. Создать папку - `mkdir qa`
3. Зайти в папку - `cd qa`
4. Создать 3 папки - `mkdir html, mkdir css, mkdir js`
5. Зайти в любоую папку - `cd html`
6. Создать 5 файлов (3 txt, 2 json) - `touch html/test.txt, touch html/body.txt, touch css/style.txt, touch js/script.json, touch js/logs.json`
7. Создать 3 папки - `mkdir html, mkdir css, mkdir js`
8. Вывести список содержимого папки - `ls`
9. Открыть любой txt файл - `vim body.txt`
10. Написать туда что-нибудь, любой текст - `text`
11. Сохранить и выйти. - `ESC :wq`
12. Выйти из папки на уровень выше - `cd ..`
13. Переместить любые 2 файла, которые вы создали, в любую другую папку - `mv js/logs.json html/logs.json`
14. Скопировать любые 2 файла, которые вы создали, в любую другую папку - `cp html/body.txt, js/body.txt`
15. Найти файл по имени find - `name "script.json"`
16. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает - `grep "test" body.txt`
17. Вывести несколько первых строк из текстового файла - `head body.txt`
18. Вывести несколько последних строк из текстового файла - `tail body.txt`
19. Просмотреть содержимое длинного файла (команда less) изучите как она работает. - `less body.txt`
20. Вывести дату и время - `date`

## Task*

1) Отправить http запрос на сервер.
http://162.55.220.72:5006/terminal-hw-request
   - `curl "http://162.55.220.72:5006/terminal-hw-request"`

![1](https://github.com/supremexkid/Terminal/assets/126493566/ae1fb9c9-eeef-465b-9e77-7cd827b79e02)

 Ответ серверу.
    - `"http://162.55.220.72:5005/get_method?name=(login)&age=(17)"`
   
![2](https://github.com/supremexkid/Terminal/assets/126493566/4b13e0dc-83bc-4dbc-b8e1-be4371cf0b05)

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
```
#!/bin/sh
cd Terminal
mkdir {first,second,third}
cd second
touch {file-1.txt,file-2.txt,file-3.txt,file-4.json,file-5.json}
mkdir {fourth,fifth,sixth}
ls -la
mv file-1.txt file-5.json fourth
```
