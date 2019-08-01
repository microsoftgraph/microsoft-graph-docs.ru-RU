---
title: Тип ресурса Теаммемберсеттингс
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d657b8f022395c24d27df56442c164731215a04e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033854"
---
# <a name="teammembersettings-resource-type"></a>Тип ресурса Теаммемберсеттингс



Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команду](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Алловкреатеупдатечаннелс|Boolean|Если задано значение true, участники могут добавлять и обновлять каналы.|
|Алловделетечаннелс|Boolean|Если задано значение true, участники могут удалять каналы.|
|Алловаддремовеаппс|Boolean|Если задано значение true, участники могут добавлять и удалять приложения.|
|Алловкреатеупдатеремоветабс|Boolean|Если задано значение true, члены могут добавлять, обновлять и удалять вкладки. |
|Алловкреатеупдатеремовеконнекторс|Boolean|Если задано значение true, участники могут добавлять, обновлять и удалять соединители.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
