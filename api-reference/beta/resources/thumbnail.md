---
author: JeremyKelley
description: Тип ресурса thumbnail представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 752d46f1c8a769f9f571fd13d940586fda653a58
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007664"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="381c4-103">Тип ресурса thumbnail</span><span class="sxs-lookup"><span data-stu-id="381c4-103">Thumbnail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="381c4-104">Тип ресурса **thumbnail** представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.</span><span class="sxs-lookup"><span data-stu-id="381c4-104">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="381c4-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="381c4-105">JSON representation</span></span>

<span data-ttu-id="381c4-106">Ниже представлено описание ресурса **thumbnail** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="381c4-106">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="381c4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="381c4-107">Properties</span></span>

| <span data-ttu-id="381c4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="381c4-108">Property</span></span>     | <span data-ttu-id="381c4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="381c4-109">Type</span></span>   | <span data-ttu-id="381c4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="381c4-110">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="381c4-111">height</span><span class="sxs-lookup"><span data-stu-id="381c4-111">height</span></span>       | <span data-ttu-id="381c4-112">Int32</span><span class="sxs-lookup"><span data-stu-id="381c4-112">Int32</span></span>  | <span data-ttu-id="381c4-113">Высота эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="381c4-113">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="381c4-114">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="381c4-114">sourceItemId</span></span> | <span data-ttu-id="381c4-115">String</span><span class="sxs-lookup"><span data-stu-id="381c4-115">String</span></span> | <span data-ttu-id="381c4-p101">Уникальный идентификатор элемента, предоставившего эскиз. Доступен только при запросе эскиза папки.</span><span class="sxs-lookup"><span data-stu-id="381c4-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="381c4-118">url</span><span class="sxs-lookup"><span data-stu-id="381c4-118">url</span></span>          | <span data-ttu-id="381c4-119">String</span><span class="sxs-lookup"><span data-stu-id="381c4-119">String</span></span> | <span data-ttu-id="381c4-120">URL-адрес, используемый для получения содержимого эскиза.</span><span class="sxs-lookup"><span data-stu-id="381c4-120">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="381c4-121">width</span><span class="sxs-lookup"><span data-stu-id="381c4-121">width</span></span>        | <span data-ttu-id="381c4-122">Int32</span><span class="sxs-lookup"><span data-stu-id="381c4-122">Int32</span></span>  | <span data-ttu-id="381c4-123">Ширина эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="381c4-123">The width of the thumbnail, in pixels.</span></span>                                                                                      |
| <span data-ttu-id="381c4-124">содержимое</span><span class="sxs-lookup"><span data-stu-id="381c4-124">content</span></span> | <span data-ttu-id="381c4-125">Поток</span><span class="sxs-lookup"><span data-stu-id="381c4-125">Stream</span></span> | <span data-ttu-id="381c4-126">Поток содержимого для эскиза.</span><span class="sxs-lookup"><span data-stu-id="381c4-126">The content stream for the thumbnail.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail",
  "suppressions": []
}
-->
