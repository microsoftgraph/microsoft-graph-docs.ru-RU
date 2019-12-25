---
title: Тип ресурса Медиастреам
description: Содержит сведения о канале мультимедиа.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: de5c90453d9adb657c2df5ee761d847056664037
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870182"
---
# <a name="mediastream-resource-type"></a>Тип ресурса Медиастреам

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о канале мультимедиа.

## <a name="properties"></a>Свойства

| Свойство    | Тип    | Описание                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | Направление. `inactive`Возможные значения: `sendOnly`,, `receiveOnly`,. `sendReceive`                  |
| label       | String  | Метка потока мультимедиа.                                                                                       |
| mediaType   | String  | Тип мультимедиа. Возможные `unknown`значения:, `audio` `video`,, `videoBasedScreenSharing`,. `data`        |
| сервермутед | Логический | Указывает, отключен ли сервер к мультимедиа.                                                                          |
| Идентификатор    | String  | Идентификатор источника.                                                                                                |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted",
    "label"
  ],
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "inactive | sendOnly | receiveOnly | sendReceive",
  "label": "String",
  "mediaType": "unknown | audio | video | videoBasedScreenSharing | data",
  "serverMuted": true,
  "sourceId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
