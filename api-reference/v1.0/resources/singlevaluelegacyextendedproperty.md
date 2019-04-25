---
title: Тип ресурса singleValueLegacyExtendedProperty
description: 'Расширенное свойство, содержащее одно значение. '
localization_priority: Normal
ms.openlocfilehash: f865da1a8a4211ac99a70881b2851b38b8e72727
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549645"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a>Тип ресурса singleValueLegacyExtendedProperty

Расширенное свойство, содержащее одно значение. 

Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md). 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | Экземпляр поддерживаемого ресурса: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) или [contactFolder](../resources/contactfolder.md), но не [post](../resources/post.md) группы. | Создание объекта **singleValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса. |
|[Получение](../api/singlevaluelegacyextendedproperty-get.md) |Один или несколько экземпляров поддерживаемого ресурса ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) или [post](../resources/post.md) группы) либо один такой экземпляр, расширенный объектом [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md). |Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand` или `$filter`.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string|Идентификатор свойства. Только для чтения.|
|значение|string|Значение свойства.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
