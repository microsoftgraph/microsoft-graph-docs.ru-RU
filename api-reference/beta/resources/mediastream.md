---
title: Тип ресурса mediaStream
description: Тип mediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd003bde0eca5fd21cb12c23d5c83699a6b79c8e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916966"
---
# <a name="mediastream-resource-type"></a>Тип ресурса mediaStream

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Тип mediaStream.

## <a name="properties"></a>Свойства

| Свойство    | Тип    | Описание                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| Направление   | String  | Направление. Возможные значения: `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.                  |
| label       | String  | Метка потока мультимедиа.                                                                                       |
| Тип носителя   | String  | Тип носителя. Возможное значение — `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.        |
| serverMuted | Boolean | Если мультимедиа отключен на сервере.                                                                          |
| sourceId    | String  | Исходный код.                                                                                                |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted"
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

## <a name="example"></a>Пример

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "sendReceive",
  "label": "main-audio",
  "mediaType": "audio",
  "serverMuted": false,
  "sourceId": "1024"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
