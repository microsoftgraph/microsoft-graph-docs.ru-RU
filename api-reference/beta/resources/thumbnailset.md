---
author: JeremyKelley
description: Ресурс ThumbnailSet представляет собой коллекцию ресурсов thumbnail с ключами.
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: bb8c286cd8c3827317edc9a24e4d14dbe963a05d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964349"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="6b9a3-103">Тип ресурса ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="6b9a3-103">ThumbnailSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b9a3-p101">Ресурс **ThumbnailSet** представляет собой коллекцию ресурсов [thumbnail](thumbnail.md) с ключами. Он представляет набор эскизов, связанных с ресурсом DriveItem.</span><span class="sxs-lookup"><span data-stu-id="6b9a3-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b9a3-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b9a3-106">JSON representation</span></span>

<span data-ttu-id="6b9a3-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b9a3-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a><span data-ttu-id="6b9a3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b9a3-108">Properties</span></span>

| <span data-ttu-id="6b9a3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b9a3-109">Property</span></span> | <span data-ttu-id="6b9a3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6b9a3-110">Type</span></span>                      | <span data-ttu-id="6b9a3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6b9a3-111">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="6b9a3-112">id</span><span class="sxs-lookup"><span data-stu-id="6b9a3-112">id</span></span>       | <span data-ttu-id="6b9a3-113">String</span><span class="sxs-lookup"><span data-stu-id="6b9a3-113">String</span></span>                    | <span data-ttu-id="6b9a3-p102">Идентификатор в элементе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b9a3-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="6b9a3-116">large</span><span class="sxs-lookup"><span data-stu-id="6b9a3-116">large</span></span>    | [<span data-ttu-id="6b9a3-117">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="6b9a3-117">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="6b9a3-118">Эскиз размером 1920x1920.</span><span class="sxs-lookup"><span data-stu-id="6b9a3-118">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="6b9a3-119">medium</span><span class="sxs-lookup"><span data-stu-id="6b9a3-119">medium</span></span>   | [<span data-ttu-id="6b9a3-120">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="6b9a3-120">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="6b9a3-121">Эскиз размером 176x176.</span><span class="sxs-lookup"><span data-stu-id="6b9a3-121">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="6b9a3-122">small</span><span class="sxs-lookup"><span data-stu-id="6b9a3-122">small</span></span>    | [<span data-ttu-id="6b9a3-123">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="6b9a3-123">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="6b9a3-124">Обрезанный эскиз размером 48x48.</span><span class="sxs-lookup"><span data-stu-id="6b9a3-124">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="6b9a3-125">source</span><span class="sxs-lookup"><span data-stu-id="6b9a3-125">source</span></span>   | [<span data-ttu-id="6b9a3-126">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="6b9a3-126">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="6b9a3-127">Пользовательский эскиз исходного изображения, используемого для создания других эскизов.</span><span class="sxs-lookup"><span data-stu-id="6b9a3-127">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet",
  "suppressions": []
}
-->
