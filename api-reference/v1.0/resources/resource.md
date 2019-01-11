---
title: Тип ресурса OneNoteResource
description: 'Ресурс изображения или другого файла на странице OneNote. '
localization_priority: Normal
ms.openlocfilehash: ed2fb0dd4b6e68c24da1f2441a157f734a5025f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855106"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="6c215-103">Тип ресурса OneNoteResource</span><span class="sxs-lookup"><span data-stu-id="6c215-103">OneNoteResource resource type</span></span>

<span data-ttu-id="6c215-104">Ресурс изображения или другого файла на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="6c215-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="6c215-105">Вы можете получить двоичные данные ресурса, но получение представления объекта resource или коллекции resource в формате JSON не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c215-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

<span data-ttu-id="6c215-106">Чтобы получить двоичные данные определенного ресурса, отправьте запрос GET в конечную точку `content` ресурса:</span><span class="sxs-lookup"><span data-stu-id="6c215-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="6c215-107">При получении HTML-контента страницы с использованием указанного ниже запроса возвращается URI ресурса файла.</span><span class="sxs-lookup"><span data-stu-id="6c215-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="6c215-108">На HTML-странице тег `img` включает конечные точки для исходного ресурса изображения в атрибуте `data-fullres-src` и оптимизированного изображения в атрибуте `src`:</span><span class="sxs-lookup"><span data-stu-id="6c215-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="6c215-109">Тег `object`, который представляет файлы, например PDF-, DOCX- и PNG-файлы, включает конечную точку для ресурса файла в атрибуте `data`:</span><span class="sxs-lookup"><span data-stu-id="6c215-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="6c215-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c215-110">Properties</span></span>

| <span data-ttu-id="6c215-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c215-111">Property</span></span>             | <span data-ttu-id="6c215-112">Тип</span><span class="sxs-lookup"><span data-stu-id="6c215-112">Type</span></span>            | <span data-ttu-id="6c215-113">Описание</span><span class="sxs-lookup"><span data-stu-id="6c215-113">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="6c215-114">content</span><span class="sxs-lookup"><span data-stu-id="6c215-114">content</span></span>              | <span data-ttu-id="6c215-115">Stream</span><span class="sxs-lookup"><span data-stu-id="6c215-115">Stream</span></span>          | <span data-ttu-id="6c215-116">Поток содержимого</span><span class="sxs-lookup"><span data-stu-id="6c215-116">The content stream</span></span>
| <span data-ttu-id="6c215-117">contentUrl</span><span class="sxs-lookup"><span data-stu-id="6c215-117">contentUrl</span></span>           | <span data-ttu-id="6c215-118">String (URL-адрес)</span><span class="sxs-lookup"><span data-stu-id="6c215-118">String (url)</span></span>    | <span data-ttu-id="6c215-119">URL-адрес загрузки содержимого</span><span class="sxs-lookup"><span data-stu-id="6c215-119">The URL for downloading the content</span></span>

## <a name="relationships"></a><span data-ttu-id="6c215-120">Связи</span><span class="sxs-lookup"><span data-stu-id="6c215-120">Relationships</span></span>
<span data-ttu-id="6c215-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="6c215-121">None.</span></span>


## <a name="methods"></a><span data-ttu-id="6c215-122">Методы</span><span class="sxs-lookup"><span data-stu-id="6c215-122">Methods</span></span>
| <span data-ttu-id="6c215-123">Метод</span><span class="sxs-lookup"><span data-stu-id="6c215-123">Method</span></span>           | <span data-ttu-id="6c215-124">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6c215-124">Return Type</span></span>    |<span data-ttu-id="6c215-125">Описание</span><span class="sxs-lookup"><span data-stu-id="6c215-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c215-126">Получения двоичных данных ресурса</span><span class="sxs-lookup"><span data-stu-id="6c215-126">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="6c215-127">Stream</span><span class="sxs-lookup"><span data-stu-id="6c215-127">Stream</span></span> |<span data-ttu-id="6c215-128">Получение двоичных данных ресурса файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="6c215-128">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
