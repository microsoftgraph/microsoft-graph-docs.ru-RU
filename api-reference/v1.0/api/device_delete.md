<span data-ttu-id="ed2a6-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ed2a6-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

## <span data-ttu-id="ed2a6-120">Пример</span><span class="sxs-lookup"><span data-stu-id="ed2a6-120">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="ed2a6-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed2a6-121">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="ed2a6-122">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed2a6-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <span data-ttu-id="ed2a6-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed2a6-123">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="ed2a6-124">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ed2a6-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
