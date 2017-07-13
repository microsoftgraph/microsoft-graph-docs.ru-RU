<span data-ttu-id="3af15-p103">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3af15-p103">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.

## <span data-ttu-id="3af15-120">Пример</span><span class="sxs-lookup"><span data-stu-id="3af15-120">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="3af15-121">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3af15-121">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="3af15-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="3af15-122">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="3af15-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3af15-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <span data-ttu-id="3af15-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="3af15-124">Response</span></span>
<a id="response" class="xliff"></a>
##### <span data-ttu-id="3af15-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="3af15-125">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="3af15-126">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3af15-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
