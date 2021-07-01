---
author: MarcMroz
description: Ресурс mediaSource содержит метаданные об источнике элемента диска мультимедиа (аудио или видео).
title: Тип ресурса mediaSource
localization_priority: Normal
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: c0b2f93095d7e7a4b9176073cc8688b5eb473cd3
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236338"
---
# <a name="mediasource-resouce-type"></a><span data-ttu-id="56332-103">тип resouce mediaSource</span><span class="sxs-lookup"><span data-stu-id="56332-103">mediaSource resouce type</span></span>

<span data-ttu-id="56332-104">Ресурс **mediaSource содержит** метаданные об источнике диска мультимедиа (аудио или видео).</span><span class="sxs-lookup"><span data-stu-id="56332-104">The **mediaSource** resource contains metadata about the source of media (audio or video) drive item.</span></span>

<span data-ttu-id="56332-105">Он доступен в свойстве мультимедиа ресурсов [driveItem.][item-resource]</span><span class="sxs-lookup"><span data-stu-id="56332-105">It is available on the media property of [driveItem][item-resource] resources.</span></span>

## <a name="properties"></a><span data-ttu-id="56332-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="56332-106">Properties</span></span>

| <span data-ttu-id="56332-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="56332-107">Property</span></span>                 | <span data-ttu-id="56332-108">Тип</span><span class="sxs-lookup"><span data-stu-id="56332-108">Type</span></span>                       | <span data-ttu-id="56332-109">Описание</span><span class="sxs-lookup"><span data-stu-id="56332-109">Description</span></span>                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| <span data-ttu-id="56332-110">**contentCategory**</span><span class="sxs-lookup"><span data-stu-id="56332-110">**contentCategory**</span></span>      | <span data-ttu-id="56332-111">mediaSourceContentCategory</span><span class="sxs-lookup"><span data-stu-id="56332-111">mediaSourceContentCategory</span></span> | <span data-ttu-id="56332-112">Значение переумерия, которое указывает на категорию контента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="56332-112">Enumeration value that indicates the media content category.</span></span>                                     |

### <a name="mediasourcecontentcategory-values"></a><span data-ttu-id="56332-113">значения mediaSourceContentCategory</span><span class="sxs-lookup"><span data-stu-id="56332-113">mediaSourceContentCategory values</span></span>

| <span data-ttu-id="56332-114">Значение</span><span class="sxs-lookup"><span data-stu-id="56332-114">Value</span></span>               | <span data-ttu-id="56332-115">Описание</span><span class="sxs-lookup"><span data-stu-id="56332-115">Description</span></span>                                         |
|:------------------- |:----------------------------------------------------|
| <span data-ttu-id="56332-116">собрание</span><span class="sxs-lookup"><span data-stu-id="56332-116">meeting</span></span>             | <span data-ttu-id="56332-117">Носители — это собрание.</span><span class="sxs-lookup"><span data-stu-id="56332-117">The media is a meeting.</span></span>                             |
| <span data-ttu-id="56332-118">liveStream</span><span class="sxs-lookup"><span data-stu-id="56332-118">liveStream</span></span>          | <span data-ttu-id="56332-119">Носители — это прямая трансляция.</span><span class="sxs-lookup"><span data-stu-id="56332-119">The media is a live stream.</span></span>                         |
| <span data-ttu-id="56332-120">презентация</span><span class="sxs-lookup"><span data-stu-id="56332-120">presentation</span></span>        | <span data-ttu-id="56332-121">Носители — это презентация.</span><span class="sxs-lookup"><span data-stu-id="56332-121">The media is a presentation.</span></span>                        |
| <span data-ttu-id="56332-122">screenRecording</span><span class="sxs-lookup"><span data-stu-id="56332-122">screenRecording</span></span>     | <span data-ttu-id="56332-123">Носители — это запись экрана.</span><span class="sxs-lookup"><span data-stu-id="56332-123">The media is a screen recording.</span></span>                    |
| <span data-ttu-id="56332-124">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="56332-124">unknownFutureValue</span></span>  | <span data-ttu-id="56332-125">Значение маркера для будущей совместимости.</span><span class="sxs-lookup"><span data-stu-id="56332-125">Marker value for future compatibility.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="56332-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="56332-126">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="56332-127">См. также</span><span class="sxs-lookup"><span data-stu-id="56332-127">See also</span></span>

<span data-ttu-id="56332-128">Дополнительные сведения о гранях на driveItem см. [в сайте driveItem.](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="56332-128">For more information about the facets on a driveItem, see [driveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The mediaSource facet provides information about drive item source.",
  "keywords": "mediaSource,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/MediaSource"
} -->
