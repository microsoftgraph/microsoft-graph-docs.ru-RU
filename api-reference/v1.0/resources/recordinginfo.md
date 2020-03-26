---
title: Тип ресурса Рекордингинфо
description: Представляет сведения о записи для участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6a41195705a46ac46bd085f3b4a655943b730ad3
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962568"
---
# <a name="recordinginfo-resource-type"></a>Тип ресурса Рекордингинфо

Пространство имен: microsoft.graph

Представляет сведения о записи для участника.

## <a name="properties"></a>Свойства

| Свойство        | Тип    | Описание|
|:----------------|:--------|:----------|
| initiator     | [identitySet](identitySet.md) | Идентификаторы инициатора записи. |
| рекордингстатус | String | `unknown`Возможные значения: `notRecording`,, `recording`, или. `failed` |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "initiator"
  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "recordingStatus": "unknown | notRecording | recording | failed"
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
