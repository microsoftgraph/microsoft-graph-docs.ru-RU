# <a name="resource-resource-type"></a><span data-ttu-id="a13d3-101">Тип ресурса resource</span><span class="sxs-lookup"><span data-stu-id="a13d3-101">resource resource type</span></span>

<span data-ttu-id="a13d3-102">Ресурс изображения или другого файла на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="a13d3-102">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="a13d3-103">Вы можете получить двоичные данные ресурса, но получение представления объекта resource или коллекции resource в формате JSON не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a13d3-103">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="a13d3-104">Чтобы получить двоичные данные определенного ресурса, отправьте запрос GET в конечную точку `content` ресурса:</span><span class="sxs-lookup"><span data-stu-id="a13d3-104">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="a13d3-105">При получении HTML-контента страницы с использованием указанного ниже запроса возвращается URI ресурса файла.</span><span class="sxs-lookup"><span data-stu-id="a13d3-105">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="a13d3-106">На HTML-странице тег `img` включает конечные точки для исходного ресурса изображения в атрибуте `data-fullres-src` и оптимизированного изображения в атрибуте `src`:</span><span class="sxs-lookup"><span data-stu-id="a13d3-106">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="a13d3-107">Тег `object`, который представляет файлы, например PDF-, DOCX- и PNG-файлы, включает конечную точку для ресурса файла в атрибуте `data`:</span><span class="sxs-lookup"><span data-stu-id="a13d3-107">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="a13d3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a13d3-108">Properties</span></span>
<span data-ttu-id="a13d3-109">Нет</span><span class="sxs-lookup"><span data-stu-id="a13d3-109">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="a13d3-110">Связи</span><span class="sxs-lookup"><span data-stu-id="a13d3-110">Relationships</span></span>
<span data-ttu-id="a13d3-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a13d3-111">None.</span></span>


## <a name="methods"></a><span data-ttu-id="a13d3-112">Методы</span><span class="sxs-lookup"><span data-stu-id="a13d3-112">Methods</span></span>
| <span data-ttu-id="a13d3-113">Метод</span><span class="sxs-lookup"><span data-stu-id="a13d3-113">Method</span></span>           | <span data-ttu-id="a13d3-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a13d3-114">Return Type</span></span>    |<span data-ttu-id="a13d3-115">Описание</span><span class="sxs-lookup"><span data-stu-id="a13d3-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a13d3-116">Получения двоичных данных ресурса</span><span class="sxs-lookup"><span data-stu-id="a13d3-116">Get resource binary data</span></span>](../api/resource_get.md) | <span data-ttu-id="a13d3-117">Stream</span><span class="sxs-lookup"><span data-stu-id="a13d3-117">Stream</span></span> |<span data-ttu-id="a13d3-118">Получение двоичных данных ресурса файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="a13d3-118">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->