# <span data-ttu-id="e62f3-101">Список дочерних элементов ресурса driveItem.</span><span class="sxs-lookup"><span data-stu-id="e62f3-101">List children of a driveItem</span></span>
<a id="list-children-of-a-driveitem" class="xliff"></a>

<span data-ttu-id="e62f3-102">Возвращает коллекцию [DriveItems](../resources/driveitem.md) в **дочерние** элементы ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="e62f3-102">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="e62f3-103">Ресурсы DriveItem с аспектом **папки** или **пакета**, не равным NULL, могут содержать один или несколько дочерних элементов DriveItems.</span><span class="sxs-lookup"><span data-stu-id="e62f3-103">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <span data-ttu-id="e62f3-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e62f3-104">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="e62f3-105">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="e62f3-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="e62f3-106">Files.Read</span><span class="sxs-lookup"><span data-stu-id="e62f3-106">Files.Read</span></span>
* <span data-ttu-id="e62f3-107">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="e62f3-107">Files.ReadWrite</span></span>
* <span data-ttu-id="e62f3-108">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="e62f3-108">Files.Read.All</span></span>
* <span data-ttu-id="e62f3-109">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62f3-109">Files.ReadWrite.All</span></span>
* <span data-ttu-id="e62f3-110">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="e62f3-110">Sites.Read.All</span></span>
* <span data-ttu-id="e62f3-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62f3-111">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="e62f3-112">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e62f3-112">HTTP request</span></span>
<a id="http-request" class="xliff"></a>
```http
GET /me/drive/root/children
GET /me/drive/items/{item-id}/children
GET /me/drive/root:/{item-path}:/children
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/root/children
GET /groups/{group-id}/drive/items/{item-id}
```

## <span data-ttu-id="e62f3-113">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e62f3-113">Optional query parameters</span></span>
<a id="optional-query-parameters" class="xliff"></a>
<span data-ttu-id="e62f3-114">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e62f3-114">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <span data-ttu-id="e62f3-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e62f3-115">Request headers</span></span>
<a id="request-headers" class="xliff"></a>

| <span data-ttu-id="e62f3-116">Имя</span><span class="sxs-lookup"><span data-stu-id="e62f3-116">Name</span></span>          | <span data-ttu-id="e62f3-117">Тип</span><span class="sxs-lookup"><span data-stu-id="e62f3-117">Type</span></span>   | <span data-ttu-id="e62f3-118">Описание</span><span class="sxs-lookup"><span data-stu-id="e62f3-118">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e62f3-119">if-none-match</span><span class="sxs-lookup"><span data-stu-id="e62f3-119">if-none-match</span></span> | <span data-ttu-id="e62f3-120">String</span><span class="sxs-lookup"><span data-stu-id="e62f3-120">String</span></span> | <span data-ttu-id="e62f3-121">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то возвращается отклик `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="e62f3-121">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <span data-ttu-id="e62f3-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e62f3-122">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="e62f3-123">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e62f3-123">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="e62f3-124">Пример</span><span class="sxs-lookup"><span data-stu-id="e62f3-124">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="e62f3-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="e62f3-125">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="e62f3-126">Вот пример запроса на возвращение DriveItems в корневую папку OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="e62f3-126">Here is an example request to return the DriveItems in the root folder of the current user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_children"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children
```

## <span data-ttu-id="e62f3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e62f3-127">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="e62f3-128">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e62f3-128">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="e62f3-129">**Примечание.** Если коллекция превышает размер страницы по умолчанию (200 элементов), свойство **@odata.nextLink** возвращается в отклике, чтобы указать доступность дополнительных элементов и предоставить запрашиваемый URL-адрес для следующей страницы элементов.</span><span class="sxs-lookup"><span data-stu-id="e62f3-129">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="e62f3-130">Вы можете управлять размером страницы с помощью [необязательных параметров строки запроса](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span><span class="sxs-lookup"><span data-stu-id="e62f3-130">You can control the page size through [optional query string parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "OneDrive/DriveItem/List children"
} -->
