<span data-ttu-id="329ba-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="329ba-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a><span data-ttu-id="329ba-119">Пример</span><span class="sxs-lookup"><span data-stu-id="329ba-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="329ba-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="329ba-120">Request</span></span>
<span data-ttu-id="329ba-121">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="329ba-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```
##### <a name="response"></a><span data-ttu-id="329ba-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="329ba-122">Response</span></span>
<span data-ttu-id="329ba-123">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="329ba-123">Here is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->