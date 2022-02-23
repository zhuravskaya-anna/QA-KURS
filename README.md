1. Посмотреть где я
   `pwd`
2. Создать папку
   `mkdir fff`
3. Зайти в папку
   `cd fff`
4. Создать 3 папки
   `mkdir f1 f2 f3`
5. Зайти в любоую папку
   `cd f1`
6. Создать 5 файлов (3 txt, 2 json)  
   `touch txt1.txt txt2.txt txt3.txt j1.json j2.json`
7. Создать 3 папки
   `mkdir ff1 ff2 ff3`
8. Вывести список содержимого папки
   ls -la
9. Открыть любой txt файл
   `cat > txt1.txt`
10. - написать туда что-нибудь, любой текст. ===
            в траве
            сидел
            кузнечик
            совсем
            как огуречик

11. - сохранить и выйти. ===
      `CTRL+C`
12. Выйти из папки на уровень выше
    `cd ..`
13. переместить любые 2 файла, которые вы создали, в любую другую папку.
    `mv f1/{txt1.txt,txt2.txt} f2/`
14. скопировать любые 2 файла, которые вы создали, в любую другую папку.
    `cp f1/{j1.json,j2.json} f3/`
15. Найти файл по имени
    `find . -name txt*`
16. просмотреть содержимое в реальном времени  
    `tail -f 1.txt` _отображает измения в файле (после сохранения файла)_
17. вывести несколько первых строк из текстового файла
    `head -n 2 1.txt`
18. вывести несколько последних строк из текстового файла
    `tail -n 2 1.txt`
19. просмотреть содержимое длинного файла (команда less) изучите как она работает.
    `less 1.txt`
    `q` _выйти_
20. вывести дату и время
    `date`

---

Задание \*

1. Отправить http запрос на сервер.
   http://162.55.220.72:5005/terminal-hw-request
   
   `curl "http://162.55.220.72:5005/terminal-hw-request"`

ответ сервера
      {"Intro":"Hello!! This is your the first response from server","Tasks":{"Task*1":"Send the next URL in terminal: set * your\_ String","result":["Your_String","Your_number"]}}

`curl "http://162.55.220.72:5005/get_method?name=Anna&age=28"`

ответ сервера

        ["Anna","28"]

---

2. Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

-создать файл
myscript.sh

      > \#1/bin/bash

            cd fff
            mkdir f1 f2 f3
            cd f1
            touch txt1.txt txt2.txt txt3.txt j1.json j2.json
            mkdir ff1 ff2 ff3
            ls -la
            mv {txt1.txt,txt2.txt} ../f2/cd

-сделать файл исполняемым
`chmod +x ./myscript.sh`

-запустить файл
`./myscript.sh`

---
