---
title: Тип ресурса resource
description: 'Ресурс изображения или другого файла на странице OneNote. '
localization_priority: Normal
ms.openlocfilehash: c85897af91290df83f4d6fccaf0552513b4f0535
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510283"
---
# <a name="resource-resource-type"></a><span data-ttu-id="abb10-103">Тип ресурса resource</span><span class="sxs-lookup"><span data-stu-id="abb10-103">resource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abb10-104">Ресурс изображения или другого файла на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="abb10-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="abb10-105">Вы можете получить двоичные данные ресурса, но получение представления объекта resource или коллекции resource в формате JSON не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abb10-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="abb10-106">Чтобы получить двоичные данные определенного ресурса, отправьте запрос GET в конечную точку `content` ресурса:</span><span class="sxs-lookup"><span data-stu-id="abb10-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="abb10-107">При получении HTML-контента страницы с использованием указанного ниже запроса возвращается URI ресурса файла.</span><span class="sxs-lookup"><span data-stu-id="abb10-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="abb10-108">На HTML-странице тег `img` включает конечные точки для исходного ресурса изображения в атрибуте `data-fullres-src` и оптимизированного изображения в атрибуте `src`:</span><span class="sxs-lookup"><span data-stu-id="abb10-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="abb10-109">Тег `object`, который представляет файлы, например PDF-, DOCX- и PNG-файлы, включает конечную точку для ресурса файла в атрибуте `data`:</span><span class="sxs-lookup"><span data-stu-id="abb10-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="abb10-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="abb10-110">Properties</span></span>
<span data-ttu-id="abb10-111">Нет</span><span class="sxs-lookup"><span data-stu-id="abb10-111">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="abb10-112">Связи</span><span class="sxs-lookup"><span data-stu-id="abb10-112">Relationships</span></span>
<span data-ttu-id="abb10-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="abb10-113">None.</span></span>


## <a name="methods"></a><span data-ttu-id="abb10-114">Методы</span><span class="sxs-lookup"><span data-stu-id="abb10-114">Methods</span></span>
| <span data-ttu-id="abb10-115">Метод</span><span class="sxs-lookup"><span data-stu-id="abb10-115">Method</span></span>           | <span data-ttu-id="abb10-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="abb10-116">Return Type</span></span>    |<span data-ttu-id="abb10-117">Описание</span><span class="sxs-lookup"><span data-stu-id="abb10-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="abb10-118">Получения двоичных данных ресурса</span><span class="sxs-lookup"><span data-stu-id="abb10-118">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="abb10-119">Stream</span><span class="sxs-lookup"><span data-stu-id="abb10-119">Stream</span></span> |<span data-ttu-id="abb10-120">Получение двоичных данных ресурса файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="abb10-120">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
