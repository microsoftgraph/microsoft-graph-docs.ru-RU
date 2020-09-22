---
title: Тип ресурса Митингкапабилити
description: Содержит возможности собрания
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 29da5c8d4796e393bfead08979aca8e58a95024d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971687"
---
# <a name="meetingcapability-resource-type"></a>Тип ресурса Митингкапабилити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит возможности собрания

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| аллованонимаусусерстодиалаут      | Boolean | Указывает, разрешено ли исходящие вызовы анонимных пользователей на собрании. |
| аллованонимаусусерстостартмитинг | Boolean | Указывает, разрешено ли анонимным пользователям начинать собрание.  |
| аутоадмиттедусерс                 | String  | Возможные значения: `everyoneInCompany`, `everyone`.              |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


