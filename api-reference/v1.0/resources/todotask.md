---
title: тип ресурса todoTask
description: Ресурс todoTask отслеживает рабочий элемент.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9e620161e48f87a4e46afcfcfe6a0dce6bb069b3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134320"
---
# <a name="todotask-resource-type"></a>тип ресурса todoTask

Пространство имен: microsoft.graph

**TodoTask представляет** собой задачу, например часть работы или личный элемент, которую можно отслеживать и завершить. 

**TodoTask всегда** содержится в [todoTaskList.](todotasklist.md) Он включает связь с коллекцией объектов [linkedResource,](./linkedResource.md) отслеживая один или несколько источников задачи.

Этот ресурс поддерживает следующее:
* Добавление данных в качестве настраиваемой свойства в [открытых расширениях.](/graph/extensibility-overview)
* Использование [delta-запроса](/graph/delta-query-overview) для отслеживания дополнительных дополнений, удалений и обновлений.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление задач](../api/todotasklist-list-tasks.md)|Коллекция [todoTask](todotask.md)|Получение всех ресурсов [todoTask](todotask.md) в указанном списке.|
|[Создание задачи](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| Создание [todoTask в](todotask.md) указанном списке задач|
|[Вывод задачи](../api/todotask-get.md)|[todoTask](../resources/todotask.md)|Ознакомьтесь с свойствами и отношениями [объекта todoTask.](../resources/todotask.md)|
|[Обновление задачи](../api/todotask-update.md)|[todoTask](../resources/todotask.md)|Обновление свойств объекта [todoTask.](../resources/todotask.md)|
|[Удаление задачи](../api/todotask-delete.md)|Нет|Удаляет объект [todoTask.](../resources/todotask.md)|
|[Список linkedResources](../api/todotask-list-linkedresources.md)|[коллекция linkedResource](../resources/linkedresource.md)|Получите linkedResources из свойства навигации linkedResources.|
|[Создание linkedResources](../api/todotask-post-linkedresources.md)|[linkedResource](../resources/linkedresource.md)|Создайте новый объект linkedResources.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|body|[itemBody](../resources/itembody.md)|Текст задачи, который обычно содержит сведения о задаче.|
|bodyLastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, полночь UTC 1 января 2020 г. будет выглядеть так: '2020-01-01T00:00:00Z'.|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе, когда задача была завершена.|
|createdDateTime|DateTimeOffset|Дата и время создания задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601. Например, полночь UTC 1 января 2020 г. будет выглядеть так: '2020-01-01T00:00:00Z'.|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе, когда задача должна быть завершена.|
|id|String|Уникальный идентификатор задачи. По умолчанию это значение изменяется при перемещении элемента из одного списка в другой.|
|importance|importance|Важность задачи. Возможные значения: `low`, `normal`, `high`.|
|isReminderOn|Boolean|Присвоено значение true, если установлено напоминание пользователю о задаче.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, полночь UTC 1 января 2020 г. будет выглядеть так: '2020-01-01T00:00:00Z'.|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|Расписание повторения задачи.|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата и время появления напоминания о задаче.|
|status|taskStatus|Указывает состояние или ход выполнения задачи. Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|title|Строка|Краткое описание задачи.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|extensions|Коллекция [extension](extension.md)| Коллекция открытых расширений, определенных для задачи. Допускается значение null.|
|linkedResources|[коллекция linkedResource](../resources/linkedresource.md)|Коллекция ресурсов, связанных с задачей.|


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



