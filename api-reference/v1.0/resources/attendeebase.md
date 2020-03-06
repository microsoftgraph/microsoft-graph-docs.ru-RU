---
title: Тип ресурсов attendeeBase
description: Тип участника.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a7eaf030413e576721bd672fc63111a62742c163
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532071"
---
# <a name="attendeebase-resource-type"></a>Тип ресурсов attendeeBase

Пространство имен: microsoft.graph

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
|type|attendeeType| Тип участника. Допустимые значения: `required`, `optional`, `resource`. Если участник является пользователем, то [findMeetingTimes](../api/user-findmeetingtimes.md) всегда определяет тип этого пользователя как `Required`.|
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
