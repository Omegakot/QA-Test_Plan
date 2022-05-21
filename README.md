<h1 align=center>Тест-план</h1>
Тестируется новый функционал “Личные события” в меню расписание личного кабинета преподавателя.

**Заказчик**: онлайн-школа Skyeng

**Ссылка на меню**: [Расписание](https://teachers.skyeng.ru/schedule)

<h2 align=center>Описание и документация</h2>
Основные функции нового элемента “ Личные события” в соответствии с технической документацией.

Основные требования:

- **Операции с личными событиями**: *Добавление личных событий*, *редактирование, удаление*
- **Отображение личных событий в слотах при совмещении урока**

Спецификация по новому функционалу: [Новый фукционал](https://skyengpublic.notion.site/0323fc20054c447595e2bb567efeded7)

Документация API : [API](https://skyengpublic.notion.site/API-edd2d237611546a2adb36aeb1f0f3c5c)

Будут проведены следующие виды тестирования:

**по целям**: *функциональное ( API, User Interface)* , *нефункциональное(UI)*

**по видам, связанных с изменениями в программном продукте**: *smoke*, *регресс тестирование*

**по формализации**: *сценарное*, *исследовательское*

**по видам входных данных**: *позитивное*, *негативное*

Будут применены следующие **техники тест дизайна**: *класс эквивалентности*, *граничные значения*

<h2 align=center>Тестирование требований</h2>

|**Требование**|**Вопрос к требованию**|**Критерий**|
| :-: | :-: | :-: |
|Преподаватель может использовать личные события для собственных встреч.|Как будет выполняться функция в расписании, если на это время запланирован урок? Вероятно предполагалось описание использование личных события для каких либо личных заметок.|Требование не соответствует критерию «завершенность»|
|Они служат напоминанием, что у преподавателя что-то запланировано на это время.|Предполагается ли что то более в функционале, чем просто напоминание в виде графического отображения личного события?|Требование не соответствует критерию «проверяемость, завершенность»|
|Описание — необязательно для заполнения, нет ограничения на символы|Нет какого конкретно ограничения? на их количество или на комбинации|Требование не соответствует критерию «проверяемость, атомарность»|
|На данном этапе нельзя вставлять картинки. Доступны маркдауны и ссылки.|На каком этапе? на этапе сохранения? Доступны в поле или допустимы при вводе данных типа: маркдауны и ссылки?|Требование не соответствует критерию «недвусмысленность»|
|Цвет события — по умолчанию серый.|Почему в макете представлен цвет в градиентах?|Требование не соответствует критерию «непротиворечивость»|
|Если событие и урок совпадают по времени, урок отображается всегда выше всего.|**Выше всего** это чего? Выше личного события или слота? На макете не полностью отражены варианты расположения. |Требование не соответствует критерию «недвусмысленность, завершенность»|
|Если два события происходят в одно время, отображается выше то, которое было создано последним.|а если их больше? например 15 и выше, как это будет отображено в слоте? |Требование не соответствует завершенность, проверяемость»|
<h2 align=center>Декомпозиция</h2>

[карта функционала "Личные события"](https://miro.com/app/board/o9J_liIdz7g=/)



<h2 align=center>Приемочные тест-кейсы</h2>

[Тест кейсы](https://app.qase.io/project/1COURSE)

Отчет о проведении test run приёмочного тестирования доступен по ссылке: 

<https://app.qase.io/public/report/99ef8c19196869a71288ed8aff2452569e4f2606>

комментарий по не пройдённому тест кейсу по ссылке: 

<https://app.qase.io/case/1COURSE-2#comments>

[QASE.IO](https://app.qase.io/) : 


<h2 align=center>Тестовая документация</h2>

**Функциональное и нефункциональное тестирование**:

1. Добавление события 

>- чек лист: <https://chlist.sitechco.ru/project/25280/checklist/1115177/details>

2. Редактирование события 

>- чек лист: <https://chlist.sitechco.ru/project/25280/checklist/1115227/details>

3. Удаление события 

>- чек лист: <https://chlist.sitechco.ru/project/25280/checklist/1115186/details>

4. Отображение события при совмещении урока 

>- чек лист: <https://chlist.sitechco.ru/project/25280/checklist/1115228/details>

**Исследовательское тестирование**:

>- чек лист: <https://chlist.sitechco.ru/project/25280/checklist/1115354/details>

**Smoke тесты**: <https://app.qase.io/project/1COURSE?suite=3>

**Чек лист проверки нового функционала через backend по API** : [Чек лист](https://chlist.sitechco.ru/project/25280/checklist/1163530/details)

**Postman collection**: 

[Collection](https://drive.google.com/file/d/1c23KD-Tc-Ig7yARGe2LF6IC_FM6pSP6J/view?usp=sharing)

*Доступ к чек листам и ТMS*:

<https://chlist.sitechco.ru/> 

<http://qase.io> 

<h2 align=center>Cроки тестирования</h2>

Тестировщик: **Владимир Евтушенко**

|**Виды тестирования**|**Срок тестирования(план)**|**Срок тестирования(факт)**|
| :-: | :-: | :-: |
|Функциональное|18.11-02.12|18.11-19.11|
|Нефункциональное тестирование|18.11-02.12|18.11-19.11|
|Исследовательское (регресс-тестирование)|18.11-02.12|18.11-19.11|
|Функциональное тестирование (API)|03.02.-04.02|03.02.-03.02|


<h2 align=center>Окружение тестируемой системы</h2>

**ОС**: Windows 10, 

**Browser**: Google Chrome Версия 96.0.4664.45 (Официальная сборка), (64 бит), MS Edge.

**ПО для тестирования API:** Postman v9.13.0 

<h2 align=center>«Отчет о тестировании итогового проекта»</h2>

Все тесты проведены в указанный срок.

Были проведены следующие виды тестирования: 

>- функциональное ( via User Intrface, via API ), 
>- нефункциональное(UI)
>- smoke, регресс тестирование
>- сценарное, исследовательское

применены следующие техники тест дизайна при составлении чек листов: 

класс эквивалентности, граничные значения

Также при составлении чек листов учитывались входные данные: позитивное, негативное, что позволило провести тестирование критического пути.

Проведен тест ран smoke тестирования, результаты теста по ссылке: [Отчет test run](https://app.qase.io/public/report/749b3e7590a67322337c0ba23154768c4fcc2b84)

Сформирован отчет по результатам прохождения тестирования по чек листам: 

>- Добавление события : <https://chlist.sitechco.ru/project/25280/checklist/result/200209/details>
>- Удаление события: <https://chlist.sitechco.ru/project/25280/checklist/result/200210/details>
>- Редактирования события: <https://chlist.sitechco.ru/project/25280/checklist/result/200217/details>
>- Отображение события: <https://chlist.sitechco.ru/project/25280/checklist/result/200211/details>

Отчет по исследовательскому тестированию: <https://chlist.sitechco.ru/project/25280/checklist/result/200266/details>

Отчет по тестированию API: <https://chlist.sitechco.ru/project/25280/checklist/result/208068/details>
#### **Баг репорты**
Ссылка на проект в JIRA: [Course](https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7)



>**Баг репорты по новому функционалу**: 

**c высоким приоритетом(High)**:

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-11>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-20>

**со средним приоритетом (Medium)**:

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-2>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-9>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-18>

**с низким приоритетом(Low)**:

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-4>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-5>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-6>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-7>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-8>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-10>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-12>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-13>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-14>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-15>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-16>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-17>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-19>

**с незначительным приоритетом (Lowest)**:

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-21>

<https://evtushenko.atlassian.net/jira/software/projects/XMSX/boards/7?selectedIssue=XMSX-22>
<h2 align=center>Метрика</h2>

>Успешность прохождение smoke-тестов: **100%**

>Успешность прохождение чек-листов функционального и нефункционального тестирования составляет: **79%**

>Общее затраченное время на прохождение тестирования составляет: **100 минут**

>Коэффициент тестового покрытия составляет: **5,05**

>Общее количество найденных дефектов составляет: **21 шт.**

<h2 align=center>Рекомендации</h2>

В результате проведенного тестирования команде dream team необходимо тщательно пересмотреть техническую документацию продукта, так как она неполноценно описывает сущность всех требований. Были выявлены дефекты, которые не соответствуют описанию в документации нового функционала, а значит излишне потраченное время тестировщика на заведение баг репортов, которые в последствии будут тестироваться повторно. Рекомендовано разработать автоматизацию тестов для regress и smoke тестирования, что позволит сократить время проверок, используемых при ручном тестировании, тем самым уменьшить сроки выхода нового функционала в релиз согласно используемой модели разработки web продукта.

<h2 align=center>Выводы</h2>

На основании проведенного тестирования **новый функционал (личные события)** системы полностью **не готов** к релизу, не смотря на то, что проведено регресс-тестирование старого функционала, в ходе которого не было выявлено значительных дефектов. Выявлены дефекты в новом функционале, которые необходимо устранить, в частности одновременного отображения в слоте события и урока при их совмещении по времени, а также дефекты связанные со стилями текста и ограничение на символы, которые необходимо дополнить в технической документации, дефекты по выбору даты личного события. Не менее значимое действие, которое повлияет на дальнейшую доработку и прогресс выпуска нового функционала является изучение информации согласно рекомендаций. После проведенных процедур устранения значительных багов и проведение цикла повторных тестов продукт готов к релизу.
