---
title: Тип ресурса singleValueLegacyExtendedProperty
description: 'Расширенное свойство, содержащее одно значение. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 578b2792a815dd0c7cd5dad4fc77d9c96319045a
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334586"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a>Тип ресурса singleValueLegacyExtendedProperty

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Расширенное свойство, содержащее одно значение.

Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Post](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | Поддерживаемый экземпляр [ресурса:](../resources/message.md)сообщение , [mailFolder](../resources/mailfolder.md) [,](../resources/event.md)событие [,](../resources/calendar.md)календарь [,](../resources/contact.md)контакт , [contactFolder](../resources/contactfolder.md), [Outlook](../resources/outlooktask.md)задачи , или Outlook папку задач [,](../resources/outlooktaskfolder.md)но не групповую [должность](../resources/post.md). | Создание объекта **singleValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса. |
|[Получение](../api/singlevaluelegacyextendedproperty-get.md) |Один или коллекция поддерживаемых экземпляров ресурсов[(сообщение](../resources/message.md), [mailFolder](../resources/mailfolder.md) [,](../resources/event.md)событие [,](../resources/calendar.md)календарь [,](../resources/contact.md)контакт , [contactFolder](../resources/contactfolder.md), [Outlook](../resources/outlooktask.md)задача , [Outlook](../resources/outlooktaskfolder.md)папка задачи , или групповой пост [),](../resources/post.md)или один такой экземпляр, расширенный с одним [объектомValueLegacyExtendedProperty.](singlevaluelegacyextendedproperty.md) |Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand` или `$filter`.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string|Идентификатор свойства. Только для чтения.|
|значение|string|Значение свойства.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


