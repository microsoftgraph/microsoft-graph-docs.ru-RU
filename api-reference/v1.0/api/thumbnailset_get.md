<span data-ttu-id="f580d-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f580d-p101">Bearer token. Required.</span></span>  | Bearer {токен}. Обязательный. |


## <span data-ttu-id="f580d-118">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="f580d-118">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="f580d-119">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f580d-119">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="f580d-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="f580d-120">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="f580d-121">В случае успеха этот метод возвращает код отклика `200 OK` и объект [thumbnailSet](../resources/thumbnailset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f580d-121">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <span data-ttu-id="f580d-122">Пример</span><span class="sxs-lookup"><span data-stu-id="f580d-122">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="f580d-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="f580d-123">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="f580d-124">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f580d-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <span data-ttu-id="f580d-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="f580d-125">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="f580d-126">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f580d-126">Here is an example of the response.</span></span>
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
