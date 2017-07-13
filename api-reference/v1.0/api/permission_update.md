<span data-ttu-id="43da9-p101">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="43da9-p101">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| <span data-ttu-id="43da9-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="43da9-120">Property</span></span>     | <span data-ttu-id="43da9-121">Тип</span><span class="sxs-lookup"><span data-stu-id="43da9-121">Type</span></span>   | <span data-ttu-id="43da9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="43da9-122">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="43da9-123">**roles**</span><span class="sxs-lookup"><span data-stu-id="43da9-123">**roles**</span></span>    | <span data-ttu-id="43da9-124">String</span><span class="sxs-lookup"><span data-stu-id="43da9-124">String</span></span> | <span data-ttu-id="43da9-125">Массив типов разрешений.</span><span class="sxs-lookup"><span data-stu-id="43da9-125">An array of permission types.</span></span> |


## <span data-ttu-id="43da9-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="43da9-126">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="43da9-127">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [permission](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43da9-127">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <span data-ttu-id="43da9-128">Пример</span><span class="sxs-lookup"><span data-stu-id="43da9-128">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="43da9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="43da9-129">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="43da9-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43da9-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
##### <span data-ttu-id="43da9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="43da9-131">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="43da9-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="43da9-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
