---
title: Тип ресурса itemAttachment
description: Контакт, событие или сообщение, присоединенное к другому событию,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: cf8f539411f0825b372da803d07cc341e9babef2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401737"
---
# <a name="itemattachment-resource-type"></a>Тип ресурса itemAttachment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контакт, событие или сообщение, прикрепленное к [событию](../resources/event.md)пользователя, [сообщению](../resources/message.md), [задаче Outlook](../resources/outlooktask.md)или [POST](../resources/post.md).  

Производный от типа [attachment](attachment.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение](../api/attachment-get.md) | [itemAttachment](itemattachment.md) |Чтение свойств, связей или необработанного содержимого объекта itemAttachment.|
|[удаление](../api/attachment-delete.md); | Нет |Удаление объекта itemAttachment. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentType|String|Тип контента этого вложения.|
|id|String| Идентификатор вложения.|
|isInline|Boolean|Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.|
|lastModifiedDateTime|DateTimeOffset|Время и дата последнего изменения вложения.|
|name|String|Отображаемое имя вложения.|
|size|Int32|Размер вложения в байтах.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|item|[OutlookItem](outlookitem.md)|Вложенный контакт, сообщение или событие. Свойство навигации.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "optionalProperties": [
    "item"
  ],
  "@odata.type": "microsoft.graph.itemAttachment"
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
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
