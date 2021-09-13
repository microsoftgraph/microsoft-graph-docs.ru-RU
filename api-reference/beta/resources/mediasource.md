---
author: MarcMroz
description: Ресурс mediaSource содержит метаданные об источнике элемента диска мультимедиа (аудио или видео).
title: Тип ресурса mediaSource
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: fac36dbd1112289e289b6f74ce16e5a971076e60
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59124114"
---
# <a name="mediasource-resouce-type"></a>тип resouce mediaSource

Ресурс **mediaSource содержит** метаданные об источнике диска мультимедиа (аудио или видео).

Он доступен в свойстве мультимедиа ресурсов [driveItem.][item-resource]

## <a name="properties"></a>Свойства

| Свойство                 | Тип                       | Описание                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| **contentCategory**      | mediaSourceContentCategory | Значение переумерия, которое указывает на категорию контента мультимедиа.                                     |

### <a name="mediasourcecontentcategory-values"></a>значения mediaSourceContentCategory

| Значение               | Описание                                         |
|:------------------- |:----------------------------------------------------|
| собрание             | Носители — это собрание.                             |
| liveStream          | Носители — это прямая трансляция.                         |
| презентация        | Носители — это презентация.                        |
| screenRecording     | Носители — это запись экрана.                    |
| unknownFutureValue  | Значение маркера для будущей совместимости.              |

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentCategory"
  ],
  "@odata.type": "microsoft.graph.mediaSource"
}-->

```json
{
  "contentCategory" : "string"
}
```

## <a name="see-also"></a>См. также

Дополнительные сведения о гранях на driveItem см. [в сайте driveItem.](driveitem.md)

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The mediaSource facet provides information about drive item source.",
  "keywords": "mediaSource,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/MediaSource"
} -->
