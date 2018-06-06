# <a name="planner-tasks-and-plans-api-overview"></a>Обзор API планов и заданий Планировщика
Планировщик — удобное средство для визуальной организации работы команд. С помощью Планировщика пользователи могут создавать планы, упорядочивать и назначать задачи, делиться сведениями о ходе выполнения, а также совместно работать над контентом.  Планировщик включает несколько интерактивных интерфейсов, в том числе доску задач, страницу диаграмм и представление расписаний, а также интеграцию между службами Office 365.

**Доска задач в Планировщике (Майкрософт)**

![Снимок экрана с доской задач Планировщика (Майкрософт)](images/plannerboard.png "Изображение доски Планировщика")


## <a name="why-integrate-with-planner-tasks"></a>Преимущества интеграции с задачами Планировщика
Планировщик предоставляет возможности отслеживания задач в решениях для совместной работы в Office 365. Если в ваших сценариях требуется отслеживать задачи и упорядочивать работу команды или группы пользователей, то Планировщик отлично вам подойдет. Интеграция с Планировщиком поможет вам связываться с миллионами пользователей, совместно работающих в Office 365. 

### <a name="organize-your-teams-work"></a>Организация работы в команде
Планировщик предоставляет общее пространство, где вы можете собрать команду, [создавать задачи](../api-reference/v1.0/api/planner_post_tasks.md) и назначать их другим пользователям в команде. Планировщик помогает всем узнавать, чем занимаются другие пользователи и как продвигается работа над проектом. Вы можете обновлять задачи, добавляя такие сведения, как даты выполнения, ход выполнения и описания, а также упорядочивать задачи с помощью настраиваемых сегментов и меток категорий.   

### <a name="collaborate-across-office-365"></a>Совместная работа в Office 365
Планировщик интегрируется в решения для совместной работы в Office 365. Помимо веб-клиента и мобильного клиента Планировщика, пользователям доступны возможности просмотра и обновления планов и задач из SharePoint и Microsoft Teams.  

Сам Планировщик также работает на платформе Microsoft Graph и службы групп Office 365. Файлы, отправляемые и вкладываемые в задачи Планировщика, хранятся в SharePoint. Примечания в Планировщике основаны на беседах групп Outlook.

<!-- Add image
Note: Put an image here showing the relationship between Planner and other things
-->

### <a name="automate-the-creation-of-plans-and-tasks"></a>Автоматизация создания планов и задач
Работаете над повторяющимся процессом или типом проекта? С помощью API Планировщика вы можете автоматизировать создания плана и списка задач.  
 
## <a name="top-planner-api-tasks"></a>Основные задачи API Планировщика

|Операция|URL-адрес|
|:--------|:--|
|Просмотр всех [планов](../api-reference/beta/resources/plannerplan.md) для группы|GET [https://graph.microsoft.com/v1.0/groups/{id}/planner/plans](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|Просмотр [задач](../api-reference/beta/resources/plannertask.md) в плане|GET [https://graph.microsoft.com/v1.0/planner/plans/{id}/tasks](https://developer.microsoft.com/en-us/graph/graph-explorer?request=planner/plans/{id}/tasks&version=v1.0)|
|Просмотр всех [личных задач](../api-reference/beta/api/planneruser_list_tasks.md), назначенных мне во всех планах|GET [https://graph.microsoft.com/v1.0/me/planner/tasks/](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/planner/tasks/&version=v1.0)|
|[Создание задачи](../api-reference/v1.0/api/planner_post_tasks.md)|POST [https://graph.microsoft.com/v1.0/planner/tasks](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|[Обновление задачи](../api-reference/v1.0/api/plannertask_update.md)|PATCH [https://graph.microsoft.com/v1.0/planner/tasks/{task-id}](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|[Удаление задачи](../api-reference/v1.0/api/plannertask_delete.md)|DELETE [https://graph.microsoft.com/v1.0/planner/tasks/<id>](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|


## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Планировщика](../api-reference/v1.0/resources/planner_overview.md)
- [Работа с планами](../api-reference/v1.0/resources/planner_overview.md#plans)
- [Работа с задачами](../api-reference/v1.0/resources/planner_overview.md#tasks)
