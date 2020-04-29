---
title: Тип ресурса Медиапромпт
description: Этот тип ресурса содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4bc2f315a2f339d2ef6fe0f4b76b335970b5a642
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447446"
---
# <a name="mediaprompt-resource-type"></a>Тип ресурса Медиапромпт

Пространство имен: microsoft.graph

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
