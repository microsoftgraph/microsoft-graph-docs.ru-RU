---
title: Тип ресурса Теаммемберсеттингс
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d75ae8d97d3d2c95cc1779e38346efeea3026f23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533531"
---
# <a name="teammembersettings-resource-type"></a>Тип ресурса Теаммемберсеттингс

Пространство имен: microsoft.graph



Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команду](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|алловкреатеприватечаннелс|Boolean|Если задано значение true, участники могут добавлять и обновлять частные каналы.|
|алловкреатеупдатечаннелс|Boolean|Если задано значение true, участники могут добавлять и обновлять каналы.|
|алловделетечаннелс|Boolean|Если задано значение true, участники могут удалять каналы.|
|алловаддремовеаппс|Boolean|Если задано значение true, участники могут добавлять и удалять приложения.|
|алловкреатеупдатеремоветабс|Boolean|Если задано значение true, члены могут добавлять, обновлять и удалять вкладки. |
|алловкреатеупдатеремовеконнекторс|Boolean|Если задано значение true, участники могут добавлять, обновлять и удалять соединители.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreatePrivateChannels": true,
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
