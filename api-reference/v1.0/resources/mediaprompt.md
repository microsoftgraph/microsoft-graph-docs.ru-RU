---
title: тип ресурса mediaPrompt
description: Этот тип ресурса содержит сведения о звуковом файле, который будет играть, и других дополнительных параметрах.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b69111bda37ce59305aaf126225f974c25721ceb7ed0ac34af71c1f9bf743438
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141436"
---
# <a name="mediaprompt-resource-type"></a>тип ресурса mediaPrompt

Пространство имен: microsoft.graph

Этот тип ресурса содержит сведения о звуковом файле, который будет играть, и других дополнительных параметрах.

## <a name="properties"></a>Свойства

| Свойство    | Тип                      | Описание                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| mediaInfo   | [mediaInfo](mediainfo.md) | Сведения о средствах массовой информации                                                           |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

