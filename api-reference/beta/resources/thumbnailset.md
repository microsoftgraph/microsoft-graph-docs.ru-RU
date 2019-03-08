---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: a21c6d8fb8808f41d6b343f4bdfb2d63c0531a9e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482212"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="08de7-102">Тип ресурса ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="08de7-102">ThumbnailSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08de7-p101">Ресурс **ThumbnailSet** представляет собой коллекцию ресурсов [thumbnail](thumbnail.md) с ключами. Он представляет набор эскизов, связанных с ресурсом DriveItem.</span><span class="sxs-lookup"><span data-stu-id="08de7-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="08de7-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08de7-105">JSON representation</span></span>

<span data-ttu-id="08de7-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08de7-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="08de7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="08de7-107">Properties</span></span>

| <span data-ttu-id="08de7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="08de7-108">Property</span></span> | <span data-ttu-id="08de7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="08de7-109">Type</span></span>                      | <span data-ttu-id="08de7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="08de7-110">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="08de7-111">id</span><span class="sxs-lookup"><span data-stu-id="08de7-111">id</span></span>       | <span data-ttu-id="08de7-112">String</span><span class="sxs-lookup"><span data-stu-id="08de7-112">String</span></span>                    | <span data-ttu-id="08de7-p102">Идентификатор в элементе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08de7-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="08de7-115">large</span><span class="sxs-lookup"><span data-stu-id="08de7-115">large</span></span>    | [<span data-ttu-id="08de7-116">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="08de7-116">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="08de7-117">Эскиз размером 1920x1920.</span><span class="sxs-lookup"><span data-stu-id="08de7-117">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="08de7-118">medium</span><span class="sxs-lookup"><span data-stu-id="08de7-118">medium</span></span>   | [<span data-ttu-id="08de7-119">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="08de7-119">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="08de7-120">Эскиз размером 176x176.</span><span class="sxs-lookup"><span data-stu-id="08de7-120">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="08de7-121">small</span><span class="sxs-lookup"><span data-stu-id="08de7-121">small</span></span>    | [<span data-ttu-id="08de7-122">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="08de7-122">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="08de7-123">Обрезанный эскиз размером 48x48.</span><span class="sxs-lookup"><span data-stu-id="08de7-123">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="08de7-124">source</span><span class="sxs-lookup"><span data-stu-id="08de7-124">source</span></span>   | [<span data-ttu-id="08de7-125">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="08de7-125">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="08de7-126">Пользовательский эскиз исходного изображения, используемого для создания других эскизов.</span><span class="sxs-lookup"><span data-stu-id="08de7-126">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/thumbnailset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
