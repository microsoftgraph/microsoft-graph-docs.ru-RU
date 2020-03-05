---
title: Тип ресурса Оненотересаурце
description: 'Изображение или другой файловый ресурс на странице OneNote. '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 03dde18905892538e4f883f2e90b6b0c36fda460
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446977"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="4d4f5-103">Тип ресурса Оненотересаурце</span><span class="sxs-lookup"><span data-stu-id="4d4f5-103">OneNoteResource resource type</span></span>

<span data-ttu-id="4d4f5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4d4f5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4d4f5-105">Изображение или другой файловый ресурс на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="4d4f5-105">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="4d4f5-106">Вы можете получить двоичные данные ресурса, но получение представления объекта ресурса или коллекции ресурсов в формате JSON не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d4f5-106">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

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

<span data-ttu-id="4d4f5-107">Получение двоичных данных определенного ресурса путем отправки запроса GET в `content` конечную точку ресурса:</span><span class="sxs-lookup"><span data-stu-id="4d4f5-107">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="4d4f5-108">URI ресурса файла возвращается при получении HTML-контента страницы с помощью следующего запроса:</span><span class="sxs-lookup"><span data-stu-id="4d4f5-108">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="4d4f5-109">В HTML-коде страницы `img` тег включает конечные точки для исходного ресурса изображения в `data-fullres-src` атрибуте и оптимизированное изображение в `src` атрибуте:</span><span class="sxs-lookup"><span data-stu-id="4d4f5-109">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="4d4f5-110">`object` Тег, представляющий файлы, такие как PDF, docx и PNG, включает конечную точку для ресурса файла в `data` атрибуте:</span><span class="sxs-lookup"><span data-stu-id="4d4f5-110">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="4d4f5-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d4f5-111">Properties</span></span>

| <span data-ttu-id="4d4f5-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d4f5-112">Property</span></span>             | <span data-ttu-id="4d4f5-113">Тип</span><span class="sxs-lookup"><span data-stu-id="4d4f5-113">Type</span></span>            | <span data-ttu-id="4d4f5-114">Описание</span><span class="sxs-lookup"><span data-stu-id="4d4f5-114">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="4d4f5-115">содержимое</span><span class="sxs-lookup"><span data-stu-id="4d4f5-115">content</span></span>              | <span data-ttu-id="4d4f5-116">Поток</span><span class="sxs-lookup"><span data-stu-id="4d4f5-116">Stream</span></span>          | <span data-ttu-id="4d4f5-117">Поток содержимого</span><span class="sxs-lookup"><span data-stu-id="4d4f5-117">The content stream</span></span>
| <span data-ttu-id="4d4f5-118">contentUrl</span><span class="sxs-lookup"><span data-stu-id="4d4f5-118">contentUrl</span></span>           | <span data-ttu-id="4d4f5-119">Строка (URL-адрес)</span><span class="sxs-lookup"><span data-stu-id="4d4f5-119">String (url)</span></span>    | <span data-ttu-id="4d4f5-120">URL-адрес для скачивания контента</span><span class="sxs-lookup"><span data-stu-id="4d4f5-120">The URL for downloading the content</span></span>

## <a name="relationships"></a><span data-ttu-id="4d4f5-121">Связи</span><span class="sxs-lookup"><span data-stu-id="4d4f5-121">Relationships</span></span>
<span data-ttu-id="4d4f5-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4d4f5-122">None.</span></span>


## <a name="methods"></a><span data-ttu-id="4d4f5-123">Методы</span><span class="sxs-lookup"><span data-stu-id="4d4f5-123">Methods</span></span>
| <span data-ttu-id="4d4f5-124">Метод</span><span class="sxs-lookup"><span data-stu-id="4d4f5-124">Method</span></span>           | <span data-ttu-id="4d4f5-125">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4d4f5-125">Return Type</span></span>    |<span data-ttu-id="4d4f5-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4d4f5-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4d4f5-127">Получение двоичных данных ресурса</span><span class="sxs-lookup"><span data-stu-id="4d4f5-127">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="4d4f5-128">Stream</span><span class="sxs-lookup"><span data-stu-id="4d4f5-128">Stream</span></span> |<span data-ttu-id="4d4f5-129">Получение двоичных данных ресурса файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="4d4f5-129">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
