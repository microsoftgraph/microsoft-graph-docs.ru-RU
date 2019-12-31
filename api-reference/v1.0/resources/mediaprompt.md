---
title: Тип ресурса Медиапромпт
description: Этот тип ресурса содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0ef83d9645ac4277893ff8c769ecb6e092e3e84d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913200"
---
# <a name="mediaprompt-resource-type"></a>Тип ресурса Медиапромпт

Этот тип ресурса содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.

## <a name="properties"></a>Свойства

| Свойство    | Тип                      | Описание                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| медиаинфо   | [медиаинфо](mediainfo.md) | Сведения о мультимедиа                                                           |

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
