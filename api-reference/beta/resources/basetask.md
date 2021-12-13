---
title: тип ресурса baseTask
description: Представляет задачу, например часть работы или личный элемент, которую можно отслеживать и завершить
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 99577e6576c2a2bce2e4580df65b7f9da5931eb6
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61425138"
---
# <a name="basetask-resource-type"></a>тип ресурса baseTask

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет задачу, например часть работы или личный элемент, которую можно отслеживать и завершить.
Это абстрактный базовый тип, унаследованный [ресурсом задач.](task.md)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список baseTasks](../api/basetasklist-list-tasks.md)|[коллекция baseTask](../resources/basetask.md)|Получите список объектов [baseTask](../resources/basetask.md) и их свойств.|
|[Создание baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Создайте новый [объект baseTask.](../resources/basetask.md)|
|[Get baseTask](../api/basetask-get.md)|[baseTask](../resources/basetask.md)|Ознакомьтесь с свойствами и отношениями [объекта baseTask.](../resources/basetask.md)|
|[Обновление baseTask](../api/basetask-update.md)|[baseTask](../resources/basetask.md)|Обновление свойств объекта [baseTask.](../resources/basetask.md)|
|[Удаление baseTask](../api/basetask-delete.md)|Нет|Удаляет объект [baseTask.](../resources/basetask.md)|
|[move](../api/basetask-move.md)|[baseTask](../resources/basetask.md)|Переместим сообщение в другой список.|
|[delta](../api/basetask-delta.md)|[коллекция baseTask](../resources/basetask.md)|Получите набор объектов **baseTask,** которые были добавлены, удалены или обновлены в указанном списке.|
|[Контрольные списки спискаItems](../api/basetask-list-checklistitems.md)|[коллекция checklistItem](../resources/checklistitem.md)|Получите **ресурсы checklistItem** из свойства навигации checklistItems.|
|[Создание контрольного спискаItem](../api/basetask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Создайте **новый объект checklistItem.**|
|[Список linkedResources](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) коллекции|Получите **linkedResource_v2** ресурсов из свойства навигации linkedResources.|
|[Создание linkedResource_v2](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Создание нового **linkedResource_v2** объекта.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|body|[itemBody](../resources/itembody.md)|Текст задачи, который обычно содержит сведения о задаче. |
|bodyLastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, полночь UTC 1 января 2020 г. будет выглядеть так: '2020-01-01T00:00:00Z'. |
|completedDateTime|DateTimeOffset|Дата завершения задачи. |
|createdDateTime|DateTimeOffset|Дата и время создания задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601. Например, полночь UTC 1 января 2020 г. будет выглядеть так: '2020-01-01T00:00:00Z'. |
|displayName|Строка|Имя задачи. |
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе, когда задача должна быть завершена. |
|id|String|Уникальный идентификатор задачи. По умолчанию это значение не изменится, если задача перемещается из одного списка в другой. |
|importance|importance|Важность задачи. Возможные значения: `low`, `normal`, `high`.  Допустимые значения: `low`, `normal`, `high`.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, полночь UTC 1 января 2020 г. будет выглядеть так: '2020-01-01T00:00:00Z'. |
|personalProperties|[personalTaskProperties](../resources/personaltaskproperties.md)|Свойства, которые являются личными для пользователя, такие как reminderDateTime. |
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|Расписание повторения задачи. |
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе, когда задача должна быть начата. |
|status|taskStatus_v2|Указывает состояние или ход выполнения задачи. Возможные значения: `notStarted` `inProgress` , , `completed` `unknownFutureValue` . |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|checklistItems|[коллекция checklistItem](../resources/checklistitem.md)|Коллекция контрольных списков, связанных с задачей. |
|extensions|Коллекция [extension](../resources/extension.md)|Коллекция открытых расширений, определенных для задачи. |
|linkedResources|[linkedResource_v2](../resources/linkedresource_v2.md) коллекции|Коллекция ресурсов, связанных с задачей. |
|parentList|[baseTaskList](../resources/basetasklist.md)|Список, содержащий задачу. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseTask",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.baseTask",
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

