# <a name="get-a-driveitem-resource"></a><span data-ttu-id="5ea5d-101">Получение ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="5ea5d-101">Get a DriveItem resource</span></span>

<span data-ttu-id="5ea5d-102">Получение метаданных для ресурса [DriveItem](../resources/driveitem.md) в объекте [Drive](../resources/drive.md) по пути в файловой системе или идентификатору.</span><span class="sxs-lookup"><span data-stu-id="5ea5d-102">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ea5d-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="5ea5d-103">Prerequisites</span></span>
<span data-ttu-id="5ea5d-104">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="5ea5d-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="5ea5d-105">Files.Read</span><span class="sxs-lookup"><span data-stu-id="5ea5d-105">Files.Read</span></span>
* <span data-ttu-id="5ea5d-106">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="5ea5d-106">Files.ReadWrite</span></span>
* <span data-ttu-id="5ea5d-107">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ea5d-107">Files.Read.All</span></span>
* <span data-ttu-id="5ea5d-108">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ea5d-108">Files.ReadWrite.All</span></span>
* <span data-ttu-id="5ea5d-109">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ea5d-109">Sites.Read.All</span></span>
* <span data-ttu-id="5ea5d-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ea5d-110">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="5ea5d-111">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ea5d-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /drives/{drive-id}/items/{item-id}
GET /groups/{group-id}/drive/items/{item-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ea5d-112">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5ea5d-112">Optional query parameters</span></span>
<span data-ttu-id="5ea5d-113">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5ea5d-113">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ea5d-114">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ea5d-114">Request headers</span></span>

| <span data-ttu-id="5ea5d-115">Имя</span><span class="sxs-lookup"><span data-stu-id="5ea5d-115">Name</span></span>          | <span data-ttu-id="5ea5d-116">Значение</span><span class="sxs-lookup"><span data-stu-id="5ea5d-116">Value</span></span>  | <span data-ttu-id="5ea5d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="5ea5d-117">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5ea5d-118">if-none-match</span><span class="sxs-lookup"><span data-stu-id="5ea5d-118">if-none-match</span></span> | <span data-ttu-id="5ea5d-119">String</span><span class="sxs-lookup"><span data-stu-id="5ea5d-119">String</span></span> | <span data-ttu-id="5ea5d-120">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то возвращается отклик `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="5ea5d-120">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5ea5d-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ea5d-121">Request body</span></span>
<span data-ttu-id="5ea5d-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ea5d-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ea5d-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ea5d-123">Response</span></span>

<span data-ttu-id="5ea5d-124">В случае успеха этот метод возвращает код отклика `200 OK` и ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5ea5d-124">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea5d-125">Пример</span><span class="sxs-lookup"><span data-stu-id="5ea5d-125">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5ea5d-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ea5d-126">Request</span></span>

<span data-ttu-id="5ea5d-127">Ниже приведен пример запроса к корневой папке OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="5ea5d-127">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item"
}-->
```
GET https://graph.microsoft.com/v1.0//me/drive/root
```

##### <a name="response"></a><span data-ttu-id="5ea5d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ea5d-128">Response</span></span>
<span data-ttu-id="5ea5d-129">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5ea5d-129">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <a name="notes"></a><span data-ttu-id="5ea5d-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="5ea5d-130">Notes</span></span>

<span data-ttu-id="5ea5d-131">С помощью [`$expand`параметра строки запроса](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) вы можете включить дочерние элементы запрос на получение метаданных элемента при наличии **дочерней** связи.</span><span class="sxs-lookup"><span data-stu-id="5ea5d-131">You can use the [`$expand` query string parameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get item"
}-->
