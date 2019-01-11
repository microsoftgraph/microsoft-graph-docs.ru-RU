---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: thumbnail
localization_priority: Normal
ms.openlocfilehash: 22602d534c3fd1f308a5e2bb67992bd76086c4fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863226"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="44db4-102">Тип ресурса thumbnail</span><span class="sxs-lookup"><span data-stu-id="44db4-102">Thumbnail resource type</span></span>

> <span data-ttu-id="44db4-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44db4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44db4-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44db4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44db4-105">Тип ресурса **thumbnail** представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.</span><span class="sxs-lookup"><span data-stu-id="44db4-105">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="44db4-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44db4-106">JSON representation</span></span>

<span data-ttu-id="44db4-107">Ниже представлено описание ресурса **thumbnail** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44db4-107">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="44db4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="44db4-108">Properties</span></span>

| <span data-ttu-id="44db4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="44db4-109">Property</span></span>     | <span data-ttu-id="44db4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="44db4-110">Type</span></span>   | <span data-ttu-id="44db4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="44db4-111">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="44db4-112">height</span><span class="sxs-lookup"><span data-stu-id="44db4-112">height</span></span>       | <span data-ttu-id="44db4-113">Int32</span><span class="sxs-lookup"><span data-stu-id="44db4-113">Int32</span></span>  | <span data-ttu-id="44db4-114">Высота эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="44db4-114">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="44db4-115">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="44db4-115">sourceItemId</span></span> | <span data-ttu-id="44db4-116">String</span><span class="sxs-lookup"><span data-stu-id="44db4-116">String</span></span> | <span data-ttu-id="44db4-p102">Уникальный идентификатор элемента, предоставившего эскиз. Доступен только при запросе эскиза папки.</span><span class="sxs-lookup"><span data-stu-id="44db4-p102">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="44db4-119">url</span><span class="sxs-lookup"><span data-stu-id="44db4-119">url</span></span>          | <span data-ttu-id="44db4-120">String</span><span class="sxs-lookup"><span data-stu-id="44db4-120">String</span></span> | <span data-ttu-id="44db4-121">URL-адрес, используемый для получения содержимого эскиза.</span><span class="sxs-lookup"><span data-stu-id="44db4-121">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="44db4-122">width</span><span class="sxs-lookup"><span data-stu-id="44db4-122">width</span></span>        | <span data-ttu-id="44db4-123">Int32</span><span class="sxs-lookup"><span data-stu-id="44db4-123">Int32</span></span>  | <span data-ttu-id="44db4-124">Ширина эскиза в пикселях.</span><span class="sxs-lookup"><span data-stu-id="44db4-124">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="44db4-125">Связи</span><span class="sxs-lookup"><span data-stu-id="44db4-125">Relationships</span></span>

| <span data-ttu-id="44db4-126">Имя</span><span class="sxs-lookup"><span data-stu-id="44db4-126">Name</span></span>    | <span data-ttu-id="44db4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="44db4-127">Type</span></span>   | <span data-ttu-id="44db4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="44db4-128">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="44db4-129">content</span><span class="sxs-lookup"><span data-stu-id="44db4-129">content</span></span> | <span data-ttu-id="44db4-130">Stream</span><span class="sxs-lookup"><span data-stu-id="44db4-130">Stream</span></span> | <span data-ttu-id="44db4-131">Поток содержимого для эскиза.</span><span class="sxs-lookup"><span data-stu-id="44db4-131">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
