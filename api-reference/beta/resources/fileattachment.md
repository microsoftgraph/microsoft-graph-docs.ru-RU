---
title: Тип ресурса fileAttachment
description: Файл (например, текстовый файл или документ Word), подключенного к событию
localization_priority: Normal
ms.openlocfilehash: 7d9f92565e38aaf418691480b7f8f3187c57647c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644093"
---
# <a name="fileattachment-resource-type"></a>Тип ресурса fileAttachment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Файл (например, текстовый файл или документ Word) подключенного к [события](../resources/event.md), [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md). Свойство **contentBytes** содержит кодировки Base64 содержимое файла.  

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
|id|String|Идентификатор вложения.|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/fileattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
