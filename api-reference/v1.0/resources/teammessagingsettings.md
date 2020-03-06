---
title: Тип ресурса Теаммессагингсеттингс
description: Параметры для настройки обмена сообщениями и упоминаний в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e742dd0e785a94b33a57e55b50a00aab0c207ab4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533522"
---
# <a name="teammessagingsettings-resource-type"></a>Тип ресурса Теаммессагингсеттингс

Пространство имен: microsoft.graph



Параметры для настройки обмена сообщениями и упоминаний в [команде](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|алловусередитмессажес|Boolean|Если задано значение true, пользователи могут редактировать сообщения.|
|алловусерделетемессажес|Boolean|Если задано значение true, пользователи могут удалять свои сообщения.|
|аллововнерделетемессажес|Boolean|Если задано значение true, владельцы могут удалять любые сообщения.|
|алловтеамментионс|Boolean|Если задано значение true, @team упоминаний разрешены.|
|алловчаннелментионс|Boolean|Если задано значение true, @channel упоминаний разрешены.|

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
