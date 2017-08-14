<span data-ttu-id="3c17b-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3c17b-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a><span data-ttu-id="3c17b-121">Пример</span><span class="sxs-lookup"><span data-stu-id="3c17b-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c17b-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c17b-122">Request</span></span>
<span data-ttu-id="3c17b-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c17b-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="3c17b-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c17b-124">Response</span></span>
<span data-ttu-id="3c17b-125">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3c17b-125">Here is an example of the response.</span></span> 
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
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
