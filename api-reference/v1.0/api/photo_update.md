<span data-ttu-id="0f1de-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0f1de-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| <span data-ttu-id="0f1de-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f1de-118">Property</span></span>     | <span data-ttu-id="0f1de-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0f1de-119">Type</span></span>   |<span data-ttu-id="0f1de-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0f1de-120">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="0f1de-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f1de-121">Response</span></span>

<span data-ttu-id="0f1de-122">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0f1de-122">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f1de-123">Пример</span><span class="sxs-lookup"><span data-stu-id="0f1de-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f1de-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f1de-124">Request</span></span>
<span data-ttu-id="0f1de-125">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f1de-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="0f1de-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f1de-126">Response</span></span>
<span data-ttu-id="0f1de-127">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0f1de-127">Here is an example of the response.</span></span>
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
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
