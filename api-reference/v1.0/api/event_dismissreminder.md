<span data-ttu-id="58f89-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="58f89-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a><span data-ttu-id="58f89-118">Пример</span><span class="sxs-lookup"><span data-stu-id="58f89-118">Example</span></span>
<span data-ttu-id="58f89-119">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="58f89-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="58f89-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="58f89-120">Request</span></span>
<span data-ttu-id="58f89-121">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58f89-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

##### <a name="response"></a><span data-ttu-id="58f89-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="58f89-122">Response</span></span>
##### <a name="response"></a><span data-ttu-id="58f89-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="58f89-123">Response</span></span>
<span data-ttu-id="58f89-124">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="58f89-124">Here is an example of the response.</span></span>
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
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
