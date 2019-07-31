---
title: Тип ресурса Митингкапабилити
description: Содержит возможности собрания
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1de406cf0614a4cbb64749cef763a97a3723eb48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966868"
---
# <a name="meetingcapability-resource-type"></a>Тип ресурса Митингкапабилити

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит возможности собрания

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| Аллованонимаусусерстодиалаут      | Boolean | Указывает, разрешено ли исходящие вызовы анонимных пользователей на собрании. |
| Аллованонимаусусерстостартмитинг | Boolean | Указывает, разрешено ли анонимным пользователям начинать собрание.  |
| Аутоадмиттедусерс                 | String  | Возможные значения: `everyoneInCompany`, `everyone`.              |

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
