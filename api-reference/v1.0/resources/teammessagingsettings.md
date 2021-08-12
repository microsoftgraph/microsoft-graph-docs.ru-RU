---
title: тип ресурса teamMessagingSettings
description: Параметры для настройки обмена сообщениями и упоминаний в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9818e161e21f78a83023ead66d7b790eadd01bb2737942a383665338d0ec73c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129962"
---
# <a name="teammessagingsettings-resource-type"></a>тип ресурса teamMessagingSettings

Пространство имен: microsoft.graph



Параметры настраивать сообщения и упоминания в [команде.](team.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowUserEditMessages|Логический|Если установлено, что это так, пользователи могут изменять свои сообщения.|
|allowUserDeleteMessages|Логическое|Если установлено, что это так, пользователи могут удалять свои сообщения.|
|allowOwnerDeleteMessages|Логический|Если установлено, что это правда, владельцы могут удалить любое сообщение.|
|allowTeamMentions|Логическое|Если установлено, @team разрешены упоминания.|
|allowChannelMentions|Логическое|Если установлено, @channel разрешены упоминания.|

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

