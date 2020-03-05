---
author: JeremyKelley
description: Ресурс ThumbnailSet представляет собой коллекцию ресурсов thumbnail с ключами.
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: bd6e3326eaa0ea0bea407429e89d361575f20916
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519759"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="d3cc7-103">Тип ресурса ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="d3cc7-103">ThumbnailSet resource type</span></span>

<span data-ttu-id="d3cc7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d3cc7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3cc7-p101">Ресурс **ThumbnailSet** представляет собой коллекцию ресурсов [thumbnail](thumbnail.md) с ключами. Он представляет набор эскизов, связанных с ресурсом DriveItem.</span><span class="sxs-lookup"><span data-stu-id="d3cc7-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3cc7-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3cc7-107">JSON representation</span></span>

<span data-ttu-id="d3cc7-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3cc7-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d3cc7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3cc7-109">Properties</span></span>

| <span data-ttu-id="d3cc7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3cc7-110">Property</span></span> | <span data-ttu-id="d3cc7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d3cc7-111">Type</span></span>                      | <span data-ttu-id="d3cc7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d3cc7-112">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="d3cc7-113">id</span><span class="sxs-lookup"><span data-stu-id="d3cc7-113">id</span></span>       | <span data-ttu-id="d3cc7-114">String</span><span class="sxs-lookup"><span data-stu-id="d3cc7-114">String</span></span>                    | <span data-ttu-id="d3cc7-p102">Идентификатор в элементе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d3cc7-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="d3cc7-117">large</span><span class="sxs-lookup"><span data-stu-id="d3cc7-117">large</span></span>    | [<span data-ttu-id="d3cc7-118">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="d3cc7-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d3cc7-119">Эскиз размером 1920x1920.</span><span class="sxs-lookup"><span data-stu-id="d3cc7-119">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="d3cc7-120">medium</span><span class="sxs-lookup"><span data-stu-id="d3cc7-120">medium</span></span>   | [<span data-ttu-id="d3cc7-121">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="d3cc7-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d3cc7-122">Эскиз размером 176x176.</span><span class="sxs-lookup"><span data-stu-id="d3cc7-122">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="d3cc7-123">small</span><span class="sxs-lookup"><span data-stu-id="d3cc7-123">small</span></span>    | [<span data-ttu-id="d3cc7-124">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="d3cc7-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d3cc7-125">Обрезанный эскиз размером 48x48.</span><span class="sxs-lookup"><span data-stu-id="d3cc7-125">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="d3cc7-126">source</span><span class="sxs-lookup"><span data-stu-id="d3cc7-126">source</span></span>   | [<span data-ttu-id="d3cc7-127">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="d3cc7-127">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d3cc7-128">Пользовательский эскиз исходного изображения, используемого для создания других эскизов.</span><span class="sxs-lookup"><span data-stu-id="d3cc7-128">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

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
