# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="f2fc4-101">Список дочерних элементов ресурса driveItem.</span><span class="sxs-lookup"><span data-stu-id="f2fc4-101">List children of a driveItem</span></span>

<span data-ttu-id="f2fc4-102">Возвращает коллекцию [DriveItems](../resources/driveitem.md) в **дочерние** элементы ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="f2fc4-102">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="f2fc4-103">Ресурсы DriveItem с аспектом **папки** или **пакета**, отличным от NULL, могут содержать один или несколько дочерних элементов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="f2fc4-103">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="f2fc4-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2fc4-104">Permissions</span></span>
<span data-ttu-id="f2fc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f2fc4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2fc4-107">Permission type</span></span>      | <span data-ttu-id="f2fc4-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2fc4-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="f2fc4-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2fc4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f2fc4-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2fc4-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="f2fc4-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2fc4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2fc4-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2fc4-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="f2fc4-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2fc4-113">Application</span></span> | <span data-ttu-id="f2fc4-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2fc4-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f2fc4-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2fc4-115">HTTP request</span></span>
```http
GET /me/drive/root/children
GET /me/drive/items/{item-id}/children
GET /me/drive/root:/{item-path}:/children
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/root/children
GET /groups/{group-id}/drive/items/{item-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2fc4-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2fc4-116">Optional query parameters</span></span>
<span data-ttu-id="f2fc4-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f2fc4-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2fc4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2fc4-118">Request headers</span></span>

| <span data-ttu-id="f2fc4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f2fc4-119">Name</span></span>          | <span data-ttu-id="f2fc4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f2fc4-120">Type</span></span>   | <span data-ttu-id="f2fc4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f2fc4-121">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f2fc4-122">if-none-match</span><span class="sxs-lookup"><span data-stu-id="f2fc4-122">if-none-match</span></span> | <span data-ttu-id="f2fc4-123">String</span><span class="sxs-lookup"><span data-stu-id="f2fc4-123">String</span></span> | <span data-ttu-id="f2fc4-124">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то возвращается отклик `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="f2fc4-124">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2fc4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2fc4-125">Request body</span></span>
<span data-ttu-id="f2fc4-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2fc4-126">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="f2fc4-127">Пример</span><span class="sxs-lookup"><span data-stu-id="f2fc4-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f2fc4-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2fc4-128">Request</span></span>
<span data-ttu-id="f2fc4-129">Вот пример запроса на возвращение DriveItems в корневую папку OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="f2fc4-129">Here is an example request to return the DriveItems in the root folder of the current user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_children"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children
```

## <a name="response"></a><span data-ttu-id="f2fc4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2fc4-130">Response</span></span>

<span data-ttu-id="f2fc4-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f2fc4-131">Here is an example of the response.</span></span>
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

<span data-ttu-id="f2fc4-132">**Примечание.** Если коллекция превышает размер страницы по умолчанию (200 элементов), свойство **@odata.nextLink** возвращается в отклике, чтобы указать доступность дополнительных элементов и предоставить запрашиваемый URL-адрес для следующей страницы элементов.</span><span class="sxs-lookup"><span data-stu-id="f2fc4-132">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="f2fc4-133">Вы можете управлять размером страницы с помощью [необязательных параметров строки запроса](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span><span class="sxs-lookup"><span data-stu-id="f2fc4-133">You can control the page size through [optional query string parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "OneDrive/DriveItem/List children"
} -->
