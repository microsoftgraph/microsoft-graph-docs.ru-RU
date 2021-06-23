---
title: тип ресурса teamMemberSettings
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dfa463ce47b9724d18f6f13b53ef46a1cb493f4a
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060455"
---
# <a name="teammembersettings-resource-type"></a>тип ресурса teamMemberSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команде.](team.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Boolean|Если установлено, что это так, участники могут добавлять и обновлять любые каналы.|
|allowCreatePrivateChannels|Boolean|Если установлено, что это так, участники могут добавлять и обновлять частные каналы.|
|allowDeleteChannels|Boolean|Если установлено, что это так, участники могут удалять каналы.|
|allowAddRemoveApps|Boolean|Если установлено, что это так, участники могут добавлять и удалять приложения.|
|allowCreateUpdateRemoveTabs|Boolean|Если установлено true, участники могут добавлять, обновлять и удалять вкладки. |
|allowCreateUpdateRemoveConnectors|Boolean|Если установлено верно, участники могут добавлять, обновлять и удалять соединители.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowCreatePrivateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


