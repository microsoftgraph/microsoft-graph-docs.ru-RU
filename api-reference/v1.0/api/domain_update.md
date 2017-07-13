<span data-ttu-id="fb74c-p102">В теле запроса укажите значения для соответствующих полей, которые необходимо обновить. Существующие свойства, не включенные в тело запроса, сохранят имеющиеся значения либо будут пересчитаны на основании изменений других значений свойств. Для повышения производительности включайте только измененные значения.</span><span class="sxs-lookup"><span data-stu-id="fb74c-p102">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

В теле запроса укажите значения для соответствующих полей, которые необходимо обновить. Существующие свойства, не включенные в тело запроса, сохранят имеющиеся значения либо будут пересчитаны на основании изменений других значений свойств. Для повышения производительности включайте только измененные значения.

### <span data-ttu-id="fb74c-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb74c-120">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="fb74c-121">При успешном выполнении этот метод возвращает код отклика `204 No Content` и не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="fb74c-121">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

### <span data-ttu-id="fb74c-122">Пример</span><span class="sxs-lookup"><span data-stu-id="fb74c-122">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="fb74c-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb74c-123">Request</span></span>
<a id="request" class="xliff"></a>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/V1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <span data-ttu-id="fb74c-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb74c-124">Response</span></span>
<a id="response" class="xliff"></a>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->