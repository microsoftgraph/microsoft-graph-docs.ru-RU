---
title: Тип ресурсов attendeeBase
description: Тип участника.
localization_priority: Normal
ms.openlocfilehash: d009ef6a58c63017addf8b8a1bdecc1974abbff3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878675"
---
# <a name="attendeebase-resource-type"></a>Тип ресурсов attendeeBase

Тип участника.

Тип, производный от [recipient](recipient.md).

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|type|attendeeType| Тип участника. Возможные значения: `required`, `optional`, `resource`. В настоящее время Если участник — это пользователь, [findMeetingTimes](../api/user-findmeetingtimes.md) всегда считает пользователя принадлежит `Required` типа.|
|emailAddress|[emailAddress](emailaddress.md)|Включает имя и SMTP-адрес участника.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
