---
title: Тип ресурса teamMemberSettings
description: Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, рабочих групп.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 3854481e89f04fa727b77c6b4f8699c62a16d739
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978251"
---
# <a name="teammembersettings-resource-type"></a>Тип ресурса teamMemberSettings

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, в [группы](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Логический|Если параметр имеет значение true, участники могли добавлять и обновлять каналов.|
|allowDeleteChannels|Логический|Если параметр имеет значение true, участники могут удалять каналы.|
|allowAddRemoveApps|Логический|Если параметр имеет значение true, участники могут добавлять и удалять приложения.|
|allowCreateUpdateRemoveTabs|Логический|Если параметр имеет значение true, участники могут добавлять, обновлять и удалять вкладки. |
|allowCreateUpdateRemoveConnectors|Логический|Если параметр имеет значение true, участники могут добавлять, обновлять и удалять соединители.|

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
