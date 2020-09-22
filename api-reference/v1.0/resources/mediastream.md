---
title: Тип ресурса Медиастреам
description: Тип Медиастреам.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1158dfb01b9e92c5dc97f34bef3bb3661da51b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088491"
---
# <a name="mediastream-resource-type"></a>Тип ресурса Медиастреам

Пространство имен: microsoft.graph

Содержит сведения о канале мультимедиа.

## <a name="properties"></a>Свойства

| Свойство    | Тип    | Описание                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | Направление. Возможные значения: `inactive` ,, `sendOnly` `receiveOnly` , `sendReceive` .                  |
| label       | Строка  | Метка потока мультимедиа.                                                                                       |
| MediaType   | Строка  | Тип мультимедиа. Возможные значения:,,, `unknown` `audio` `video` `videoBasedScreenSharing` , `data` .        |
| сервермутед | Boolean | Если сервер отключен на носителе.                                                                          |
| Идентификатор    | Строка  | Идентификатор источника.                                                                                                |

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

