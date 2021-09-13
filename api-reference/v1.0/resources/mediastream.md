---
title: Тип ресурса mediaStream
description: Тип mediaStream.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4fa45c863bf06d2c1c2083a1f66796abcb46eaff
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134607"
---
# <a name="mediastream-resource-type"></a>Тип ресурса mediaStream

Пространство имен: microsoft.graph

Это содержит сведения о канале мультимедиа.

## <a name="properties"></a>Свойства

| Свойство    | Тип    | Описание                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | Направление. Возможные значения `inactive` , `sendOnly` , `receiveOnly` `sendReceive` .                  |
| подпись       | String  | Метка потока мультимедиа.                                                                                       |
| MediaType   | Строка  | Тип мультимедиа. Возможное значение `unknown` , , , `audio` `video` `videoBasedScreenSharing` `data` .        |
| serverMuted | Boolean | Если мультимедиа отключено сервером.                                                                          |
| sourceId    | Строка  | Исходный код.                                                                                                |

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

