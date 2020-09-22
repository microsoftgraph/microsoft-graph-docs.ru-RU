---
title: Тип ресурса Медиастреам
description: Содержит сведения о канале мультимедиа.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 37ed8ce10f62888a7bf1be67f489c6b8a0b95c76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971736"
---
# <a name="mediastream-resource-type"></a>Тип ресурса Медиастреам

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о канале мультимедиа.

## <a name="properties"></a>Свойства

| Свойство    | Тип    | Описание                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | Направление. Возможные значения: `inactive` ,, `sendOnly` `receiveOnly` , `sendReceive` .                  |
| label       | String  | Метка потока мультимедиа.                                                                                       |
| MediaType   | String  | Тип мультимедиа. Возможные значения:,,, `unknown` `audio` `video` `videoBasedScreenSharing` , `data` .        |
| сервермутед | Boolean | Указывает, отключен ли сервер к мультимедиа.                                                                          |
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


