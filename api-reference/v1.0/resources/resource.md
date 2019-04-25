---
title: Тип ресурса Оненотересаурце
description: 'Изображение или другой файловый ресурс на странице OneNote. '
localization_priority: Normal
ms.openlocfilehash: ed2fb0dd4b6e68c24da1f2441a157f734a5025f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579326"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="bd1ea-103">Тип ресурса Оненотересаурце</span><span class="sxs-lookup"><span data-stu-id="bd1ea-103">OneNoteResource resource type</span></span>

<span data-ttu-id="bd1ea-104">Изображение или другой файловый ресурс на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="bd1ea-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="bd1ea-105">Вы можете получить двоичные данные ресурса, но получение представления объекта ресурса или коллекции ресурсов в формате JSON не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd1ea-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

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

<span data-ttu-id="bd1ea-106">Получение двоичных данных определенного ресурса путем отправки запроса GET в `content` конечную точку ресурса:</span><span class="sxs-lookup"><span data-stu-id="bd1ea-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="bd1ea-107">URI ресурса файла возвращается при получении HTML-контента страницы с помощью следующего запроса:</span><span class="sxs-lookup"><span data-stu-id="bd1ea-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="bd1ea-108">В HTML-коде страницы `img` тег включает конечные точки для исходного ресурса изображения в `data-fullres-src` атрибуте и оптимизированное изображение в `src` атрибуте:</span><span class="sxs-lookup"><span data-stu-id="bd1ea-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="bd1ea-109">`object` Тег, представляющий файлы, такие как PDF, docx и PNG, включает конечную точку для ресурса файла в `data` атрибуте:</span><span class="sxs-lookup"><span data-stu-id="bd1ea-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="bd1ea-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd1ea-110">Properties</span></span>

| <span data-ttu-id="bd1ea-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd1ea-111">Property</span></span>             | <span data-ttu-id="bd1ea-112">Тип</span><span class="sxs-lookup"><span data-stu-id="bd1ea-112">Type</span></span>            | <span data-ttu-id="bd1ea-113">Описание</span><span class="sxs-lookup"><span data-stu-id="bd1ea-113">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="bd1ea-114">содержимое</span><span class="sxs-lookup"><span data-stu-id="bd1ea-114">content</span></span>              | <span data-ttu-id="bd1ea-115">Поток</span><span class="sxs-lookup"><span data-stu-id="bd1ea-115">Stream</span></span>          | <span data-ttu-id="bd1ea-116">Поток содержимого</span><span class="sxs-lookup"><span data-stu-id="bd1ea-116">The content stream</span></span>
| <span data-ttu-id="bd1ea-117">contentUrl</span><span class="sxs-lookup"><span data-stu-id="bd1ea-117">contentUrl</span></span>           | <span data-ttu-id="bd1ea-118">Строка (URL-адрес)</span><span class="sxs-lookup"><span data-stu-id="bd1ea-118">String (url)</span></span>    | <span data-ttu-id="bd1ea-119">URL-адрес для скачивания контента</span><span class="sxs-lookup"><span data-stu-id="bd1ea-119">The URL for downloading the content</span></span>

## <a name="relationships"></a><span data-ttu-id="bd1ea-120">Связи</span><span class="sxs-lookup"><span data-stu-id="bd1ea-120">Relationships</span></span>
<span data-ttu-id="bd1ea-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="bd1ea-121">None.</span></span>


## <a name="methods"></a><span data-ttu-id="bd1ea-122">Методы</span><span class="sxs-lookup"><span data-stu-id="bd1ea-122">Methods</span></span>
| <span data-ttu-id="bd1ea-123">Метод</span><span class="sxs-lookup"><span data-stu-id="bd1ea-123">Method</span></span>           | <span data-ttu-id="bd1ea-124">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bd1ea-124">Return Type</span></span>    |<span data-ttu-id="bd1ea-125">Описание</span><span class="sxs-lookup"><span data-stu-id="bd1ea-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd1ea-126">Получение двоичных данных ресурса</span><span class="sxs-lookup"><span data-stu-id="bd1ea-126">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="bd1ea-127">Поток</span><span class="sxs-lookup"><span data-stu-id="bd1ea-127">Stream</span></span> |<span data-ttu-id="bd1ea-128">Получение двоичных данных ресурса файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="bd1ea-128">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
