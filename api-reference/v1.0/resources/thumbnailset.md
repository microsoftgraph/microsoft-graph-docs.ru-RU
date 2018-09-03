---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
ms.openlocfilehash: 2ba45363b684142b91aac62d4b2a5b0d371d6b3d
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23270813"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="5a22c-102">Тип ресурса ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="5a22c-102">ThumbnailSet resource type</span></span>

<span data-ttu-id="5a22c-p101">Ресурс **ThumbnailSet** представляет собой коллекцию ресурсов [thumbnail](thumbnail.md) с ключами. Он представляет набор эскизов, связанных с ресурсом DriveItem.</span><span class="sxs-lookup"><span data-stu-id="5a22c-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a22c-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a22c-105">JSON representation</span></span>

<span data-ttu-id="5a22c-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a22c-106">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "source",
    "small",
    "medium",
    "large"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.thumbnailSet",
  "openType": true
}-->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a><span data-ttu-id="5a22c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a22c-107">Properties</span></span>

| <span data-ttu-id="5a22c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a22c-108">Property</span></span> | <span data-ttu-id="5a22c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5a22c-109">Type</span></span>                      | <span data-ttu-id="5a22c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5a22c-110">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="5a22c-111">id</span><span class="sxs-lookup"><span data-stu-id="5a22c-111">id</span></span>       | <span data-ttu-id="5a22c-112">Строка</span><span class="sxs-lookup"><span data-stu-id="5a22c-112">String</span></span>                    | <span data-ttu-id="5a22c-p102">Идентификатор в элементе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a22c-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="5a22c-115">large</span><span class="sxs-lookup"><span data-stu-id="5a22c-115">large</span></span>    | [<span data-ttu-id="5a22c-116">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="5a22c-116">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="5a22c-117">Эскиз размером 1920x1920.</span><span class="sxs-lookup"><span data-stu-id="5a22c-117">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="5a22c-118">medium</span><span class="sxs-lookup"><span data-stu-id="5a22c-118">medium</span></span>   | [<span data-ttu-id="5a22c-119">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="5a22c-119">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="5a22c-120">Эскиз размером 176x176.</span><span class="sxs-lookup"><span data-stu-id="5a22c-120">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="5a22c-121">small</span><span class="sxs-lookup"><span data-stu-id="5a22c-121">small</span></span>    | [<span data-ttu-id="5a22c-122">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="5a22c-122">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="5a22c-123">Обрезанный эскиз размером 48x48.</span><span class="sxs-lookup"><span data-stu-id="5a22c-123">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="5a22c-124">source</span><span class="sxs-lookup"><span data-stu-id="5a22c-124">source</span></span>   | [<span data-ttu-id="5a22c-125">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="5a22c-125">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="5a22c-126">Пользовательский эскиз исходного изображения, используемого для создания других эскизов.</span><span class="sxs-lookup"><span data-stu-id="5a22c-126">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
