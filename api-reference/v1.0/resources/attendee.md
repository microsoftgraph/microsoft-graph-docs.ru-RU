---
title: Тип ресурса attendee
description: Участник события. Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6c90d086afb7716dc3696443f18931f17cb291d9
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427244"
---
# <a name="attendee-resource-type"></a>Тип ресурса attendee

Пространство имен: microsoft.graph

Участник события. Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.

Тип, производный от [attendeeBase](attendeebase.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|emailAddress|[emailAddress](emailaddress.md)|Включает имя и SMTP-адрес участника.|
|пропоседневтиме|[timeSlot](timeslot.md)|Альтернативная дата/время, предлагаемая участником для начала и конца приглашения на собрание. Если участник не предложил другое время, это свойство не включается в ответ на событие GET.|
|status|[ResponseStatus](responsestatus.md)|Ответ участника (нет, принято, отклонено и т. д.) на событие, а также дата и время отправки ответа.|
|type|String|Тип участника: `required`, `optional`, `resource`.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
  "optionalProperties": [
   "proposedNewTime"
  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "proposedNewTime": {"@odata.type": "microsoft.graph.timeSlot"},
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
