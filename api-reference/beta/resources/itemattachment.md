---
title: Тип ресурса itemAttachment
description: Контакт, событие или сообщение, присоединенное к другому событию,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 31fd3e74e7fc35589abc57a891678e9a129c2a2e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010086"
---
# <a name="itemattachment-resource-type"></a>Тип ресурса itemAttachment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контакт, событие или сообщение, присоединенное к другому событию [](../resources/event.md), [сообщению](../resources/message.md), [задаче Outlook](../resources/outlooktask.md)или [POST](../resources/post.md).  

Производный от типа [attachment](attachment.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение](../api/attachment-get.md) | [itemAttachment](itemattachment.md) |Чтение свойств и связей объекта itemAttachment.|
|[Удаление](../api/attachment-delete.md) | Нет |Удаление объекта itemAttachment. |

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
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|item|[OutlookItem](outlookitem.md)|Вложенный контакт, сообщение или событие. Свойство навигации.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
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
