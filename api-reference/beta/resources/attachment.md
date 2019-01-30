---
title: Тип ресурса attachment
description: Связанное содержимое можно добавить на событие
localization_priority: Normal
ms.openlocfilehash: 59e1074cea9508af45cef0b6e61ea223a3ca851e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643152"
---
# <a name="attachment-resource-type"></a>Тип ресурса attachment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Связанное содержимое можно добавить для [события](../resources/event.md), [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md) в виде вложения.

**attachment** — базовый ресурс для следующих производных типов вложений:

* файл (ресурс [fileAttachment](../resources/fileattachment.md));
* элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));
* ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).

## <a name="methods"></a>Методы

Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение вложения](../api/attachment-get.md) | [attachment](attachment.md) |Чтение свойства и связи вложения, подключенного к события, сообщения, задачи Outlook или post.|
|[Добавление вложения к данным о событии](../api/event-post-attachments.md) | [attachment](attachment.md) |Добавление для события файла, элемента или ссылки в качестве вложения.|
|[Добавление вложения в сообщение](../api/message-post-attachments.md) | [attachment](attachment.md) |Добавление в сообщение файла, элемента или ссылки в качестве вложения.|
|[Добавление вложения в задачи Outlook](../api/outlooktask-post-attachments.md) | [attachment](attachment.md) |Добавление файла, элемента или вложения ссылки на задачи Outlook.|
|[Добавление вложения в запись](../api/post-post-attachments.md) | [attachment](attachment.md) |Добавление в запись файла, элемента или ссылки в качестве вложения.|
|[Список вложений для события](../api/event-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для события. |
|[Список вложений для сообщения](../api/message-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для сообщения. |
|[Вложения списка задачи Outlook](../api/outlooktask-list-attachments.md) | Коллекция [attachment](attachment.md) | Получение списка вложений для задачи Outlook. |
|[Список вложений для записи](../api/post-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для записи. |
|[Удаление](../api/attachment-delete.md) | Нет |Удаление вложения на события, сообщения, задачи Outlook или post. |

## <a name="properties"></a>Свойства

Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentType|String|Тип MIME.|
|id|String| Только для чтения.|
|isInline|Boolean|Значение `true`, если вложение является встроенным. В противном случае — значение `false`.|
|lastModifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|имя|String|Отображаемое имя вложения. Она не обязательно должна находиться фактическое имя файла.|
|size|Int32|Размер вложения в байтах.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
