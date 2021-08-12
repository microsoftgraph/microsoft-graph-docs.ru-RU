---
title: Тип ресурса mediaStream
description: Тип mediaStream.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 98fa09655faa6068c48c6fe2d1e340fa28ff253b99717900bed5d9f863561c1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141443"
---
# <a name="mediastream-resource-type"></a>Тип ресурса mediaStream

Пространство имен: microsoft.graph

Это содержит сведения о канале мультимедиа.

## <a name="properties"></a>Свойства

| Свойство    | Тип    | Описание                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | Направление. Возможные значения `inactive` , `sendOnly` , `receiveOnly` `sendReceive` .                  |
| label       | String  | Метка потока мультимедиа.                                                                                       |
| MediaType   | String  | Тип мультимедиа. Возможное значение `unknown` , , , `audio` `video` `videoBasedScreenSharing` `data` .        |
| serverMuted | Логическое | Если мультимедиа отключено сервером.                                                                          |
| sourceId    | String  | Исходный код.                                                                                                |

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

