---
title: Тип ресурса singleValueLegacyExtendedProperty
description: 'Расширенное свойство, содержащее одно значение. '
localization_priority: Normal
ms.openlocfilehash: 0d889756204853a525269f28cfdd3cc1b40be8a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512369"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a>Тип ресурса singleValueLegacyExtendedProperty

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Расширенное свойство, содержащее одно значение. 

Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md). 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Post](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | Поддерживаемые ресурсов экземпляра: [сообщения](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md)или [папки задач Outlook](../resources/outlooktaskfolder.md), но не группа [учета](../resources/post.md). | Создание объекта **singleValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса. |
|[Получение](../api/singlevaluelegacyextendedproperty-get.md) |Один или коллекцию поддерживаемых ресурсов экземпляра ([сообщение](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md), [папки задач Outlook](../resources/outlooktaskfolder.md)или группа [учета](../resources/post.md)), или один экземпляр, включающим объект [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) . |Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand` или `$filter`.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string|Идентификатор свойства. Только для чтения.|
|value|строка|Значение свойства.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/singlevaluelegacyextendedproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
