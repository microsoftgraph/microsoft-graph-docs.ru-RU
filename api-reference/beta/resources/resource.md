---
title: Тип ресурса ресурса
description: 'Изображение или другой файловый ресурс на странице OneNote. '
localization_priority: Normal
ms.openlocfilehash: c85897af91290df83f4d6fccaf0552513b4f0535
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563023"
---
# <a name="resource-resource-type"></a><span data-ttu-id="ec1f6-103">Тип ресурса ресурса</span><span class="sxs-lookup"><span data-stu-id="ec1f6-103">resource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec1f6-104">Изображение или другой файловый ресурс на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="ec1f6-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="ec1f6-105">Вы можете получить двоичные данные ресурса, но получение представления объекта ресурса или коллекции ресурсов в формате JSON не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec1f6-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="ec1f6-106">Получение двоичных данных определенного ресурса путем отправки запроса GET в `content` конечную точку ресурса:</span><span class="sxs-lookup"><span data-stu-id="ec1f6-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="ec1f6-107">URI ресурса файла возвращается при получении HTML-контента страницы с помощью следующего запроса:</span><span class="sxs-lookup"><span data-stu-id="ec1f6-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="ec1f6-108">В HTML-коде страницы `img` тег включает конечные точки для исходного ресурса изображения в `data-fullres-src` атрибуте и оптимизированное изображение в `src` атрибуте:</span><span class="sxs-lookup"><span data-stu-id="ec1f6-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="ec1f6-109">`object` Тег, представляющий файлы, такие как PDF, docx и PNG, включает конечную точку для ресурса файла в `data` атрибуте:</span><span class="sxs-lookup"><span data-stu-id="ec1f6-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="ec1f6-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec1f6-110">Properties</span></span>
<span data-ttu-id="ec1f6-111">Нет</span><span class="sxs-lookup"><span data-stu-id="ec1f6-111">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="ec1f6-112">Связи</span><span class="sxs-lookup"><span data-stu-id="ec1f6-112">Relationships</span></span>
<span data-ttu-id="ec1f6-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="ec1f6-113">None.</span></span>


## <a name="methods"></a><span data-ttu-id="ec1f6-114">Методы</span><span class="sxs-lookup"><span data-stu-id="ec1f6-114">Methods</span></span>
| <span data-ttu-id="ec1f6-115">Метод</span><span class="sxs-lookup"><span data-stu-id="ec1f6-115">Method</span></span>           | <span data-ttu-id="ec1f6-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ec1f6-116">Return Type</span></span>    |<span data-ttu-id="ec1f6-117">Описание</span><span class="sxs-lookup"><span data-stu-id="ec1f6-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec1f6-118">Получение двоичных данных ресурса</span><span class="sxs-lookup"><span data-stu-id="ec1f6-118">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="ec1f6-119">Поток</span><span class="sxs-lookup"><span data-stu-id="ec1f6-119">Stream</span></span> |<span data-ttu-id="ec1f6-120">Получение двоичных данных ресурса файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="ec1f6-120">Retrieve the binary data of a file or image resource.</span></span>|

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
