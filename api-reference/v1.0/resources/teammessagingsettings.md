---
title: тип ресурса teamMessagingSettings
description: Параметры для настройки обмена сообщениями и упоминаний в команде.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 08af21e988862a4d6b459953e6d1a1fd5554da36
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049489"
---
# <a name="teammessagingsettings-resource-type"></a>тип ресурса teamMessagingSettings

Пространство имен: microsoft.graph



Параметры настраивать сообщения и упоминания в [команде.](team.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowUserEditMessages|Логический|Если установлено, что это так, пользователи могут изменять свои сообщения.|
|allowUserDeleteMessages|Boolean|Если установлено, что это так, пользователи могут удалять свои сообщения.|
|allowOwnerDeleteMessages|Логический|Если установлено, что это правда, владельцы могут удалить любое сообщение.|
|allowTeamMentions|Boolean|Если установлено, @team разрешены упоминания.|
|allowChannelMentions|Логический|Если установлено, @channel разрешены упоминания.|

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

