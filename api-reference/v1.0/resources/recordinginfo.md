---
title: Тип ресурса Рекордингинфо
description: Представляет сведения о записи для участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b7044f13f16a9d1126a5b1c72cdc86c3527f6b37
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543270"
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
  "initiator": {"@odata.type": "#microsoft.graph.identitySet"},
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
