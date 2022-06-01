---
title: Тип ресурса task
description: Представляет задачу, например рабочий или личный элемент, которую можно отслеживать и завершить.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6d07d876535115c26b42d808e6870ec65f5dd2eb
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821241"
---
# <a name="task-resource-type-deprecated"></a>тип ресурса task (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

Представляет задачу, например рабочий или личный элемент, которую можно отслеживать и завершить. Задача **всегда** содержится в [базовом списке задач](basetasklist.md). 

Этот ресурс поддерживает следующее:
* Добавление данных в виде настраиваемых свойств в [открытых расширениях](/graph/extensibility-overview).
* подписку на [уведомления об изменениях](/graph/webhooks);
* Использование [разностного](/graph/delta-query-overview) запроса для отслеживания добавочных дополнений, удалений и обновлений.

Наследуется от [baseTask](../resources/basetask.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление задач](../api/basetasklist-list-tasks.md)|[коллекция задач](../resources/task.md)|Получение списка объектов [задачи](../resources/task.md) и их свойств.|
|[Вывод задачи](../api/basetask-get.md)|[task](../resources/task.md)|Чтение свойств и связей [объекта задачи](../resources/task.md) .|
|[Обновление задачи](../api/basetask-update.md)|[task](../resources/task.md)|Обновление свойств [объекта задачи.](../resources/task.md)|
|[Удаление задачи](../api/basetask-delete.md)|Нет|Удаляет [объект задачи](../resources/task.md) .|
|[move](../api/basetask-move.md)|[baseTask](../resources/basetask.md)|Переместите сообщение в другой список.|
|[Перечисление контрольных элементов](../api/todotask-list-checklistitems.md)|[Коллекция checklistItem](../resources/checklistitem.md)|Получите ресурсы checklistItem из свойства навигации checklistItems.|
|[Создание checklistItem](../api/todotask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Создайте объект checklistItem.|
|[Перечисление linkedResources](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) коллекции|Получение linkedResource_v2 ресурсов из свойства навигации linkedResources.|
|[Создание linkedResource](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Создайте новый linkedResource_v2 объекта.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|textbody|[itemBody](../resources/itembody.md)|Текст задачи в текстовом формате, который обычно содержит сведения о задаче. Наследуется от [baseTask](../resources/basetask.md).|
|bodyLastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, полночь в формате UTC 1 января 2020 г. будет выглядеть следующим образом: "2020-01-01T00:00:00Z". Наследуется от [baseTask](../resources/basetask.md).|
|completedDateTime|DateTimeOffset|Дата завершения задачи. Наследуется от [baseTask](../resources/basetask.md).|
|createdDateTime|DateTimeOffset|Дата и время создания задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601. Например, полночь в формате UTC 1 января 2020 г. будет выглядеть следующим образом: "2020-01-01T00:00:00Z". Наследуется от [baseTask](../resources/basetask.md).|
|displayName|Строка|Имя задачи. Наследуется от [baseTask](../resources/basetask.md).|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе, когда задача должна быть завершена. Наследуется от [baseTask](../resources/basetask.md).|
|id|String|Уникальный идентификатор задачи. По умолчанию это значение не изменится, если задача перемещается из одного списка в другой. Наследуется от [baseTask](../resources/basetask.md).|
|importance|importance|Важность задачи. Возможные значения: `low`, `normal`, `high`. Наследуется от [baseTask](../resources/basetask.md). Допустимые значения: `low`, `normal`, `high`.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, полночь в формате UTC 1 января 2020 г. будет выглядеть следующим образом: "2020-01-01T00:00:00Z". Наследуется от [baseTask](../resources/basetask.md).|
|Точки обзора|[taskViewpoint](../resources/taskviewpoint.md)|Свойства, которые являются личными для пользователя, такие как **reminderDateTime** и **категории**. Наследуется от [baseTask](../resources/basetask.md).|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|Расписание повторения задачи. Наследуется от [baseTask](../resources/basetask.md).|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе, когда задача должна быть начата. Наследуется от [baseTask](../resources/basetask.md).|
|status|taskStatus_v2|Указывает состояние или ход выполнения задачи. Возможные значения: `notStarted`, `inProgress`, , `completed`,`unknownFutureValue`. Наследуется от [baseTask](../resources/basetask.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|checklistItems|[Коллекция checklistItem](../resources/checklistitem.md)|Коллекция checklistItems, связанных с задачей. Наследуется от [baseTask](../resources/basetask.md)|
|extensions|Коллекция объектов [extension](../resources/extension.md)|Коллекция открытых расширений, определенных для задачи. Наследуется от [baseTask](../resources/basetask.md)|
|linkedResources|[linkedResource_v2](../resources/linkedresource_v2.md) коллекции|Коллекция ресурсов, связанных с задачей. Наследуется от [baseTask](../resources/basetask.md)|
|parentList|[baseTaskList](../resources/basetasklist.md)|Список, содержащий задачу. Наследуется от [baseTask](../resources/basetask.md)|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.task",
  "baseType": "microsoft.graph.baseTask",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.task",
  "textBody": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "bodyLastModifiedDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "startDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "importance": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "displayName": "String",
  "status": "String",
  "viewpoint": {
    "@odata.type": "microsoft.graph.taskViewpoint"
  },
  "id": "String (identifier)"
}
```

