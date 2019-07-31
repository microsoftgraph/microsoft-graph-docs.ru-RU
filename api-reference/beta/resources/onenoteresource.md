---
title: Тип ресурса Оненотересаурце
description: 'Изображение или другой файловый ресурс на странице OneNote. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3884be59ed0eedafa9d4a45c851570d08ea70848
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009344"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="44dea-103">Тип ресурса Оненотересаурце</span><span class="sxs-lookup"><span data-stu-id="44dea-103">onenoteResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44dea-104">Изображение или другой файловый ресурс на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="44dea-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="44dea-105">Вы можете получить двоичные данные ресурса, но получение представления объекта ресурса или коллекции ресурсов в формате JSON не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44dea-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": "String (Stream)",
  "contentUrl": "String"
}

```
<span data-ttu-id="44dea-106">Получение двоичных данных определенного ресурса путем отправки запроса GET в `content` конечную точку ресурса:</span><span class="sxs-lookup"><span data-stu-id="44dea-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="44dea-107">URI ресурса файла возвращается при получении HTML-контента страницы с помощью следующего запроса:</span><span class="sxs-lookup"><span data-stu-id="44dea-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="44dea-108">В HTML-коде страницы `img` тег включает конечные точки для исходного ресурса изображения в `data-fullres-src` атрибуте и оптимизированное изображение в `src` атрибуте:</span><span class="sxs-lookup"><span data-stu-id="44dea-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="44dea-109">`object` Тег, представляющий файлы, такие как PDF, docx и PNG, включает конечную точку для ресурса файла в `data` атрибуте:</span><span class="sxs-lookup"><span data-stu-id="44dea-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="44dea-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="44dea-110">Properties</span></span>
| <span data-ttu-id="44dea-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="44dea-111">Property</span></span>     | <span data-ttu-id="44dea-112">Тип</span><span class="sxs-lookup"><span data-stu-id="44dea-112">Type</span></span>   |<span data-ttu-id="44dea-113">Описание</span><span class="sxs-lookup"><span data-stu-id="44dea-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="44dea-114">content</span><span class="sxs-lookup"><span data-stu-id="44dea-114">content</span></span> | <span data-ttu-id="44dea-115">Модель EDM. Stream</span><span class="sxs-lookup"><span data-stu-id="44dea-115">Edm.Stream</span></span>||
| <span data-ttu-id="44dea-116">contentUrl</span><span class="sxs-lookup"><span data-stu-id="44dea-116">contentUrl</span></span> | <span data-ttu-id="44dea-117">String</span><span class="sxs-lookup"><span data-stu-id="44dea-117">String</span></span> ||

## <a name="relationships"></a><span data-ttu-id="44dea-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="44dea-118">Relationships</span></span>
<span data-ttu-id="44dea-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="44dea-119">None.</span></span>


## <a name="methods"></a><span data-ttu-id="44dea-120">Методы</span><span class="sxs-lookup"><span data-stu-id="44dea-120">Methods</span></span>
| <span data-ttu-id="44dea-121">Метод</span><span class="sxs-lookup"><span data-stu-id="44dea-121">Method</span></span>           | <span data-ttu-id="44dea-122">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="44dea-122">Return Type</span></span>    |<span data-ttu-id="44dea-123">Описание</span><span class="sxs-lookup"><span data-stu-id="44dea-123">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="44dea-124">Получение двоичных данных ресурса</span><span class="sxs-lookup"><span data-stu-id="44dea-124">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="44dea-125">Поток</span><span class="sxs-lookup"><span data-stu-id="44dea-125">Stream</span></span> |<span data-ttu-id="44dea-126">Получение двоичных данных ресурса файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="44dea-126">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
