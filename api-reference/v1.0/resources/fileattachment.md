---
title: Тип ресурса fileAttachment
description: 'Файл (например, текстовый файл или документ Word), вложенный в сведения о событии, сообщение или запись. **contentBytes** '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d71eb6e142097474ac6616456cf6e57ceb8cfb02
ms.sourcegitcommit: 496269b62d42cb7a96752a77b0f2e0cb16918f0b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2019
ms.locfileid: "36484354"
---
# <a name="fileattachment-resource-type"></a>Тип ресурса fileAttachment

Файл (например, текстовый файл или документ Word), вложенный в сведения о событии, сообщение или запись. Свойство **contentBytes** включает содержимое файла в кодировке Base 64.  

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
|contentBytes|Edm.Binary|Содержимое файла в кодировке base64.|
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
  "baseType": "microsoft.graph.attachment",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "string (binary)",
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
<!-- {
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
