---
title: тип ресурса teamGuestSettings
description: Параметры для настройки того, могут ли гости создавать, изменять или удалять каналы в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8b8c0a47135af606d2bfb83d190bd88d6af4ad65356c99096563f76053f9a9ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146358"
---
# <a name="teamguestsettings-resource-type"></a>тип ресурса teamGuestSettings

Пространство имен: microsoft.graph



Параметры настроить, могут ли гости создавать, обновлять или удалять каналы в [команде.](team.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Логический|Если установлено, что это так, гости могут добавлять и обновлять каналы.|
|allowDeleteChannels|Логическое|Если установлено, что это так, гости могут удалять каналы.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

