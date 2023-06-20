# Home work for Vadim Ksendzov's course.
## XML

**1. Создать внешний репозиторий c названием XML**
- создаю на своем github.com репозиторий с названием XML
 
**2. Клонировать репозиторий XML на локальный компьютер**
- `git clone https://github.com/00Julie00/XML`

**3. Внутри локального XML создать файл “new.xml”**
- перехожу в локальный репозиторий XML
  `cd XML` 
- создаю файл 
   `touch new.xml`
   
**4. Добавить файл под гит**
- `git add -A`
- `git status`

**5. Закоммитить файл**
- `git commit - m "add file new"`

**6. Отправить изменения на внешний репозиторий**
- `git push`

**7. Отредактировать содержание файла “new.xml” - написать информацию о себе 
(ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML**

```
vim new.xml
i
<?xml version="1.0" encoding="UTF-8"?>
<root>
   	<name>Julia</name>
   	<surname>Rusanova</surname>
   	<age>39</age>
   	<pets>false</pets>
   	<my_desierd_salary>600</salary>
</root>
ESC 
:wq
Enter
```

**8. Закоммитить файл**
- `git commit -a -m "modified new.xml"`

**9. Отправить изменения на внешний репозиторий**
- `git push`

**10. Создать файл preferences.xml**
- `touch preferences.xml`

**11. В файл preferences.xml добавить информацию о своих предпочтениях 
(Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) 
в формате XML**
```
vim preferences.xml
i
<?xml version="1.0" encoding="UTF-8"?>
<root>
  <favorite_movie>Knockin 'on Heaven</favorite_movie>
  <favorite_series>Game of Thrones</favorite_series>
  <favorite_food>bread</fav_food>
  <favorite_season>summer</favorite_season>
  <my_future_travel>Japan</my_future_travel>
</root>
ESC 
:wq
Enter
```

**12. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML**
- `touch sklls.xml`
```
vim sklls.xml
i
<?xml version="1.0" encoding="UTF-8"?>
<root>
  <skill_1>Terminal</skill_1>
  <skill_2>GitBash</skill_2>
  <skill_3>Git</skill_3>
  <skill_4>Testing documentation</skill_4>
  <skill_5>Types of testing</skill_5>
  <skill_6>Postman</skill_6>
  <skill_7>API</skill_7>
  <skill_8>Dev Tools</skill_8>
  <skill_9>Charles</skill_9>
  <skill_10>ADB</skill_10>
  <skill_11>SQL</skill_11>
  <skill_12>Postgres</skill_12>
  <skill_13>Redis</skill_13>
  <skill_14>Jmeter</skill_14>
  <skill_15>Scrum</skill_15>
  <skill_16>Python</skill_16>
</root>	
ESC
:wq
Enter
```
**13. Отправить сразу 2 файла на внешний репозиторий**
- `git add -A` 
- `git status`
- `git commit -m "add preferences.xml, sklls.xml"` 
- `git push`

**14. На веб интерфейсе создать файл bug_report.xml**
- создала файл на веб-интерфейсе файл с названием bug_report.xml

**15. Сделать Commit changes (сохранить) изменения на веб интерфейсе**
- сделала commit, сохранила изменения

**16. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML**
- добавила баг репорт на веб интерфейсе
```
<?xml version="1.0" encoding="UTF-8"?>
<root>
    <ID>2</ID>
    <Title>Значение текущей даты в поле Дата Рождения принмается как валидное в форме заявки на кредитную карту</Title>
    <Steps>
       <Step_1>Зайти на страницу http://zayavka-na-kartu.ru/</Step_1>
       <Step_2>Заполнить в произвольном порядке все поля в заявке валидными значениями: имя, фамилия, отчество, телефон, паспорт</Step_2>
       <Step_3>В поле Дата Рождения ввести текущую дату = сегодняшний день</Step_3>
       <Step_4>Нажать кнопку 'отправить' внизу формы</Step_4>
    </Steps>
    <Actual_result>Поле заполняется, данные принмаются как валидные. Форма заявки отправляется</Actual_result>
    <Expected_result>Поле 'Дата Рождения' выделяется красным, появляется сообщение 'Проверьте корректность данных'</Expected_result>
</root>

```
**17. Сделать Commit changes (сохранить) изменения на веб интерфейсе**
- сделала commit, сохранила изменения

**18. Синхронизировать внешний и локальный репозиторий XML**
- получаю последнюю версию удаленного репозитория
`git pull`
