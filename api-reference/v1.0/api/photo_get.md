<span data-ttu-id="c1988-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1988-p101">Bearer token. Required.</span></span>  | Bearer {токен}. Обязательный. |

## <span data-ttu-id="c1988-117">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="c1988-117">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="c1988-118">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c1988-118">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="c1988-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1988-119">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="c1988-120">В случае успеха этот метод возвращает код отклика `200 OK` и объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1988-120">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <span data-ttu-id="c1988-121">Пример</span><span class="sxs-lookup"><span data-stu-id="c1988-121">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="c1988-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1988-122">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="c1988-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1988-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <span data-ttu-id="c1988-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1988-124">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="c1988-125">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c1988-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
