# <a name="get-thumbnailset"></a><span data-ttu-id="10ad5-101">Получение объекта thumbnailSet</span><span class="sxs-lookup"><span data-stu-id="10ad5-101">Get thumbnailSet</span></span>

<span data-ttu-id="10ad5-102">Получение свойств и связей объекта [thumbnailSet](../resources/thumbnailset.md).</span><span class="sxs-lookup"><span data-stu-id="10ad5-102">Retrieve the properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.</span></span>

<span data-ttu-id="10ad5-103">Дополнительные сведения см. в описании операции [Список эскизов](item_list_thumbnails.md).</span><span class="sxs-lookup"><span data-stu-id="10ad5-103">For more info, see [List thumbnails](item_list_thumbnails.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="10ad5-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10ad5-104">Permissions</span></span>
<span data-ttu-id="10ad5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="10ad5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="10ad5-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10ad5-107">Permission type</span></span>      | <span data-ttu-id="10ad5-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10ad5-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="10ad5-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10ad5-109">Delegated (work or school account)</span></span> | <span data-ttu-id="10ad5-110">Files.Read</span><span class="sxs-lookup"><span data-stu-id="10ad5-110">Files.Read</span></span>    | 
|<span data-ttu-id="10ad5-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10ad5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10ad5-112">Files.Read</span><span class="sxs-lookup"><span data-stu-id="10ad5-112">Files.Read</span></span>    | 
|<span data-ttu-id="10ad5-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10ad5-113">Application</span></span> | <span data-ttu-id="10ad5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ad5-114">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="10ad5-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10ad5-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /drive/root/thumbnails/{id}
GET /drive/items/{id}/thumbnails/{id}
GET /drives/{id}/root/thumbnails/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10ad5-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10ad5-116">Optional query parameters</span></span>
<span data-ttu-id="10ad5-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="10ad5-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10ad5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10ad5-118">Request headers</span></span>
| <span data-ttu-id="10ad5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="10ad5-119">Name</span></span>       | <span data-ttu-id="10ad5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="10ad5-120">Type</span></span> | <span data-ttu-id="10ad5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="10ad5-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="10ad5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="10ad5-122">Authorization</span></span>  | <span data-ttu-id="10ad5-123">string</span><span class="sxs-lookup"><span data-stu-id="10ad5-123">string</span></span>  | <span data-ttu-id="10ad5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10ad5-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="10ad5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10ad5-126">Request body</span></span>
<span data-ttu-id="10ad5-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10ad5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10ad5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ad5-128">Response</span></span>

<span data-ttu-id="10ad5-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [thumbnailSet](../resources/thumbnailset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10ad5-129">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10ad5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="10ad5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10ad5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="10ad5-131">Request</span></span>
<span data-ttu-id="10ad5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10ad5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="10ad5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ad5-133">Response</span></span>
<span data-ttu-id="10ad5-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="10ad5-134">Here is an example of the response.</span></span>
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
