---
title: Тип ресурса baseTask
description: Представляет задачу, например рабочий или личный элемент, которую можно отслеживать и завершить.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4ec4f4fd5f124f475a2183f468063051e4c26526
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820947"
---
# <a name="basetask-resource-type-deprecated"></a>Тип ресурса baseTask (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

Абстрактный тип, представляющий задачу, например рабочий или личный элемент, который можно отслеживать и завершить.

Это базовый тип, наследуемый [ресурсом](task.md) задачи.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление baseTasks](../api/basetasklist-list-tasks.md)|[Коллекция baseTask](../resources/basetask.md)|Получение списка объектов [baseTask](../resources/basetask.md) и их свойств.|
|[Создание baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Создайте объект [baseTask](../resources/basetask.md) .|
|[Получение baseTask](../api/basetask-get.md)|[baseTask](../resources/basetask.md)|Чтение свойств и связей объекта [baseTask](../resources/basetask.md) .|
|[Обновление baseTask](../api/basetask-update.md)|[baseTask](../resources/basetask.md)|Обновление свойств объекта [baseTask](../resources/basetask.md) .|
|[Удаление baseTask](../api/basetask-delete.md)|Нет|Удаляет объект [baseTask](../resources/basetask.md) .|
|[move](../api/basetask-move.md)|[baseTask](../resources/basetask.md)|Переместите сообщение в другой список.|
|[delta](../api/basetask-delta.md)|[Коллекция baseTask](../resources/basetask.md)|Получение набора объектов **baseTask** , которые были добавлены, удалены или обновлены в указанном списке.|
|[Перечисление контрольных элементов](../api/todotask-list-checklistitems.md)|[Коллекция checklistItem](../resources/checklistitem.md)|Получите ресурсы **checklistItem** из свойства навигации checklistItems.|
|[Создание checklistItem](../api/todotask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Создайте объект **checklistItem** .|
|[Перечисление linkedResources](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) коллекции|Получение **linkedResource_v2 ресурсов** из свойства навигации linkedResources.|
|[Создание linkedResource_v2](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Создайте **новый linkedResource_v2** объекта.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|textBody|Строка|Текст задачи в текстовом формате, который обычно содержит сведения о задаче. |
|bodyLastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, полночь в формате UTC 1 января 2020 г. будет выглядеть следующим образом: "2020-01-01T00:00:00Z". |
|completedDateTime|DateTimeOffset|Дата завершения задачи. |
|createdDateTime|DateTimeOffset|Дата и время создания задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601. Например, полночь в формате UTC 1 января 2020 г. будет выглядеть следующим образом: "2020-01-01T00:00:00Z". |
|displayName|Строка|Имя задачи. |
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе, когда задача должна быть завершена. |
|id|String|Уникальный идентификатор задачи. По умолчанию это значение не изменится, если задача перемещается из одного списка в другой. |
|importance|importance|Важность задачи. Возможные значения: `low`, `normal`, `high`.  Допустимые значения: `low`, `normal`, `high`.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, полночь в формате UTC 1 января 2020 г. будет выглядеть следующим образом: "2020-01-01T00:00:00Z". |
|Точки обзора|[taskViewpoint](../resources/taskviewpoint.md)|Свойства, которые являются личными для пользователя, такие как **reminderDateTime** и **категории**. |
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|Расписание повторения задачи. |
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе, когда задача должна быть начата. |
|status|taskStatus_v2|Указывает состояние или ход выполнения задачи. Возможные значения: `notStarted`, `inProgress`, , `completed`,`unknownFutureValue`. |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|checklistItems|[Коллекция checklistItem](../resources/checklistitem.md)|Коллекция небольших подзадач, связанных с более сложной родительской задачей. |
|extensions|Коллекция объектов [extension](../resources/extension.md)|Коллекция открытых расширений, определенных для задачи. |
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

