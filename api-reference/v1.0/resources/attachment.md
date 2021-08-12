---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в экземпляр event,
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1151ff7a9392ba6450651b8d5df24eed1b6a28189a25b935ec2570a0280d436b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178614"
---
# <a name="attachment-resource-type"></a>Тип ресурса attachment

Пространство имен: microsoft.graph

Вы можете добавить связанное содержимое в экземпляр [event](../resources/event.md), [message](../resources/message.md) или [post](../resources/post.md) в форме вложения.

**attachment** — базовый ресурс для следующих производных типов вложений:

* файл (ресурс [fileAttachment](../resources/fileattachment.md));
* элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));
* ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).

События в календарях группы не поддерживают вложения.

## <a name="methods"></a>Методы

Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение вложения](../api/attachment-get.md) | [attachment](attachment.md) |Чтение свойств, связей или необработанного содержимого объекта, представляющего вложение, которое было добавлено к пользовательскому событию, сообщению или записи.|
|[Добавление вложения в пользовательское событие](../api/event-post-attachments.md) | [attachment](attachment.md) |Добавление файла, элемента или вложения-ссылки в качестве события в пользовательском календаре.|
|[Добавление вложения в сообщение](../api/message-post-attachments.md) | [attachment](attachment.md) |Добавление в сообщение файла, элемента или ссылки в качестве вложения.|
|[Добавление вложения в запись](../api/post-post-attachments.md) | [attachment](attachment.md) |Добавление в запись файла, элемента или ссылки в качестве вложения.|
|[Список вложений пользовательского события](../api/event-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для события в пользовательском календаре. |
|[Список вложений для сообщения](../api/message-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для сообщения. |
|[Список вложений для записи](../api/post-list-attachments.md) | Коллекция [attachment](attachment.md)  | Получение списка вложений для записи. |
|[Удаление](../api/attachment-delete.md) | Нет |Удаление объекта, представляющего вложение, которое было добавлено к сообщению, записи или данным о событии. |

## <a name="properties"></a>Свойства

Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentType|String|Тип MIME.|
|id|String| Только для чтения.|
|isInline|Boolean|Значение `true`, если вложение является встроенным. В противном случае — значение `false`.|
|lastModifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|name|String|Имя вложенного файла.|
|size|Int32|Размер вложения в байтах.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
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
<!-- {
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

