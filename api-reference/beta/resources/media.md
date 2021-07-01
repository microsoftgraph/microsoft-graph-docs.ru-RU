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
# <a name="media-resouce-type"></a><span data-ttu-id="3d427-103">тип повторного окантовки мультимедиа</span><span class="sxs-lookup"><span data-stu-id="3d427-103">media resouce type</span></span>

<span data-ttu-id="3d427-104">Содержит метаданные о элементе диска мультимедиа (аудио или видео).</span><span class="sxs-lookup"><span data-stu-id="3d427-104">Contains metadata about the media (audio or video) drive item.</span></span>

<span data-ttu-id="3d427-105">Он доступен в свойстве мультимедиа ресурсов [driveItem.][item-resource]</span><span class="sxs-lookup"><span data-stu-id="3d427-105">It is available on the media property of [driveItem][item-resource] resources.</span></span>


## <a name="properties"></a><span data-ttu-id="3d427-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d427-106">Properties</span></span>

| <span data-ttu-id="3d427-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d427-107">Property</span></span>                 | <span data-ttu-id="3d427-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3d427-108">Type</span></span>                  | <span data-ttu-id="3d427-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3d427-109">Description</span></span>                                                                                                   |
| :----------------------- | :-------------------- | :------------------------------------------------------------------------------------------------------------ 
| <span data-ttu-id="3d427-110">**isTranscriptionShown**</span><span class="sxs-lookup"><span data-stu-id="3d427-110">**isTranscriptionShown**</span></span> | <span data-ttu-id="3d427-111">Логический</span><span class="sxs-lookup"><span data-stu-id="3d427-111">Boolean</span></span>               | <span data-ttu-id="3d427-112">Если файл имеет стенограмму, этот параметр управляет, если закрытые подписи /транскрипция для файла мультимедиа должны быть показаны людям во время просмотра.</span><span class="sxs-lookup"><span data-stu-id="3d427-112">If a file has a transcript, this setting controls if the closed captions / transcription for the media file should be shown to people during viewing.</span></span> <span data-ttu-id="3d427-113">Read-Write.</span><span class="sxs-lookup"><span data-stu-id="3d427-113">Read-Write.</span></span>                                                    |
| <span data-ttu-id="3d427-114">**mediaSource**</span><span class="sxs-lookup"><span data-stu-id="3d427-114">**mediaSource**</span></span>          | [<span data-ttu-id="3d427-115">mediaSource</span><span class="sxs-lookup"><span data-stu-id="3d427-115">mediaSource</span></span>](mediaSource.md)         | <span data-ttu-id="3d427-116">Сведения об источнике мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="3d427-116">Information about the source of media.</span></span> <span data-ttu-id="3d427-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d427-117">Read-only.</span></span>                                                             | 


## <a name="json-representation"></a><span data-ttu-id="3d427-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d427-118">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="3d427-119">См. также</span><span class="sxs-lookup"><span data-stu-id="3d427-119">See also</span></span> 

<span data-ttu-id="3d427-120">Дополнительные сведения о гранях на driveItem см. [в сайте driveItem.](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="3d427-120">For more information about the facets on a driveItem, see [driveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md
[mediaSource]: mediaSource.md

<!-- {
  "type": "#page.annotation",
  "description": "The media resource type provides information about the media item.",
  "keywords": "mediaItem,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/Media"
} -->
