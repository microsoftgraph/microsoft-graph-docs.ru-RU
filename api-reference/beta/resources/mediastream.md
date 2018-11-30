---
title: Тип ресурса mediaStream
description: Тип mediaStream.
ms.openlocfilehash: 28eb98a3ab1be67c60c6ebd35deb7618f1618be3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082392"
---
# <a name="mediastream-resource-type"></a>Тип ресурса mediaStream

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Тип mediaStream.

## <a name="properties"></a>Свойства

| Свойство    | Тип    | Description                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| Направление   | String  | Направление. Возможные значения: `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.                  |
| label       | String  | Метка потока мультимедиа.                                                                                       |
| Тип носителя   | String  | Тип носителя. Возможное значение — `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.        |
| serverMuted | Логический | Если мультимедиа отключен на сервере.                                                                          |
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
