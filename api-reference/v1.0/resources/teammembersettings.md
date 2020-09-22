---
title: Тип ресурса Теаммемберсеттингс
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7087457ac68c98b40b1c89dc4b99b13ae85d46b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094010"
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

