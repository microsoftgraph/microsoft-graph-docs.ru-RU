---
title: Тип ресурса Оненотересаурце
description: 'Изображение или другой файловый ресурс на странице OneNote. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: fc4f3962e5be1eeb69598548067b61aa86c9c246
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806299"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="0f89f-103">Тип ресурса Оненотересаурце</span><span class="sxs-lookup"><span data-stu-id="0f89f-103">onenoteResource resource type</span></span>

<span data-ttu-id="0f89f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f89f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f89f-105">Изображение или другой файловый ресурс на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="0f89f-105">An image or other file resource on a OneNote page.</span></span>

<span data-ttu-id="0f89f-106">Вы можете получить двоичные данные ресурса, но получение представления объекта ресурса или коллекции ресурсов в формате JSON не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f89f-106">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

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
<span data-ttu-id="0f89f-107">Получение двоичных данных определенного ресурса путем отправки запроса GET в `content` конечную точку ресурса:</span><span class="sxs-lookup"><span data-stu-id="0f89f-107">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="0f89f-108">URI ресурса файла возвращается при получении HTML-контента страницы с помощью следующего запроса:</span><span class="sxs-lookup"><span data-stu-id="0f89f-108">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="0f89f-109">В HTML-коде страницы `img` тег включает конечные точки для исходного ресурса изображения в `data-fullres-src` атрибуте и оптимизированное изображение в `src` атрибуте:</span><span class="sxs-lookup"><span data-stu-id="0f89f-109">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="0f89f-110">`object`Тег, представляющий файлы, такие как PDF, docx и PNG, включает конечную точку для ресурса файла в `data` атрибуте:</span><span class="sxs-lookup"><span data-stu-id="0f89f-110">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="0f89f-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f89f-111">Properties</span></span>
| <span data-ttu-id="0f89f-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f89f-112">Property</span></span>     | <span data-ttu-id="0f89f-113">Тип</span><span class="sxs-lookup"><span data-stu-id="0f89f-113">Type</span></span>   |<span data-ttu-id="0f89f-114">Описание</span><span class="sxs-lookup"><span data-stu-id="0f89f-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0f89f-115">content</span><span class="sxs-lookup"><span data-stu-id="0f89f-115">content</span></span> | <span data-ttu-id="0f89f-116">Модель EDM. Stream</span><span class="sxs-lookup"><span data-stu-id="0f89f-116">Edm.Stream</span></span>||
| <span data-ttu-id="0f89f-117">contentUrl</span><span class="sxs-lookup"><span data-stu-id="0f89f-117">contentUrl</span></span> | <span data-ttu-id="0f89f-118">String</span><span class="sxs-lookup"><span data-stu-id="0f89f-118">String</span></span> ||

## <a name="relationships"></a><span data-ttu-id="0f89f-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="0f89f-119">Relationships</span></span>
<span data-ttu-id="0f89f-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0f89f-120">None.</span></span>


## <a name="methods"></a><span data-ttu-id="0f89f-121">Методы</span><span class="sxs-lookup"><span data-stu-id="0f89f-121">Methods</span></span>
| <span data-ttu-id="0f89f-122">Метод</span><span class="sxs-lookup"><span data-stu-id="0f89f-122">Method</span></span>           | <span data-ttu-id="0f89f-123">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0f89f-123">Return Type</span></span>    |<span data-ttu-id="0f89f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0f89f-124">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f89f-125">Получение двоичных данных ресурса</span><span class="sxs-lookup"><span data-stu-id="0f89f-125">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="0f89f-126">Stream</span><span class="sxs-lookup"><span data-stu-id="0f89f-126">Stream</span></span> |<span data-ttu-id="0f89f-127">Получение двоичных данных ресурса файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="0f89f-127">Retrieve the binary data of a file or image resource.</span></span>|

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
