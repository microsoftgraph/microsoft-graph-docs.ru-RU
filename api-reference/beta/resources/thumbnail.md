---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
ms.openlocfilehash: db8c8c37313402d694d9e0badfd244b739c0459a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342004"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="4c66d-102">Тип ресурса thumbnail</span><span class="sxs-lookup"><span data-stu-id="4c66d-102">Thumbnail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c66d-103">Тип ресурса **thumbnail** представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.</span><span class="sxs-lookup"><span data-stu-id="4c66d-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c66d-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c66d-104">JSON representation</span></span>

<span data-ttu-id="4c66d-105">Ниже представлено описание ресурса **thumbnail** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c66d-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4c66d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c66d-106">Properties</span></span>

| <span data-ttu-id="4c66d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c66d-107">Property</span></span>     | <span data-ttu-id="4c66d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4c66d-108">Type</span></span>   | <span data-ttu-id="4c66d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4c66d-109">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="4c66d-110">height</span><span class="sxs-lookup"><span data-stu-id="4c66d-110">height</span></span>       | <span data-ttu-id="4c66d-111">Int32</span><span class="sxs-lookup"><span data-stu-id="4c66d-111">Int32</span></span>  | <span data-ttu-id="4c66d-112">Высота эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="4c66d-112">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="4c66d-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="4c66d-113">sourceItemId</span></span> | <span data-ttu-id="4c66d-114">String</span><span class="sxs-lookup"><span data-stu-id="4c66d-114">String</span></span> | <span data-ttu-id="4c66d-p101">Уникальный идентификатор элемента, предоставившего эскиз. Доступен только при запросе эскиза папки.</span><span class="sxs-lookup"><span data-stu-id="4c66d-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="4c66d-117">url</span><span class="sxs-lookup"><span data-stu-id="4c66d-117">url</span></span>          | <span data-ttu-id="4c66d-118">String</span><span class="sxs-lookup"><span data-stu-id="4c66d-118">String</span></span> | <span data-ttu-id="4c66d-119">URL-адрес, используемый для получения содержимого эскиза.</span><span class="sxs-lookup"><span data-stu-id="4c66d-119">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="4c66d-120">width</span><span class="sxs-lookup"><span data-stu-id="4c66d-120">width</span></span>        | <span data-ttu-id="4c66d-121">Int32</span><span class="sxs-lookup"><span data-stu-id="4c66d-121">Int32</span></span>  | <span data-ttu-id="4c66d-122">Ширина эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="4c66d-122">The width of the thumbnail, in pixels.</span></span>                                                                                      |
| <span data-ttu-id="4c66d-123">содержимое</span><span class="sxs-lookup"><span data-stu-id="4c66d-123">content</span></span> | <span data-ttu-id="4c66d-124">Поток</span><span class="sxs-lookup"><span data-stu-id="4c66d-124">Stream</span></span> | <span data-ttu-id="4c66d-125">Поток содержимого для эскиза.</span><span class="sxs-lookup"><span data-stu-id="4c66d-125">The content stream for the thumbnail.</span></span> |


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
