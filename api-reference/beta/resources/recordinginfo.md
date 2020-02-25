---
title: Тип ресурса Рекордингинфо
description: Сведения о записи для участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 644ba7fbd762acde7f5229d15267de5352f03ca8
ms.sourcegitcommit: 6144934d4f6cf8c9797aa19e62285217220c7f45
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268317"
---
# <a name="recordinginfo-resource-type"></a>Тип ресурса Рекордингинфо

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о записи для участника.

## <a name="properties"></a>Свойства

| Свойство        | Тип    | Описание|
|:----------------|:--------|:----------|
| initiatedBy     | [participantInfo](participantinfo.md) | Участник, который инициировал запись. |
| рекордингстатус | Строка | `unknown`Возможные значения: `notRecording`,, `recording`, или. `failed` |
| initiator | [identitySet](identitySet.md) | Идентификаторы инициатора записи. |

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
  "recordingStatus": "unknown | notRecording | recording | failed",
  "initiator": {"@odata.type": "#microsoft.graph.initiator"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
