# <a name="get-thumbnailset"></a><span data-ttu-id="d8c4e-101">Получение объекта thumbnailSet</span><span class="sxs-lookup"><span data-stu-id="d8c4e-101">Get thumbnailSet</span></span>

<span data-ttu-id="d8c4e-102">Получение свойств и связей объекта [thumbnailSet](../resources/thumbnailset.md).</span><span class="sxs-lookup"><span data-stu-id="d8c4e-102">Retrieve the properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.</span></span>

<span data-ttu-id="d8c4e-103">Дополнительные сведения см. в описании операции [Список эскизов](item_list_thumbnails.md).</span><span class="sxs-lookup"><span data-stu-id="d8c4e-103">For more info, see [List thumbnails](item_list_thumbnails.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8c4e-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="d8c4e-104">Prerequisites</span></span>
<span data-ttu-id="d8c4e-105">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="d8c4e-105">One of the following **scopes** is required to execute this API:</span></span>

  * <span data-ttu-id="d8c4e-106">Files.Read</span><span class="sxs-lookup"><span data-stu-id="d8c4e-106">Files.Read</span></span>

## <a name="http-request"></a><span data-ttu-id="d8c4e-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8c4e-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /drive/root/thumbnails/{id}
GET /drive/items/{id}/thumbnails/{id}
GET /drives/{id}/root/thumbnails/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8c4e-108">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d8c4e-108">Optional query parameters</span></span>
<span data-ttu-id="d8c4e-109">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d8c4e-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8c4e-110">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8c4e-110">Request headers</span></span>
| <span data-ttu-id="d8c4e-111">Имя</span><span class="sxs-lookup"><span data-stu-id="d8c4e-111">Name</span></span>       | <span data-ttu-id="d8c4e-112">Тип</span><span class="sxs-lookup"><span data-stu-id="d8c4e-112">Type</span></span> | <span data-ttu-id="d8c4e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d8c4e-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d8c4e-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8c4e-114">Authorization</span></span>  | <span data-ttu-id="d8c4e-115">string</span><span class="sxs-lookup"><span data-stu-id="d8c4e-115">string</span></span>  | <span data-ttu-id="d8c4e-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8c4e-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8c4e-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8c4e-118">Request body</span></span>
<span data-ttu-id="d8c4e-119">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8c4e-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8c4e-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8c4e-120">Response</span></span>

<span data-ttu-id="d8c4e-121">В случае успеха этот метод возвращает код отклика `200 OK` и объект [thumbnailSet](../resources/thumbnailset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8c4e-121">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8c4e-122">Пример</span><span class="sxs-lookup"><span data-stu-id="d8c4e-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8c4e-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8c4e-123">Request</span></span>
<span data-ttu-id="d8c4e-124">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8c4e-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="d8c4e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8c4e-125">Response</span></span>
<span data-ttu-id="d8c4e-126">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d8c4e-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 456

{
  "id": "id-value",
  "large": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "medium": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "small": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "source": {
    "height": 99,
    "url": "url-value",
    "width": 99
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get thumbnailSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
