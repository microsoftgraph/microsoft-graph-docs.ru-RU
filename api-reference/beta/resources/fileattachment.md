---
title: Тип ресурса fileAttachment
description: Файл (например, текстовый файл или документ Word), присоединенный к событию,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 966de812c8b0507c3d757d42fba5624c0b82ce4f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972042"
---
# <a name="fileattachment-resource-type"></a>Тип ресурса fileAttachment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Файл (например, текстовый файл или документ Word), присоединенный к событию, [сообщению](../resources/message.md), [задаче Outlook](../resources/outlooktask.md)или [POST](../resources/post.md). [](../resources/event.md) Свойство **contentBytes** включает содержимое файла в кодировке Base 64.  

При создании вложенного файла включите в текст запроса следующее:

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* Обязательные свойства **name** и **contentBytes**.

Производный от типа [attachment](attachment.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение](../api/attachment-get.md) | [fileAttachment](fileattachment.md) |Чтение свойств и связей объекта fileAttachment.|
|[Удаление](../api/attachment-delete.md) | Нет |Удаление объекта fileAttachment. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentBytes|Двоичный|Содержимое файла в кодировке base64.|
|contentId|String|Идентификатор вложения в хранилище Exchange.|
|contentLocation|String|Не используйте это свойство, так как оно не поддерживается.|
|contentType|String|Тип контента этого вложения.|
|id|Строка|Идентификатор вложения.|
|isInline|Boolean|Задано значение true, если это встроенное вложение.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения вложения.|
|name|String|Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.|
|size|Int32|Размер вложения в байтах.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "binary",
  "contentId": "string",
  "contentLocation": "string",
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
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
