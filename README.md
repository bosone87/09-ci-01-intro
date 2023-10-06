# Домашнее задание к занятию 7 «Жизненный цикл ПО»

## Подготовка к выполнению

1. Получить бесплатную версию [Jira](https://www.atlassian.com/ru/software/jira/free).
2. Настроить её для своей команды разработки.
3. Создать доски Kanban и Scrum.
4. [Дополнительные инструкции от разработчика Jira](https://support.atlassian.com/jira-cloud-administration/docs/import-and-export-issue-workflows/).

## Основная часть

Необходимо создать собственные workflow для двух типов задач: bug и остальные типы задач. Задачи типа bug должны проходить жизненный цикл:

1. Open -> On reproduce.
2. On reproduce -> Open, Done reproduce.
3. Done reproduce -> On fix.
4. On fix -> On reproduce, Done fix.
5. Done fix -> On test.
6. On test -> On fix, Done.
7. Done -> Closed, Open.

<p align="center">
  <img width="1200 height="600" src="./workflow_bug.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./types_workflow_bug_asign.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./workflow_bug_add.png">
</p>

Остальные задачи должны проходить по упрощённому workflow:

1. Open -> On develop.
2. On develop -> Open, Done develop.
3. Done develop -> On test.
4. On test -> On develop, Done.
5. Done -> Closed, Open.

<p align="center">
  <img width="1200 height="600" src="./workflow_other.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./types_workflow_other_asign.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./workflow_other_add.png">
</p>


<p align="center">
  <img width="1200 height="600" src="./workflow_types_all.png">
</p>


**Что нужно сделать**

1. Создайте задачу с типом bug, попытайтесь провести его по всему workflow до Done.
<p align="center">
  <img width="1200 height="600" src="./bug-1-1.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./bug-1-2.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./bug-1-3.png">
</p>

2. Создайте задачу с типом epic, к ней привяжите несколько задач с типом task, проведите их по всему workflow до Done.
3. При проведении обеих задач по статусам используйте kanban.

<p align="center">
  <img width="1200 height="600" src="./epic-1-1.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./epic-1-2.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./epic-1-3.png">
</p>

4. Верните задачи в статус Open.
<p align="center">
  <img width="1200 height="600" src="./issues_kanban.png">
</p>

5. Перейдите в Scrum, запланируйте новый спринт, состоящий из задач эпика и одного бага, стартуйте спринт, проведите задачи до состояния Closed. Закройте спринт.
<p align="center">
  <img width="1200 height="600" src="./issues_scrum.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./sprint_scrum.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./issues_scrum.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./sprint-report-1.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./sprint-report-2.png">
</p>

<p align="center">
  <img width="1200 height="600" src="./sprint-report-3.png">
</p>

6. Если всё отработалось в рамках ожидания — выгрузите схемы workflow для импорта в XML. Файлы с workflow и скриншоты workflow приложите к решению задания.

[Workflow-bug](./workflow_bug.xml)

[Workflow-other](./workflow_other.xml)

---