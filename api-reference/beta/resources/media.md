---
author: MarcMroz
description: Медиаресум содержит метаданные о элементе диска мультимедиа (аудио или видео).
title: тип медиаресумов
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 488201407363469ff09220c1dcce3c15f02e3b93
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236339"
---
# <a name="media-resouce-type"></a>тип повторного окантовки мультимедиа

Содержит метаданные о элементе диска мультимедиа (аудио или видео).

Он доступен в свойстве мультимедиа ресурсов [driveItem.][item-resource]


## <a name="properties"></a>Свойства

| Свойство                 | Тип                  | Описание                                                                                                   |
| :----------------------- | :-------------------- | :------------------------------------------------------------------------------------------------------------ 
| **isTranscriptionShown** | Логический               | Если файл имеет стенограмму, этот параметр управляет, если закрытые подписи /транскрипция для файла мультимедиа должны быть показаны людям во время просмотра. Read-Write.                                                    |
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
