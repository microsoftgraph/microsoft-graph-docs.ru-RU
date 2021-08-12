---
title: Обзор API планов и заданий Планировщика
description: Планировщик — удобное средство для визуальной организации работы команд. С помощью Планировщика пользователи могут создавать планы, упорядочивать и назначать задачи, делиться сведениями о ходе выполнения, а также совместно работать над контентом.  Планировщик включает несколько интерактивных интерфейсов, в том числе доску задач, страницу диаграмм и представление расписаний, а также интеграцию между службами Microsoft 365.
author: TarkanSevilmis
localization_priority: Priority
ms.prod: planner
ms.openlocfilehash: 45ce4719e9fa46d163cb98f9318757255af9b9d6decea3af4947285f3419f243
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169060"
---
# <a name="planner-tasks-and-plans-api-overview"></a>Обзор API планов и заданий Планировщика
Планировщик — удобное средство для визуальной организации работы команд. С помощью Планировщика пользователи могут создавать планы, упорядочивать и назначать задачи, делиться сведениями о ходе выполнения, а также совместно работать над контентом.  Планировщик включает несколько интерактивных интерфейсов, в том числе доску задач, страницу диаграмм и представление расписаний, а также интеграцию между службами Microsoft 365.

**Доска задач Планировщика в Microsoft 365**

![Снимок экрана: доска задач Планировщика в Microsoft 365](images/plannerboard.png "Изображение доски Планировщика")


## <a name="why-integrate-with-planner-tasks"></a>Преимущества интеграции с задачами Планировщика
Планировщик предоставляет возможности отслеживания задач в решениях для совместной работы в Microsoft 365. Если в ваших сценариях требуется отслеживать задачи и упорядочивать работу команды или группы пользователей, то Планировщик отлично вам подойдет. Интеграция с Планировщиком поможет вам связываться с миллионами пользователей, совместно работающих в Microsoft 365. 

### <a name="organize-your-teams-work"></a>Организация работы в команде
Планировщик предоставляет общее пространство, где вы можете собрать команду, [создавать задачи](/graph/api/planner-post-tasks?view=graph-rest-1.0) и назначать их другим пользователям в команде. Планировщик помогает всем узнавать, чем занимаются другие пользователи и как продвигается работа над проектом. Вы можете обновлять задачи, добавляя такие сведения, как даты выполнения, ход выполнения и описания, а также упорядочивать задачи с помощью настраиваемых сегментов и меток категорий.   

### <a name="collaborate-across-microsoft-365"></a>Совместная работа в Microsoft 365
Планировщик интегрируется в решения Microsoft 365 для совместной работы. Помимо веб-клиента и мобильного клиента Планировщика, пользователям доступны возможности просмотра и обновления планов и задач из SharePoint и Microsoft Teams.  

Сам Планировщик также работает на платформе Microsoft Graph и службы групп Microsoft 365. Файлы, отправляемые и вкладываемые в задачи Планировщика, хранятся в SharePoint. Примечания в Планировщике основаны на беседах групп Outlook.

<!-- Add image
Note: Put an image here showing the relationship between Planner and other things
-->

### <a name="automate-the-creation-of-plans-and-tasks"></a>Автоматизация создания планов и задач
Работаете над повторяющимся процессом или типом проекта? С помощью API Планировщика вы можете автоматизировать создания плана и списка задач.  
 
## <a name="top-planner-api-tasks"></a>Основные задачи API Планировщика

|Операция|URL-адрес|
|:--------|:--|
|Просмотр всех [планов](/graph/api/resources/plannerplan?view=graph-rest-beta) для группы|GET [https://graph.microsoft.com/v1.0/groups/{id}/planner/plans](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|Просмотр [задач](/graph/api/resources/plannertask?view=graph-rest-beta) в плане|GET [https://graph.microsoft.com/v1.0/planner/plans/{id}/tasks](https://developer.microsoft.com/graph/graph-explorer?request=planner/plans/{id}/tasks&version=v1.0)|
|Просмотр всех [личных задач](/graph/api/planneruser-list-tasks?view=graph-rest-beta), назначенных мне во всех планах|GET [https://graph.microsoft.com/v1.0/me/planner/tasks/](https://developer.microsoft.com/graph/graph-explorer?request=me/planner/tasks/&version=v1.0)|
|[Создание задачи](/graph/api/planner-post-tasks?view=graph-rest-1.0)|POST [https://graph.microsoft.com/v1.0/planner/tasks](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|[Обновление задачи](/graph/api/plannertask-update?view=graph-rest-1.0)|PATCH [https://graph.microsoft.com/v1.0/planner/tasks/{task-id}](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|[Удаление задачи](/graph/api/plannertask-delete?view=graph-rest-1.0)|DELETE [https://graph.microsoft.com/v1.0/planner/tasks/{id}](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API Планировщика в Microsoft Graph 1.0](/graph/api/resources/planner-overview?view=graph-rest-1.0)
- [API Планировщика в бета-версии Microsoft Graph](/graph/api/resources/planner-overview?view=graph-rest-beta)


## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Планировщика](/graph/api/resources/planner-overview?view=graph-rest-1.0)
- [Работа с планами](/graph/api/resources/planner-overview?view=graph-rest-1.0#plans)
- [Работа с задачами](/graph/api/resources/planner-overview?view=graph-rest-1.0#tasks)
