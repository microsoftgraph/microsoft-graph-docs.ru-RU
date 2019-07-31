---
title: Тип ресурса Медиаконфиг
description: Конфигурация мультимедиа, используемая для подключения к вызову.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4d00470d517c4d701a028a1911efe02a6f441639
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009778"
---
# <a name="mediaconfig-resource-type"></a>Тип ресурса Медиаконфиг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Конфигурация мультимедиа, используемая для подключения к вызову.

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание|
|:---------------|:--------|:----------|
| Ремовефромдефаултаудиограуп | Boolean |  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
   ],
  "abstract": true,
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
