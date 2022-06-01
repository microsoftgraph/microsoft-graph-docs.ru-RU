---
title: Тип ресурса todoTask
description: Ресурс todoTask отслеживает рабочий элемент.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 541e2079d7eb9a27f61acf6e0f46e7b194dd7321
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820793"
---
# <a name="todotask-resource-type"></a>Тип ресурса todoTask

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TodoTask** представляет задачу, например рабочий или личный элемент, которую можно отслеживать и завершить. 

**TodoTask** всегда содержится в [todoTaskList](todotasklist.md). Он включает связь с коллекцией объектов [linkedResource](./linkedResource.md) , отслеживая один или несколько источников задачи.

Этот ресурс поддерживает следующее:
* Добавление данных в виде настраиваемых свойств в [открытых расширениях](/graph/extensibility-overview).
* подписку на [уведомления об изменениях](/graph/webhooks);
* Использование [разностного](/graph/delta-query-overview) запроса для отслеживания добавочных дополнений, удалений и обновлений.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление задач](../api/todotasklist-list-tasks.md)|Коллекция [todoTask](todotask.md)|Получение всех ресурсов [todoTask](todotask.md) в указанном списке.|
|[Создание задачи](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| Создание [объекта todoTask](todotask.md) в указанном списке задач|
|[Вывод задачи](../api/todotask-get.md)|[todoTask](../resources/todotask.md)|Чтение свойств и связей объекта [todoTask](../resources/todotask.md) .|
|[Обновление задачи](../api/todotask-update.md)|[todoTask](../resources/todotask.md)|Обновление свойств объекта [todoTask](../resources/todotask.md) .|
|[Удаление задачи](../api/todotask-delete.md)|Нет|Удаляет объект [todoTask](../resources/todotask.md) .|
|[Перечисление контрольных элементов](../api/todotask-list-checklistitems.md)|[Коллекция checklistItem](../resources/checklistitem.md)|Получите ресурсы **checklistItem** из свойства навигации checklistItems.|
|[Создание checklistItem](../api/todotask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Создайте объект **checklistItem** .|
|[Перечисление linkedResources](../api/todotask-list-linkedresources.md)|[Коллекция linkedResource](../resources/linkedresource.md)|Получение объекта linkedResources из свойства навигации linkedResources.|
|[Создание linkedResources](../api/todotask-post-linkedresources.md)|[linkedResource](../resources/linkedresource.md)|Создайте объект linkedResources.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|body|[itemBody](../resources/itembody.md)|Текст задачи, который обычно содержит сведения о задаче.|
|bodyLastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, полночь в формате UTC 1 января 2020 г. будет выглядеть следующим образом: "2020-01-01T00:00:00Z".|
|categories|Коллекция String|Категории, связанные с задачей. Каждая категория соответствует свойству **displayName** объекта [outlookCategory](../resources/outlookcategory.md), определенному пользователем.|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе, когда задача была завершена.|
|createdDateTime|DateTimeOffset|Дата и время создания задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601. Например, полночь в формате UTC 1 января 2020 г. будет выглядеть следующим образом: "2020-01-01T00:00:00Z".|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе, когда задача должна быть завершена.|
|id|String|Уникальный идентификатор задачи. По умолчанию это значение изменяется при перемещении элемента из одного списка в другой.|
|importance|importance|Важность задачи. Возможные значения: `low`, `normal`, `high`.|
|isReminderOn|Boolean|Присвоено значение true, если установлено напоминание пользователю о задаче.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, полночь в формате UTC 1 января 2020 г. будет выглядеть следующим образом: "2020-01-01T00:00:00Z".|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|Расписание повторения задачи.|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата и время появления напоминания о задаче.|
|status|taskStatus|Указывает состояние или ход выполнения задачи. Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|title|Строка|Краткое описание задачи.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|checklistItems|[Коллекция checklistItem](../resources/checklistitem.md)|Коллекция небольших подзадач, связанных с более сложной родительской задачей. |
|extensions|Коллекция объектов [extension](extension.md)| Коллекция открытых расширений, определенных для задачи. Допускается значение null.|
|linkedResources|[Коллекция linkedResource](../resources/linkedresource.md)|Коллекция ресурсов, связанных с задачей.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTask",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTask",
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "categories": ["string"],
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "importance": "String",
  "isReminderOn": "Boolean",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "reminderDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "status": "String",
  "title": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "bodyLastModifiedDateTime": "String (timestamp)"
}
```



