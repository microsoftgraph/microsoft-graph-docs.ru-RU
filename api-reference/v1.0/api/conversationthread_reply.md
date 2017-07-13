<span data-ttu-id="f9d14-p104">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f9d14-p104">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.

## <span data-ttu-id="f9d14-127">Пример</span><span class="sxs-lookup"><span data-stu-id="f9d14-127">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="f9d14-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f9d14-128">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="f9d14-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9d14-129">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="f9d14-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9d14-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <span data-ttu-id="f9d14-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9d14-131">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="f9d14-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f9d14-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
