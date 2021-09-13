---
title: тип ресурса recordingInfo
description: Представляет сведения о записи для участника.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 54e230ca6844d974cf918325aab48e898d87e08b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078653"
---
# <a name="recordinginfo-resource-type"></a>тип ресурса recordingInfo

Пространство имен: microsoft.graph

Представляет сведения о записи для участника.

## <a name="properties"></a>Свойства

| Свойство        | Тип    | Описание|
|:----------------|:--------|:----------|
| initiator     | [identitySet](identitySet.md) | Удостоверения инициатора записи. |
| recordingStatus | Строка | Возможные значения: `unknown` `notRecording` , , , или `recording` `failed` . |

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

