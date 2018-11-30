---
title: Тип ресурса resource
description: 'Ресурс изображения или другого файла на странице OneNote. '
ms.openlocfilehash: 8e0e049cab613c7c1a72c8c96e21bac77c507ae1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080558"
---
# <a name="resource-resource-type"></a><span data-ttu-id="bad92-103">Тип ресурса resource</span><span class="sxs-lookup"><span data-stu-id="bad92-103">resource resource type</span></span>

> <span data-ttu-id="bad92-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bad92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bad92-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bad92-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bad92-106">Ресурс изображения или другого файла на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="bad92-106">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="bad92-107">Вы можете получить двоичные данные ресурса, но получение представления объекта resource или коллекции resource в формате JSON не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bad92-107">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="bad92-108">Чтобы получить двоичные данные определенного ресурса, отправьте запрос GET в конечную точку `content` ресурса:</span><span class="sxs-lookup"><span data-stu-id="bad92-108">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="bad92-109">При получении HTML-контента страницы с использованием указанного ниже запроса возвращается URI ресурса файла.</span><span class="sxs-lookup"><span data-stu-id="bad92-109">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="bad92-110">На HTML-странице тег `img` включает конечные точки для исходного ресурса изображения в атрибуте `data-fullres-src` и оптимизированного изображения в атрибуте `src`:</span><span class="sxs-lookup"><span data-stu-id="bad92-110">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="bad92-111">Тег `object`, который представляет файлы, например PDF-, DOCX- и PNG-файлы, включает конечную точку для ресурса файла в атрибуте `data`:</span><span class="sxs-lookup"><span data-stu-id="bad92-111">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="bad92-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="bad92-112">Properties</span></span>
<span data-ttu-id="bad92-113">Нет</span><span class="sxs-lookup"><span data-stu-id="bad92-113">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="bad92-114">Связи</span><span class="sxs-lookup"><span data-stu-id="bad92-114">Relationships</span></span>
<span data-ttu-id="bad92-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="bad92-115">None.</span></span>


## <a name="methods"></a><span data-ttu-id="bad92-116">Методы</span><span class="sxs-lookup"><span data-stu-id="bad92-116">Methods</span></span>
| <span data-ttu-id="bad92-117">Метод</span><span class="sxs-lookup"><span data-stu-id="bad92-117">Method</span></span>           | <span data-ttu-id="bad92-118">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bad92-118">Return Type</span></span>    |<span data-ttu-id="bad92-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bad92-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bad92-120">Получения двоичных данных ресурса</span><span class="sxs-lookup"><span data-stu-id="bad92-120">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="bad92-121">Stream</span><span class="sxs-lookup"><span data-stu-id="bad92-121">Stream</span></span> |<span data-ttu-id="bad92-122">Получение двоичных данных ресурса файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="bad92-122">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->