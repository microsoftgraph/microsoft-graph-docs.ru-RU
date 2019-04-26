---
title: Тип ресурса Митингкапабилити
description: Содержит возможности собрания
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 55a577490ee4c40bbd4adcc63a7e4aa7f38c8dd1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342600"
---
# <a name="meetingcapability-resource-type"></a>Тип ресурса Митингкапабилити

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит возможности собрания

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| Аллованонимаусусерстодиалаут      | Логический | Указывает, разрешено ли исходящие вызовы анонимных пользователей на собрании. |
| Аллованонимаусусерстостартмитинг | Логический | Указывает, разрешено ли анонимным пользователям начинать собрание.  |
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
