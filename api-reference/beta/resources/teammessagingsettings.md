---
title: Тип ресурса Теаммессагингсеттингс
description: Параметры для настройки обмена сообщениями и упоминаний в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 352fc5bc8a8794a455a84d729bb3b2cea6ad34f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046632"
---
# <a name="teammessagingsettings-resource-type"></a>Тип ресурса Теаммессагингсеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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


