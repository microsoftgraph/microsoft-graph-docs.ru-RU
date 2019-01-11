---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: 145134d6a3ad85134ea2d6c4d72e050bc17b31d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830193"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="5f05a-102">Тип ресурса ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="5f05a-102">ThumbnailSet resource type</span></span>

> <span data-ttu-id="5f05a-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5f05a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f05a-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f05a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f05a-p102">Ресурс **ThumbnailSet** представляет собой коллекцию ресурсов [thumbnail](thumbnail.md) с ключами. Он представляет набор эскизов, связанных с ресурсом DriveItem.</span><span class="sxs-lookup"><span data-stu-id="5f05a-p102">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f05a-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f05a-107">JSON representation</span></span>

<span data-ttu-id="5f05a-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f05a-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5f05a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f05a-109">Properties</span></span>

| <span data-ttu-id="5f05a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f05a-110">Property</span></span> | <span data-ttu-id="5f05a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5f05a-111">Type</span></span>                      | <span data-ttu-id="5f05a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5f05a-112">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="5f05a-113">id</span><span class="sxs-lookup"><span data-stu-id="5f05a-113">id</span></span>       | <span data-ttu-id="5f05a-114">String</span><span class="sxs-lookup"><span data-stu-id="5f05a-114">String</span></span>                    | <span data-ttu-id="5f05a-p103">Идентификатор в элементе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f05a-p103">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="5f05a-117">large</span><span class="sxs-lookup"><span data-stu-id="5f05a-117">large</span></span>    | [<span data-ttu-id="5f05a-118">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="5f05a-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="5f05a-119">Эскиз размером 1920x1920.</span><span class="sxs-lookup"><span data-stu-id="5f05a-119">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="5f05a-120">medium</span><span class="sxs-lookup"><span data-stu-id="5f05a-120">medium</span></span>   | [<span data-ttu-id="5f05a-121">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="5f05a-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="5f05a-122">Эскиз размером 176x176.</span><span class="sxs-lookup"><span data-stu-id="5f05a-122">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="5f05a-123">small</span><span class="sxs-lookup"><span data-stu-id="5f05a-123">small</span></span>    | [<span data-ttu-id="5f05a-124">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="5f05a-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="5f05a-125">Обрезанный эскиз размером 48x48.</span><span class="sxs-lookup"><span data-stu-id="5f05a-125">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="5f05a-126">source</span><span class="sxs-lookup"><span data-stu-id="5f05a-126">source</span></span>   | [<span data-ttu-id="5f05a-127">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="5f05a-127">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="5f05a-128">Пользовательский эскиз исходного изображения, используемого для создания других эскизов.</span><span class="sxs-lookup"><span data-stu-id="5f05a-128">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
