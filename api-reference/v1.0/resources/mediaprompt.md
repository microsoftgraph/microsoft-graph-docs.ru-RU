---
title: Тип ресурса Медиапромпт
description: Этот тип ресурса содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f981559ce5bac9bb597e49ff1b9d31e48413454b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871394"
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
