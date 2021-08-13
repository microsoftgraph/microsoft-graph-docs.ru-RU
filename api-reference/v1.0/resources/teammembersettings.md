---
title: тип ресурса teamMemberSettings
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0383392f47c7f386e20860ad83ba090ce9ebe7244e62e19397525dcf7835c0dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189284"
---
# <a name="teammembersettings-resource-type"></a>тип ресурса teamMemberSettings

Пространство имен: microsoft.graph



Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команде.](team.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowCreatePrivateChannels|Логический|Если установлено, что это так, участники могут добавлять и обновлять частные каналы.|
|allowCreateUpdateChannels|Логическое|Если установлено, что это так, участники могут добавлять и обновлять каналы.|
|allowDeleteChannels|Логическое|Если установлено, что это так, участники могут удалять каналы.|
|allowAddRemoveApps|Логический|Если установлено, что это так, участники могут добавлять и удалять приложения.|
|allowCreateUpdateRemoveTabs|Логическое|Если установлено true, участники могут добавлять, обновлять и удалять вкладки. |
|allowCreateUpdateRemoveConnectors|Логическое|Если установлено верно, участники могут добавлять, обновлять и удалять соединители.|

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

