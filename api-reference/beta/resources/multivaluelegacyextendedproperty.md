---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 4ccfdc6fd703673cdd71284cf3ad367f94efdc5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021282"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a>Тип ресурса multiValueLegacyExtendedProperty

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Расширенное свойство, содержащее коллекцию значений.

Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Post](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | Поддерживаемый экземпляр ресурса: [Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task](../resources/outlooktask.md)или [Outlook Task](../resources/outlooktaskfolder.md). Обратите внимание, что ресурсы [post](../resources/post.md) групп не поддерживаются. | Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса. |
|[Получение](../api/multivaluelegacyextendedproperty-get.md) |Поддерживаемый экземпляр ресурса ([Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task Task](../resources/outlooktask.md), [Outlook Task Folder](../resources/outlooktaskfolder.md)или POST Group [POST](../resources/post.md)), дополненный объектом [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) . |Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.|

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


