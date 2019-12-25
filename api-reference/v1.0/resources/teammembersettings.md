---
title: Тип ресурса Теаммемберсеттингс
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1c1485bbc43588b8144cbe1cc7cb189f9b8c9fdc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863780"
---
# <a name="teammembersettings-resource-type"></a>Тип ресурса Теаммемберсеттингс



Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команду](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|алловкреатеприватечаннелс|Логический|Если задано значение true, участники могут добавлять и обновлять частные каналы.|
|алловкреатеупдатечаннелс|Логический|Если задано значение true, участники могут добавлять и обновлять каналы.|
|алловделетечаннелс|Логический|Если задано значение true, участники могут удалять каналы.|
|алловаддремовеаппс|Логический|Если задано значение true, участники могут добавлять и удалять приложения.|
|алловкреатеупдатеремоветабс|Логический|Если задано значение true, члены могут добавлять, обновлять и удалять вкладки. |
|алловкреатеупдатеремовеконнекторс|Логический|Если задано значение true, участники могут добавлять, обновлять и удалять соединители.|

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
