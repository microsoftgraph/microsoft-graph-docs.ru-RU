---
title: Тип ресурса teamMessagingSettings
description: Параметры для настройки системы обмена сообщениями и упоминания рабочих групп.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06aca84355a07052dcea316145dfff437eee743b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848260"
---
# <a name="teammessagingsettings-resource-type"></a>Тип ресурса teamMessagingSettings

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Параметры для настройки системы обмена сообщениями и упоминания в [группы](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowUserEditMessages|Логический|Если параметр имеет значение true, пользователи могут изменять свои сообщения;|
|allowUserDeleteMessages|Логический|Если параметр имеет значение true, пользователи могут удалять свои сообщения.|
|allowOwnerDeleteMessages|Логический|Если параметр имеет значение true, владельцы могут удалять все сообщения.|
|allowTeamMentions|Логический|Если задано значение true, допускаются упоминания @team.|
|allowChannelMentions|Логический|Если задано значение true, допускаются упоминания @channel.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
