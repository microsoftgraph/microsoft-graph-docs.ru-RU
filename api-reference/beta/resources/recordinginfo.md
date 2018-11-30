---
title: Тип ресурса recordingInfo
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 92af3fcb52ab08f3f25a2c16cc720a4053a9bdfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078132"
---
# <a name="recordinginfo-resource-type"></a>Тип ресурса recordingInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Description|
|:---------------|:--------|:----------|
| initiatedBy | [participantInfo](participantinfo.md) | Участник, который инициировал записи. |
| status | String | Возможные значения: `recordingCapable`, `notRecording`, `startedRecording`. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "status": "recordingCapable | notRecording | startedRecording"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
