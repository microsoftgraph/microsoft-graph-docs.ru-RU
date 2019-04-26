---
title: Тип ресурса Теаммессагингсеттингс
description: Параметры для настройки обмена сообщениями и упоминаний в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 48d9281a032bebd9d65936cbf9effd78416ffc7d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341471"
---
# <a name="teammessagingsettings-resource-type"></a>Тип ресурса Теаммессагингсеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры для настройки обмена сообщениями и упоминаний в [команде](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Алловусередитмессажес|Логический|Если задано значение true, пользователи могут редактировать сообщения.|
|Алловусерделетемессажес|Логический|Если задано значение true, пользователи могут удалять свои сообщения.|
|Аллововнерделетемессажес|Логический|Если задано значение true, владельцы могут удалять любые сообщения.|
|Алловтеамментионс|Логический|Если задано значение true, @team упоминаний разрешены.|
|Алловчаннелментионс|Логический|Если задано значение true, @channel упоминаний разрешены.|

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
<!--
{
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
