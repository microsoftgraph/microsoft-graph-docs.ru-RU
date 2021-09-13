---
title: тип ресурса teamMemberSettings
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 215efff423e417d83f2416021b877c8d0c08897e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049496"
---
# <a name="teammembersettings-resource-type"></a>тип ресурса teamMemberSettings

Пространство имен: microsoft.graph



Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команде.](team.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowCreatePrivateChannels|Логический|Если установлено, что это так, участники могут добавлять и обновлять частные каналы.|
|allowCreateUpdateChannels|Boolean|Если установлено, что это так, участники могут добавлять и обновлять каналы.|
|allowDeleteChannels|Логический|Если установлено, что это так, участники могут удалять каналы.|
|allowAddRemoveApps|Логический|Если установлено, что это так, участники могут добавлять и удалять приложения.|
|allowCreateUpdateRemoveTabs|Логический|Если установлено true, участники могут добавлять, обновлять и удалять вкладки. |
|allowCreateUpdateRemoveConnectors|Логический|Если установлено верно, участники могут добавлять, обновлять и удалять соединители.|

## <a name="json-representation"></a>Представление в формате JSON

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

