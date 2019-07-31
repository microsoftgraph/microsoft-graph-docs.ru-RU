---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2ace395b336a0950c814a4eb65103de440f59305
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966708"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a>Тип ресурса multiValueLegacyExtendedProperty

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Расширенное свойство, содержащее коллекцию значений.

Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Post](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | Поддерживаемый экземпляр ресурса: [Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task](../resources/outlooktask.md)или [Outlook Task](../resources/outlooktaskfolder.md). Обратите внимание, что ресурсы [post](../resources/post.md) групп не поддерживаются. | Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса. |
|[Получение](../api/multivaluelegacyextendedproperty-get.md) |Поддерживаемый экземпляр ресурса ([Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task Task](../resources/outlooktask.md), [Outlook Task Folder](../resources/outlooktaskfolder.md)или POST Group [POST](../resources/post.md)), дополненный [ Объект multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) . |Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string|Идентификатор свойства. Только для чтения.|
|значение|Коллекция строк|Коллекция значений свойств.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
