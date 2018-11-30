---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: thumbnail
ms.openlocfilehash: 065c6ae7bbd4f6aca3172afd4399f0a1b5ff3d25
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="8943d-102">Тип ресурса thumbnail</span><span class="sxs-lookup"><span data-stu-id="8943d-102">Thumbnail resource type</span></span>

<span data-ttu-id="8943d-103">Тип ресурса **thumbnail** представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.</span><span class="sxs-lookup"><span data-stu-id="8943d-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8943d-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8943d-104">JSON representation</span></span>

<span data-ttu-id="8943d-105">Ниже представлено описание ресурса **thumbnail** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8943d-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8943d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8943d-106">Properties</span></span>

| <span data-ttu-id="8943d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8943d-107">Property</span></span>     | <span data-ttu-id="8943d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8943d-108">Type</span></span>   | <span data-ttu-id="8943d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8943d-109">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8943d-110">height</span><span class="sxs-lookup"><span data-stu-id="8943d-110">height</span></span>       | <span data-ttu-id="8943d-111">Int32</span><span class="sxs-lookup"><span data-stu-id="8943d-111">Int32</span></span>  | <span data-ttu-id="8943d-112">Высота эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="8943d-112">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="8943d-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="8943d-113">sourceItemId</span></span> | <span data-ttu-id="8943d-114">String</span><span class="sxs-lookup"><span data-stu-id="8943d-114">String</span></span> | <span data-ttu-id="8943d-p101">Уникальный идентификатор элемента, предоставившего эскиз. Доступен только при запросе эскиза папки.</span><span class="sxs-lookup"><span data-stu-id="8943d-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="8943d-117">url</span><span class="sxs-lookup"><span data-stu-id="8943d-117">url</span></span>          | <span data-ttu-id="8943d-118">String</span><span class="sxs-lookup"><span data-stu-id="8943d-118">String</span></span> | <span data-ttu-id="8943d-119">URL-адрес, используемый для получения содержимого эскиза.</span><span class="sxs-lookup"><span data-stu-id="8943d-119">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="8943d-120">width</span><span class="sxs-lookup"><span data-stu-id="8943d-120">width</span></span>        | <span data-ttu-id="8943d-121">Int32</span><span class="sxs-lookup"><span data-stu-id="8943d-121">Int32</span></span>  | <span data-ttu-id="8943d-122">Ширина эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="8943d-122">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="8943d-123">Связи</span><span class="sxs-lookup"><span data-stu-id="8943d-123">Relationships</span></span>

| <span data-ttu-id="8943d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="8943d-124">Name</span></span>    | <span data-ttu-id="8943d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="8943d-125">Type</span></span>   | <span data-ttu-id="8943d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8943d-126">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="8943d-127">content</span><span class="sxs-lookup"><span data-stu-id="8943d-127">content</span></span> | <span data-ttu-id="8943d-128">Stream</span><span class="sxs-lookup"><span data-stu-id="8943d-128">Stream</span></span> | <span data-ttu-id="8943d-129">Поток содержимого для эскиза.</span><span class="sxs-lookup"><span data-stu-id="8943d-129">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
