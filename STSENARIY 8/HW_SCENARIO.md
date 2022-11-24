### **_Задание 1. Linux terminal (GitBash) commands_**
_____________________________________________
1. Посмотреть где я - `pwd`
2. Создать папку - `mkdir HW_1`
3. Зайти в папку - `cd HW_1/`
4. Создать 3 папки - `mkdir folder_1 folder_2 folder_3`
5. Зайти в любоую папку - `cd folder_1/`
6. Создать 5 файлов (3 txt, 2 json) - `touch file1.txt file2.txt file3.txt file4.json file5.json`
7. Создать 3 папки - `mkdir papka1 papka2 papka3`
8. Вывести список содержимого папки - `ls -la`
9. Открыть любой txt файл - `vim file1.txt`
10. Написать туда что-нибудь, любой текст - `нажать i и ввести текст: Я в своем познании настолько преисполнился, что я как будто бы уже сто триллионов миллиардов лет проживаю на триллионах и триллионах таких же планет, как эта Земля, мне этот мир абсолютно понятен, и я здесь ищу только одного - покоя, умиротворения и вот этой гармонии, от слияния с бесконечно вечным, от созерцания великого фрактального подобия и от вот этого замечательного всеединства существа, бесконечно вечного, куда ни посмотри, хоть вглубь - бесконечно малое, хоть ввысь - бесконечное большое, понимаешь?`
11. Сохранить и выйти - `Esc + :wq`
12. Выйти из папки на уровень выше - `cd ..`
13. Переместить любые 2 файла, которые вы создали, в любую другую папку - `mv D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_1/file4.json D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_1/file5.json D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_2`
14. Cкопировать любые 2 файла, которые вы создали, в любую другую папку - `cp D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_1/file1.txt D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_1/file2.txt D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_3`
15. Найти файл по имени - `find -name file1.txt`
16. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает - `grep "бесконечно" D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_3/file1.txt`
17. Вывести несколько первых строк из текстового файла - `head -2 D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_3/file1.txt`
18. Вывести несколько последних строк из текстового файла - `tail -2 D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_3/file1.txt`
19. Просмотреть содержимое длинного файла (команда less) изучите как она работает - `less D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_3/file1.txt`
20. Вывести дату и время - `date`
_____________________________________________
### **_*Задание №2 - Отправить http запрос на сервер_**
______________________________________________
`curl 'http://162.55.220.72:5005/object_info_3?name=Evgeney&age=24&salary=1200'`
_____________________________________________
### **_Задание №3 - Написать скрипт, который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13_**
_____________________________________________
Файл со скриптом - **[script.sh](https://github.com/EvgeneyKEO/TerminalLinux/blob/67c8599bc08e0a8a946a854269542a72809c083a/script.sh)**

Команда в терминале - `./script.sh`
```
#!/bin/bash
cd folder_2/
mkdir papochka_1 papochka_2 papochka_3
cd papochka_1/
touch file1.txt file2.txt file3.txt file4.json file5.json
mkdir papochka_4 papochka_5 papochka_6
ls -la
mv file3.txt file4.json papochka_4/
```
__________________________________________________________________________________
## **_GitHub. HW_1_**
__________________________________________________________________________________
 1. Создайте текстовый файл как в первом ДЗ по Terminal
 2. Сценарий перенесите в этот файл.
 3. На против каждого действия - напишите команду в GitBash
 _________________________________________________________________________________
### :large_orange_diamond: JSON
 _________________________________________________________________________________
 4. Создать внешний репозиторий c названием JSON            - [JSON](https://github.com/EvgeneyKEO/JSON.git)

 5. Клонировать репозиторий JSON на локальный компьютер     - `git clone git@github.com:EvgeneyKEO/JSON.git`

 6. Внутри локального JSON создать файл “new.json”          - `touch new.json`

 7. Добавить файл под гит.                                  - `git add .`

 8. Закоммитить файл.                                       - `git commit -m "add new file"`

 9. Отправить файл на внешний GitHub репозиторий.           - `git push`

 10. Отредактировать содержание файла “new.json” - написать 
информацию о себе (ФИО, возраст, количество домашних
животных, будущая желаемая зарплата).
Всё написать в формате JSON.                                - `vim new.json ---> input data ---> esc ---> enter ":wq"`
                                                               
 11. Отправить изменения на внешний репозиторий.            - `git commit -am "update file" && git push`
 							       [new.json](https://github.com/EvgeneyKEO/JSON/blob/cc2c6d91e579d92e0c575d1b85dd255531e6935c/new.json)

 12. Создать файл preferences.json                          - `touch preferences.json`

 13. В файл preferences.json добавить информацию о своих 
предпочтениях (Любимый фильм, любимый сериал, любимая еда,
любимое время года, сторона которую хотели бы посетить) 
в формате JSON.                                             - `vim preferences.json ---> input data ---> esc ---> enter ":wq"`

 14. Создать файл skills.json добавить информацию о скиллах
которые будут изучены на курсе в формате JSON               - `cat >> skills.json ---> input data ---> ctrl + c`

 15. Отправить сразу 2 файла на внешний репозиторий.        - `git add . && git commit -m "add new file" && git push` [preferences.json](https://github.com/EvgeneyKEO/JSON/blob/cc2c6d91e579d92e0c575d1b85dd255531e6935c/bug_report.json) [skills.json](https://github.com/EvgeneyKEO/JSON/blob/cc2c6d91e579d92e0c575d1b85dd255531e6935c/skills.json)

 16. На веб интерфейсе создать файл bug_report.json.        - `Add file --> Create new file --> Name: bug_report.json`

 17. Сделать Commit changes (сохранить) 
изменения на веб интерфейсе.				    - `Commit new file`  [bug_report.json](https://github.com/EvgeneyKEO/JSON/blob/cc2c6d91e579d92e0c575d1b85dd255531e6935c/skills.json)

 18. На веб интерфейсе модифицировать файл 
bug_report.json, добавить баг репорт в формате JSON.        - `Choose bug_report.json --> Edit this file` 

 19. Сделать Commit changes (сохранить) изменения
на веб интерфейсе.					    - `Commit changes`

 20. Синхронизировать внешний и локальный репозиторий JSON  - `git pull`
 _________________________________________________________________________________
### :large_orange_diamond: XML
 _________________________________________________________________________________
 21. Создать внешний репозиторий c названием XML.            - [XML](https://github.com/EvgeneyKEO/XML.git)

 22. Клонировать репозиторий XML на локальный компьютер.     - `git clone https://github.com/EvgeneyKEO/XML.git`

 23. Внутри локального XML создать файл “new.xml”.           - `touch new.xml`

 24. Добавить файл под гит.                                  - `git add .`

 25. Закоммитить файл.                                       - `git commit -m "add new file"`

 26. Отправить файл на внешний GitHub репозиторий.           - `git push`

 27. Отредактировать содержание файла “new.xml” - написать 
информацию о себе (ФИО, возраст, количество
 домашних животных, будущая желаемая зарплата). 
Всё написать в формате XML.                                  - `vim new.xml ---> input data ---> esc ---> enter ":wq"`

 28. Отправить изменения на внешний репозиторий.             - `git commit -am "update file" && git push` [new.xml](https://github.com/EvgeneyKEO/XML/blob/80e38f039f2898659ea6d7ffd6e2477226ddcb08/new.xml)

 29. Создать файл preferences.xml                            - `touch preferences.xml` 

 30. В файл preferences.xml добавить информацию о своих 
предпочтениях (Любимый фильм, любимый сериал, любимая еда,
 любимое время года, сторона которую хотели бы посетить)
 в формате XML.                                              - `vim preferences.xml ---> input data ---> esc ---> enter ":wq"`

 31. Создать файл skills.xml добавить информацию о скиллах
 которые будут изучены на курсе в формате XML		      - `cat >> skills.xml ---> input data ---> ctrl + c`

 32. Сделать коммит в одну строку.                            - `git add . && git commit -m "Add new files"` 

 33. Отправить сразу 2 файла на внешний репозиторий.	      - `git push` 
								[preferences.xml](https://github.com/EvgeneyKEO/XML/blob/80e38f039f2898659ea6d7ffd6e2477226ddcb08/preferences.xml) 
								[skills.xml](https://github.com/EvgeneyKEO/XML/blob/80e38f039f2898659ea6d7ffd6e2477226ddcb08/skills.xml)

 34. На веб интерфейсе создать файл bug_report.xml.           - `Add file --> Create new file --> Name: bug_report.xml` 
								[bug_report.xml](https://github.com/EvgeneyKEO/XML/blob/80e38f039f2898659ea6d7ffd6e2477226ddcb08/bug_report.xml)

 35. Сделать Commit changes (сохранить) изменения 
на веб интерфейсе.					      - `Commit new file`

 36. На веб интерфейсе модифицировать файл bug_report.xml, 
добавить баг репорт в формате XML. 		     	      - `Choose bug_report.xml --> Edit this file` 

 37. Сделать Commit changes (сохранить) 
изменения на веб интерфейсе.			      	      - `Commit changes`

 38. Синхронизировать внешний и локальный репозиторий XML.    - `git pull`
 _________________________________________________________________________________
### :large_orange_diamond: TXT
 _________________________________________________________________________________

 39. Создать внешний репозиторий c названием TXT.	      - [TXT](https://github.com/EvgeneyKEO/TXT.git)
 
 40. Клонировать репозиторий TXT на локальный компьютер	      - `git clone https://github.com/EvgeneyKEO/TXT.git`
 
 41. Внутри локального TXT создать файл “new.txt”.	      - `touch new.txt`

 42. Добавить файл под гит.				      - `git add .`

 43. Закоммитить файл.					      - `git commit -m "add new file"`

 44. Отправить файл на внешний GitHub репозиторий.	      - `git push`

 45. Отредактировать содержание файла “new.txt” - написать    
 информацию о себе (ФИО, возраст, количество домашних 
 животных, будущая желаемая зарплата).
 Всё написать в формате TXT. 				      - `vim new.txt ---> input data ---> esc ---> enter ":wq"`

 46. Отправить изменения на внешний репозиторий.	      - `git commit -am "update file" && git push`
 
 47. Создать файл preferences.txt			      - `touch preferences.txt`

 48. В файл preferences.txt добавить информацию о своих 
 предпочтениях (Любимый фильм, любимый сериал, любимая еда, 
 любимое время года, сторона которую хотели бы посетить) 
 в формате TXT.						      - `vim preferences.txt ---> input data ---> esc ---> enter ":wq"`

 49. Создать файл skills.txt добавить информацию о скиллах 
 которые будут изучены на курсе в формате TXT.		      - `cat >> skills.txt ---> input data ---> ctrl + c`

 50. Сделать коммит в одну строку.			      - `git add . && git commit -m "add new file"`

 51. Отправить сразу 2 файла на внешний репозиторий.	      - `git push`
 								[preferences.txt]()
								[skills.txt]()

 52. На веб интерфейсе создать файл bug_report.txt.	      - `Add file --> Create new file --> Name: bug_report.txt`

 53. Сделать Commit changes (сохранить) 
 изменения на веб интерфейсе.				      - `Commit New File` [bug_report.txt]()

 54. На веб интерфейсе модифицировать файл bug_report.txt, 
 добавить баг репорт в формате TXT.			      - `Choose bug_report.txt --> Edit this file` 

 55. Сделать Commit changes (сохранить)
 изменения на веб интерфейсе.				      - `Commit changes`

 56. Синхронизировать внешний и локальный репозиторий TXT     - `git pull`
__________________________________________________________________________
## **_GitHub. HW_2_**
__________________________________________________________________________
**_Part 1. На локальном репозитории сделать ветки для:_**
- Postman						       
- Jmeter						       
- CheckLists						       
- Bag Reports								
- SQL
- Charles
- Mobile testing
1.
 1.1. Создать на Githab репозитроий, в котором будут располагаться ветки [HW_31_group](https://github.com/EvgeneyKEO/HW_31_group.git)
 
 1.2. Клонируем внешний репозиторий на локальный репозиторий `git clone https://github.com/EvgeneyKEO/HW_31_group.git` 
 
 1.3. Заходим в склонированный репозиторий `cd HW_31_group/`
 
 1.4. Создаем ветки Postman, Jmeter, CheckLists, Bag Reports, SQL, Charles, Mobile testing:
``` 
git branch Postman
git branch Jmeter
git branch CheckLists
git branch SQL
git branch Charles
git branch Mobile_testing
``` 
      
**_Part 2. Запушить все ветки на внешний репозиторий_**
```
git push -u origin Postman
git push -u origin Jmeter
git push -u origin CheckLists
git push -u origin BagReports
git push -u origin SQL
git push -u origin Charles
git push -u origin Mobile_testing
```

**_Part 3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта_**
```
git checkout BagReports
cat >>  bagrep.txt --> добавляем структуру баг репорта
нажимаем ctrl+c
```
      
**_Part 4. Запушить структуру багрепорта на внешний репозиторий_**
`git add . && git commit -m "add new file" && git push`

**_Part 5. Вмержить ветку Bag Reports в Main_**
```
git checkout main
git merge BagReports
```
      
**_Part 6. Запушить main на внешний репозиторий._**
`git push -u origin main`

**_Part 7. В ветке CheckLists набросать структуру чек листа_**
```
git checkout CheckLists
cat >> CheckLists.json
забиваем структуру чек-листа в формате JSON
```

**_Part 8. Запушить структуру на внешний репозиторий_**
`git add . && git commit -m "add new file" && git push`

**_Part 9. На внешнем репозитории сделать Pull Request ветки CheckLists в main_**
`Переходим на внешний репозиторий в ветку CheckLists, нажимаем кнопку Compare&pull requset`

**_Part 10. Синхронизировать Внешнюю и Локальную ветки Main_**
```
git checkout main
git fetch - просмотрим действительно ли были какие-то изменения на внешнем репозитории
git pull
```