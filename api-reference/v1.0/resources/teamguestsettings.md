---
title: тип ресурса teamGuestSettings
description: Параметры для настройки того, могут ли гости создавать, изменять или удалять каналы в команде.
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 769930b28366b9918a92b9839331a421db5ff79a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134341"
---
# <a name="teamguestsettings-resource-type"></a>тип ресурса teamGuestSettings

Пространство имен: microsoft.graph



Параметры настроить, могут ли гости создавать, обновлять или удалять каналы в [команде.](team.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Логический|Если установлено, что это так, гости могут добавлять и обновлять каналы.|
|allowDeleteChannels|Логический|Если установлено, что это так, гости могут удалять каналы.|

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

