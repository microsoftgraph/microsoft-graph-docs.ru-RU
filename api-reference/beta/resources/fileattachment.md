---
title: Тип ресурса fileAttachment
description: Файл (например, текстовый файл или документ Word), вложенный в событие, сообщение, задачу или запись.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 14ae2bb7ec5e341a144fa5c00eb131853ea6b679
ms.sourcegitcommit: 2132198551c7d1f37474debab471f612a3e35a08
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2022
ms.locfileid: "66141245"
---
# <a name="fileattachment-resource-type"></a>Тип ресурса fileAttachment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Файл (например, текстовый файл или документ Word), вложенный в [событие пользователя,](../resources/event.md) [сообщение, Outlook](../resources/message.md) [задачу](../resources/outlooktask.md) [или запись](../resources/post.md). 

При создании вложенного файла включите в текст запроса следующее:

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* Обязательные свойства **name** и **contentBytes**.

Производный от типа [attachment](attachment.md).

> [!NOTE]
> Не забудьте закодировать содержимое файла в base64 перед назначением его **contentBytes**.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение](../api/attachment-get.md) | [fileAttachment](fileattachment.md) |Чтение свойств, связей или необработанного содержимого объекта **fileAttachment** .|
|[Удаление](../api/attachment-delete.md) | Нет |Удаление объекта **fileAttachment** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentBytes|Edm.Binary|Содержимое файла в кодировке base64.|
|contentId|String|Идентификатор вложения в хранилище Exchange.|
|contentLocation|String|Не используйте это свойство, так как оно не поддерживается.|
|contentType|String|Тип контента этого вложения.|
|id|String|Идентификатор вложения.|
|isInline|Boolean|Задайте `true` значение, если это встроенная вложение.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения вложения.|
|name|String|Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.|
|size|Int32|Размер вложения в байтах.|

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

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


