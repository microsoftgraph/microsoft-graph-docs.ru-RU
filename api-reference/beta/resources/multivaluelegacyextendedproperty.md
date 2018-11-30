---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
ms.openlocfilehash: efb871594028b5c2d54b1c081f901717b754c8ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078694"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a>Тип ресурса multiValueLegacyExtendedProperty

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Расширенное свойство, содержащее коллекцию значений.

Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Post](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | Поддерживаемые ресурсов экземпляра: [сообщения](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md)или [папки задач Outlook](../resources/outlooktaskfolder.md). Обратите внимание, что, группа [записи](../resources/post.md) не поддерживается. | Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса. |
|[Get](../api/multivaluelegacyextendedproperty-get.md) |Экземпляр поддерживаемые ресурсов ([сообщение](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md), [папки задач Outlook](../resources/outlooktaskfolder.md)или группа [учета](../resources/post.md)), включающим [ multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) объекта. |Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|строка|Идентификатор свойства. Только для чтения.|
|value|Коллекция строк|Коллекция значений свойств.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.multivaluelegacyextendedproperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->