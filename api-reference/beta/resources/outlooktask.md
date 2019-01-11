---
title: Тип ресурса outlookTask
description: 'Элемент Outlook, можно отслеживать рабочего элемента. '
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 71f649c0ef5fd23caafc9bcd3e35282287d35372
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865564"
---
# <a name="outlooktask-resource-type"></a>Тип ресурса outlookTask

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Элемент Outlook, можно отслеживать рабочего элемента. 

Задачи можно использовать для отслеживания начала, из-за и фактических завершения даты и времени, ее хода выполнения или состоянии, является ли он повторяется и требует получает напоминание.

Свойства, связанные с даты в ресурсе **outlookTask** относятся следующие:

- completedDateTime
- createdDateTime
- dueDateTime
- lastModifiedDateTime
- reminderDateTime
- startDateTime

По умолчанию POST, GET, ИСПРАВЛЕНИЙ и [завершения](../api/outlooktask-complete.md) операции возврата свойства, связанные с даты в их REST ответы в формате UTC. Можно использовать `Prefer: outlook.timezone` заголовок, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC. Следующий пример возвращает свойства, связанные с даты в EST в соответствующем ответа:

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение outlookTask](../api/outlooktask-get.md) | [outlookTask](outlooktask.md) |Получите свойства и связи задачи Outlook в почтовом ящике пользователя.|
|[обновление](../api/outlooktask-update.md). | [outlookTask](outlooktask.md) |Измените записываемые свойства задачи Outlook. |
|[Delete](../api/outlooktask-delete.md) | Нет |Удаление указанной задачи в почтовом ящике пользователя. |
|[Complete](../api/outlooktask-complete.md)|[outlookTask](outlooktask.md) коллекции|Завершить задачу Outlook, которая устанавливает для свойства **completedDateTime** значение текущей датой и свойство **состояние** для `completed`.|
|**Вложения**| | |
|[Список вложений](../api/outlooktask-list-attachments.md) |Коллекция [attachment](attachment.md) | Получение всех вложений на задачи Outlook.|
|[Добавление вложения](../api/outlooktask-post-attachments.md) |[attachment](attachment.md)| Добавление файла, элемент (сообщение, события или контакт) или ссылку в файл как вложение в задачу.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTask](outlooktask.md)  |Создайте один или несколько расширенных свойств одно значение в новой или существующей задачи Outlook.   |
|[Задачи с одним значением расширенных свойств](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | Получение задачи Outlook, которые содержат одно значение расширенные свойства с помощью `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTask](outlooktask.md) | Создайте один или несколько расширенных свойств Многозначный в новой или существующей задачи Outlook.  |
|[Задачи с несколькими значениями расширенных свойств](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | Получение задачи Outlook, которая содержит свойство расширенного Многозначный с помощью `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedTo|Строка|Имя пользователя, которому назначена задача.|
|body|[itemBody](itembody.md)|Основная задача, который обычно содержит сведения о задаче. Обратите внимание на то, что поддерживается только тип HTML-код.|
|categories|Коллекция String|Категории, связанные с задачей. Свойство **displayName** [outlookCategory](outlookcategory.md) , определяемые соответствует каждой категории.|
|changeKey|Строка|Версия задачи.|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата в указанный часовой пояс, окончания задачи.|
|createdDateTime|DateTimeOffset|Дата и время создания задачи. По умолчанию он не в формате UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства используется формат ISO 8601. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|dueDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата в указанный часовой пояс, которую требуется завершения задачи.|
|hasAttachments|Логический|Значение true, если у задачи вложения.|
|id|Строка|Уникальный идентификатор задачи. Только для чтения.|
|importance|string|Важность события. Возможные значения: `low`, `normal`, `high`.|
|isReminderOn|Boolean|Значение true, если оповещение установлено значение Напоминать пользователю задачи.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию он не в формате UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства в формате ISO 8601 и всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|owner|Строка|Имя человека, создавшего задачу.|
|parentFolderId|Строка|Уникальный идентификатор родительской папки задач.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Шаблон повторения для задачи.|
|reminderDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата и время оповещения напоминание задачи, будет выполнена.|
|sensitivity|string|Указывает уровень конфиденциальности для задачи. Возможные значения: `normal`, `personal`, `private`, `confidential`.|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата в указанном часовом поясе после начала задачи.|
|status|string|Указывает состояние или хода выполнения задачи. Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|subject|Строка|Краткое описание или название задачи.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [attachment](attachment.md) |Коллекция [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md)и [referenceAttachment](referenceattachment.md) вложений для задачи.  Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)|Коллекция Многозначный расширенных свойств, определенных для задачи. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)|Коллекция расширенные свойства одно значение, определенное для задачи. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.outlookTask"
}-->

```json
{
  "assignedTo": "String",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["String"],
  "changeKey": "String",
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "id": "String (identifier)",
  "importance": "string",
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "owner": "String",
  "parentFolderId": "String",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "sensitivity": "string",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "string",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
