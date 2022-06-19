---
title: Тип ресурса fileAttachment
description: Файл (например, текстовый файл или документ Word), прикрепленный к событию, сообщению или записи.
ms.localizationpriority: high
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ffd35829cfafac92b2cd6707e0d653325b37993e
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160625"
---
# <a name="fileattachment-resource-type"></a>Тип ресурса fileAttachment

Пространство имен: microsoft.graph

Файл (например, текстовый файл или документ Word), вложенный в [событие](../resources/event.md) пользователя, [сообщение](../resources/message.md) или [запись](../resources/post.md). 

При создании вложенного файла включите в текст запроса следующее:

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* Обязательные свойства **name** и **contentBytes**.

Производный от типа [attachment](attachment.md).

> [!NOTE]
> Не забудьте закодировать содержимое файла в base64 перед назначением его **contentBytes**.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение](../api/attachment-get.md) | [fileAttachment](fileattachment.md) |Чтение свойств, связей или необработанного содержимого объекта **fileAttachment**.|
|[Удаление](../api/attachment-delete.md) | Нет |Удаление объекта **fileAttachment**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentBytes|Edm.Binary|Содержимое файла в кодировке base64.|
|contentId|String|Идентификатор вложения в хранилище Exchange.|
|contentLocation|String|Не используйте это свойство, так как оно не поддерживается.|
|contentType|String|Тип контента этого вложения.|
|id|String|Идентификатор вложения.|
|isInline|Boolean|Задано значение `true`, если это встроенное вложение.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения вложения.|
|name|String|Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.|
|size|Int32|Размер вложения в байтах.|

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
  "size": "Int32"
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

