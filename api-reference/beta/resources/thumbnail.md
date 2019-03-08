---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
ms.openlocfilehash: 485714109005415d4a2c98fbbf2befb50ca991d0
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481757"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="1a61b-102">Тип ресурса thumbnail</span><span class="sxs-lookup"><span data-stu-id="1a61b-102">Thumbnail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a61b-103">Тип ресурса **thumbnail** представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.</span><span class="sxs-lookup"><span data-stu-id="1a61b-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a61b-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a61b-104">JSON representation</span></span>

<span data-ttu-id="1a61b-105">Ниже представлено описание ресурса **thumbnail** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a61b-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="1a61b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a61b-106">Properties</span></span>

| <span data-ttu-id="1a61b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a61b-107">Property</span></span>     | <span data-ttu-id="1a61b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1a61b-108">Type</span></span>   | <span data-ttu-id="1a61b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1a61b-109">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1a61b-110">height</span><span class="sxs-lookup"><span data-stu-id="1a61b-110">height</span></span>       | <span data-ttu-id="1a61b-111">Int32</span><span class="sxs-lookup"><span data-stu-id="1a61b-111">Int32</span></span>  | <span data-ttu-id="1a61b-112">Высота эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="1a61b-112">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="1a61b-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="1a61b-113">sourceItemId</span></span> | <span data-ttu-id="1a61b-114">String</span><span class="sxs-lookup"><span data-stu-id="1a61b-114">String</span></span> | <span data-ttu-id="1a61b-p101">Уникальный идентификатор элемента, предоставившего эскиз. Доступен только при запросе эскиза папки.</span><span class="sxs-lookup"><span data-stu-id="1a61b-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="1a61b-117">url</span><span class="sxs-lookup"><span data-stu-id="1a61b-117">url</span></span>          | <span data-ttu-id="1a61b-118">String</span><span class="sxs-lookup"><span data-stu-id="1a61b-118">String</span></span> | <span data-ttu-id="1a61b-119">URL-адрес, используемый для получения содержимого эскиза.</span><span class="sxs-lookup"><span data-stu-id="1a61b-119">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="1a61b-120">width</span><span class="sxs-lookup"><span data-stu-id="1a61b-120">width</span></span>        | <span data-ttu-id="1a61b-121">Int32</span><span class="sxs-lookup"><span data-stu-id="1a61b-121">Int32</span></span>  | <span data-ttu-id="1a61b-122">Ширина эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="1a61b-122">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="1a61b-123">Связи</span><span class="sxs-lookup"><span data-stu-id="1a61b-123">Relationships</span></span>

| <span data-ttu-id="1a61b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="1a61b-124">Name</span></span>    | <span data-ttu-id="1a61b-125">Тип</span><span class="sxs-lookup"><span data-stu-id="1a61b-125">Type</span></span>   | <span data-ttu-id="1a61b-126">Описание</span><span class="sxs-lookup"><span data-stu-id="1a61b-126">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="1a61b-127">content</span><span class="sxs-lookup"><span data-stu-id="1a61b-127">content</span></span> | <span data-ttu-id="1a61b-128">Stream</span><span class="sxs-lookup"><span data-stu-id="1a61b-128">Stream</span></span> | <span data-ttu-id="1a61b-129">Поток содержимого для эскиза.</span><span class="sxs-lookup"><span data-stu-id="1a61b-129">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail",
  "suppressions": [
    "Error: /api-reference/beta/resources/thumbnail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
