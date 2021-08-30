---
title: Тип ресурса outlookTask
description: 'Элемент Outlook, который может отслеживать рабочий элемент. '
author: mashriv
ms.localizationpriority: high
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f4cf54ad1420cd18ac8d7665ba8bdf02f4bc0dc2
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695268"
---
# <a name="outlooktask-resource-type-deprecated"></a>Тип ресурса outlookTask (нерекомендуемый)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]

Элемент Outlook, который может отслеживать рабочий элемент.

Вы можете использовать задачу для отслеживания начала, запланированной и фактической даты и времени выполнения, хода выполнения или состояния, а также является ли она повторяющейся и требует ли напоминания.

Свойства, связанные с датами в ресурсе **outlookTask**, включают указанные ниже:

- completedDateTime
- createdDateTime
- dueDateTime
- lastModifiedDateTime
- reminderDateTime
- startDateTime

По умолчанию операции POST, GET, PATCH и [complete](../api/outlooktask-complete.md) возвращают связанные с датами свойства в откликах REST в формате UTC.
Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC. В приведенном ниже примере связанные с датами свойства возвращаются в соответствующем отклике в часовом поясе EST:

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение outlookTask](../api/outlooktask-get.md) | [outlookTask](outlooktask.md) |Получение свойств и связей задачи Outlook в почтовом ящике пользователя.|
|[Обновление](../api/outlooktask-update.md) | [outlookTask](outlooktask.md) |Изменение записываемых свойств задачи Outlook. |
|[Удаление](../api/outlooktask-delete.md) | Нет |Удаление определенной задачи в почтовом ящике пользователя. |
|[Завершение](../api/outlooktask-complete.md)|Коллекция [outlookTask](outlooktask.md)|Завершение задачи Outlook с присвоением свойству **completedDateTime** значения текущей даты, а свойству **status** — значения `completed`.|
|**Вложения**| | |
|[Список вложений](../api/outlooktask-list-attachments.md) |Коллекция [attachment](attachment.md) | Получение всех вложений для задачи Outlook.|
|[Добавление вложения](../api/outlooktask-post-attachments.md) |[attachment](attachment.md)| Добавление файла, элемента (сообщения, события или контакта) или ссылки на файл в виде вложения в задачу.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTask](outlooktask.md)  |Создание одного или нескольких расширенных свойств с одним значением в новой или существующей задаче Outlook.   |
|[Получение задачи с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | Получение задач Outlook, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTask](outlooktask.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новой или существующей задаче Outlook.  |
|[Получение задачи с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | Получение задачи Outlook, которая содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedTo|String|Имя пользователя, которому назначена задача в Outlook. Только для чтения.|
|body|[itemBody](itembody.md)|Текст задачи, который обычно содержит сведения о задаче. Обратите внимание, что поддерживается только тип HTML.|
|categories|Коллекция String|Категории, связанные с задачей. Каждая категория соответствует свойству **displayName** объекта [outlookCategory](outlookcategory.md), определенному пользователем.|
|changeKey|String|Версия задачи.|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата в указанном часовом поясе, когда задача была завершена.|
|createdDateTime|DateTimeOffset|Дата и время создания задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|dueDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата в указанном часовом поясе, когда задача должна быть завершена.|
|hasAttachments|Boolean|Присвоено значение true, если у задачи есть вложения.|
|id|String| Уникальный идентификатор задачи. [!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] Только для чтения. |
|importance|importance|Важность события. Возможные значения: `low`, `normal`, `high`.|
|isReminderOn|Boolean|Присвоено значение true, если установлено напоминание пользователю о задаче.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию используется формат UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства представлено в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|owner|String|Имя пользователя, создавшего задачу.|
|parentFolderId|String|Уникальный идентификатор родительской папки задачи.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Расписание повторения задачи.|
|reminderDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата и время появления напоминания о задаче.|
|sensitivity|sensitivity|Указывает уровень конфиденциальности для задачи. Возможные значения: `normal`, `personal`, `private`, `confidential`.|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата в указанном часовом поясе, когда задача должна быть начата.|
|status|taskStatus|Указывает состояние или ход выполнения задачи. Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|subject|String|Краткое описание или название задачи.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [attachment](attachment.md) |Коллекция вложений [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md) и [referenceAttachment](referenceattachment.md) для задачи.  Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)|Коллекция расширенных свойств с несколькими значениями, определенных для задачи. Только для чтения. Допускается значение NULL.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)|Коллекция расширенных свойств с одним значением, определенных для задачи. Только для чтения. Допускается значение NULL.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "outlookTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


