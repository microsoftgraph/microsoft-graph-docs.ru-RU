---
author: MarcMroz
description: Медиаресум содержит метаданные о элементе диска мультимедиа (аудио или видео).
title: тип медиаресумов
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 3dd985c7259088f41412ea5d579c1e49d99acf4c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091204"
---
# <a name="media-resouce-type"></a>тип повторного окантовки мультимедиа

Содержит метаданные о элементе диска мультимедиа (аудио или видео).

Он доступен в свойстве мультимедиа ресурсов [driveItem.][item-resource]


## <a name="properties"></a>Свойства

| Свойство                 | Тип                  | Описание                                                                                                   |
| :----------------------- | :-------------------- | :------------------------------------------------------------------------------------------------------------ 
| **isTranscriptionShown** | Логическое               | Если файл имеет стенограмму, этот параметр управляет, если закрытые подписи /транскрипция для файла мультимедиа должны быть показаны людям во время просмотра. Read-Write.                                                    |
| **mediaSource**          | [mediaSource](mediaSource.md)         | Сведения об источнике мультимедиа. Только для чтения.                                                             | 


## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.media"
}-->

```json
{
  "isTranscriptionShown" : true,
  "mediaSource": { "@odata.type": "microsoft.graph.mediaSource" }
}
```

## <a name="see-also"></a>См. также 

Дополнительные сведения о гранях на driveItem см. [в сайте driveItem.](driveitem.md)

[item-resource]: ../resources/driveitem.md
[mediaSource]: mediaSource.md

<!-- {
  "type": "#page.annotation",
  "description": "The media resource type provides information about the media item.",
  "keywords": "mediaItem,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/Media"
} -->
