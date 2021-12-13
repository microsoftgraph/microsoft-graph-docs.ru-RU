---
title: тип ресурса задач
description: Представляет задачу, например часть работы или личный элемент, которую можно отслеживать и завершить.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6f9339f3ed4871ac86c2adff4a2c6efc4a145db3
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61425021"
---
# <a name="task-resource-type"></a>тип ресурса задач

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет задачу, например часть работы или личный элемент, которую можно отслеживать и завершить. Задача **всегда** содержится в [списке задач.](basetasklist.md) 

Этот ресурс поддерживает следующее:
* Добавление данных в качестве настраиваемой свойства в [открытых расширениях.](/graph/extensibility-overview)
* подписку на [уведомления об изменениях](/graph/webhooks);
* Использование [delta-запроса](/graph/delta-query-overview) для отслеживания дополнительных дополнений, удалений и обновлений.

Наследует [от baseTask](../resources/basetask.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление задач](../api/basetasklist-list-tasks.md)|[коллекция](../resources/task.md) задач|Получите список объектов [задач](../resources/task.md) и их свойств.|
|[Вывод задачи](../api/basetask-get.md)|[task](../resources/task.md)|Ознакомьтесь с свойствами и отношениями объекта [задач.](../resources/task.md)|
|[Обновление задачи](../api/basetask-update.md)|[task](../resources/task.md)|Обновление свойств объекта [задачи.](../resources/task.md)|
|[Удаление задачи](../api/basetask-delete.md)|Нет|Удаляет объект [задачи.](../resources/task.md)|
|[move](../api/basetask-move.md)|[baseTask](../resources/basetask.md)|Переместим сообщение в другой список.|
|[Контрольные списки спискаItems](../api/basetask-list-checklistitems.md)|[коллекция checklistItem](../resources/checklistitem.md)|Получите ресурсы checklistItem из свойства навигации checklistItems.|
|[Создание контрольного спискаItem](../api/basetask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Создайте новый объект checklistItem.|
|[Список linkedResources](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) коллекции|Получите linkedResource_v2 ресурсов из свойства навигации linkedResources.|
|[Создание linkedResource](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Создание нового linkedResource_v2 объекта.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|body|[itemBody](../resources/itembody.md)|Текст задачи, который обычно содержит сведения о задаче. Унаследовано от [baseTask](../resources/basetask.md).|
|bodyLastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, полночь UTC 1 января 2020 г. будет выглядеть так: '2020-01-01T00:00:00Z'. Унаследовано от [baseTask](../resources/basetask.md).|
|completedDateTime|DateTimeOffset|Дата завершения задачи. Унаследовано от [baseTask](../resources/basetask.md).|
|createdDateTime|DateTimeOffset|Дата и время создания задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601. Например, полночь UTC 1 января 2020 г. будет выглядеть так: '2020-01-01T00:00:00Z'. Унаследовано от [baseTask](../resources/basetask.md).|
|displayName|Строка|Имя задачи. Унаследовано от [baseTask](../resources/basetask.md).|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе, когда задача должна быть завершена. Унаследовано от [baseTask](../resources/basetask.md).|
|id|String|Уникальный идентификатор задачи. По умолчанию это значение не изменится, если задача перемещается из одного списка в другой. Унаследовано от [baseTask](../resources/basetask.md).|
|importance|importance|Важность задачи. Возможные значения: `low`, `normal`, `high`. Унаследовано от [baseTask](../resources/basetask.md). Допустимые значения: `low`, `normal`, `high`.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, полночь UTC 1 января 2020 г. будет выглядеть так: '2020-01-01T00:00:00Z'. Унаследовано от [baseTask](../resources/basetask.md).|
|personalProperties|[personalTaskProperties](../resources/personaltaskproperties.md)|Свойства, которые являются личными для пользователя, такие как reminderDateTime. Унаследовано от [baseTask](../resources/basetask.md).|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|Расписание повторения задачи. Унаследовано от [baseTask](../resources/basetask.md).|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе, когда задача должна быть начата. Унаследовано от [baseTask](../resources/basetask.md).|
|status|taskStatus_v2|Указывает состояние или ход выполнения задачи. Возможные значения: `notStarted` `inProgress` , , `completed` `unknownFutureValue` . Унаследовано от [baseTask](../resources/basetask.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|checklistItems|[коллекция checklistItem](../resources/checklistitem.md)|Коллекция контрольных списков, связанных с задачей. Унаследованный от [baseTask](../resources/basetask.md)|
|extensions|Коллекция [extension](../resources/extension.md)|Коллекция открытых расширений, определенных для задачи. Унаследованный от [baseTask](../resources/basetask.md)|
|linkedResources|[linkedResource_v2](../resources/linkedresource_v2.md) коллекции|Коллекция ресурсов, связанных с задачей. Унаследованный от [baseTask](../resources/basetask.md)|
|parentList|[baseTaskList](../resources/basetasklist.md)|Список, содержащий задачу. Унаследованный от [baseTask](../resources/basetask.md)|

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
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
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
  "personalProperties": {
    "@odata.type": "microsoft.graph.personalTaskProperties"
  },
  "id": "String (identifier)"
}
```

