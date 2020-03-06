---
author: JeremyKelley
description: Тип ресурса thumbnail представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 53001d2459af4dc382501e33930bc8aca55a26b2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519766"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="28c44-103">Тип ресурса thumbnail</span><span class="sxs-lookup"><span data-stu-id="28c44-103">Thumbnail resource type</span></span>

<span data-ttu-id="28c44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28c44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28c44-105">Тип ресурса **thumbnail** представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.</span><span class="sxs-lookup"><span data-stu-id="28c44-105">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="28c44-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28c44-106">JSON representation</span></span>

<span data-ttu-id="28c44-107">Ниже представлено описание ресурса **thumbnail** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28c44-107">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="28c44-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="28c44-108">Properties</span></span>

| <span data-ttu-id="28c44-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="28c44-109">Property</span></span>     | <span data-ttu-id="28c44-110">Тип</span><span class="sxs-lookup"><span data-stu-id="28c44-110">Type</span></span>   | <span data-ttu-id="28c44-111">Описание</span><span class="sxs-lookup"><span data-stu-id="28c44-111">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="28c44-112">height</span><span class="sxs-lookup"><span data-stu-id="28c44-112">height</span></span>       | <span data-ttu-id="28c44-113">Int32</span><span class="sxs-lookup"><span data-stu-id="28c44-113">Int32</span></span>  | <span data-ttu-id="28c44-114">Высота эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="28c44-114">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="28c44-115">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="28c44-115">sourceItemId</span></span> | <span data-ttu-id="28c44-116">String</span><span class="sxs-lookup"><span data-stu-id="28c44-116">String</span></span> | <span data-ttu-id="28c44-p101">Уникальный идентификатор элемента, предоставившего эскиз. Доступен только при запросе эскиза папки.</span><span class="sxs-lookup"><span data-stu-id="28c44-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="28c44-119">url</span><span class="sxs-lookup"><span data-stu-id="28c44-119">url</span></span>          | <span data-ttu-id="28c44-120">String</span><span class="sxs-lookup"><span data-stu-id="28c44-120">String</span></span> | <span data-ttu-id="28c44-121">URL-адрес, используемый для получения содержимого эскиза.</span><span class="sxs-lookup"><span data-stu-id="28c44-121">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="28c44-122">width</span><span class="sxs-lookup"><span data-stu-id="28c44-122">width</span></span>        | <span data-ttu-id="28c44-123">Int32</span><span class="sxs-lookup"><span data-stu-id="28c44-123">Int32</span></span>  | <span data-ttu-id="28c44-124">Ширина эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="28c44-124">The width of the thumbnail, in pixels.</span></span>                                                                                      |
| <span data-ttu-id="28c44-125">содержимое</span><span class="sxs-lookup"><span data-stu-id="28c44-125">content</span></span> | <span data-ttu-id="28c44-126">Поток</span><span class="sxs-lookup"><span data-stu-id="28c44-126">Stream</span></span> | <span data-ttu-id="28c44-127">Поток содержимого для эскиза.</span><span class="sxs-lookup"><span data-stu-id="28c44-127">The content stream for the thumbnail.</span></span> |


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
