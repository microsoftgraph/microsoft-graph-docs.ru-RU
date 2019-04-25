---
title: Тип ресурса Теаммессагингсеттингс
description: Параметры для настройки обмена сообщениями и упоминаний в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d98dfa3c2306cabb99b6de96aed2010cefa10717
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553950"
---
# <a name="teammessagingsettings-resource-type"></a>Тип ресурса Теаммессагингсеттингс



Параметры для настройки обмена сообщениями и упоминаний в [команде](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Алловусередитмессажес|Логический|Если задано значение true, пользователи могут редактировать сообщения.|
|Алловусерделетемессажес|Логический|Если задано значение true, пользователи могут удалять свои сообщения.|
|Аллововнерделетемессажес|Логический|Если задано значение true, владельцы могут удалять любые сообщения.|
|Алловтеамментионс|Логический|Если задано значение true, @team упоминаний разрешены.|
|Алловчаннелментионс|Логический|Если задано значение true, @channel упоминаний разрешены.|

## <a name="json-representation"></a>Представление в формате JSON

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
