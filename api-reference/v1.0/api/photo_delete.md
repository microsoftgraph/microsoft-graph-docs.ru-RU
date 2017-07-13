<span data-ttu-id="0539a-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0539a-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

## <span data-ttu-id="0539a-123">Пример</span><span class="sxs-lookup"><span data-stu-id="0539a-123">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="0539a-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="0539a-124">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="0539a-125">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0539a-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <span data-ttu-id="0539a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0539a-126">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="0539a-127">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0539a-127">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
