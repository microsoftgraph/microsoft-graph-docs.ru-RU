<span data-ttu-id="669cd-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="669cd-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

## <span data-ttu-id="669cd-117">Пример</span><span class="sxs-lookup"><span data-stu-id="669cd-117">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="669cd-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="669cd-118">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="669cd-119">Ниже представлено несколько примеров запроса.</span><span class="sxs-lookup"><span data-stu-id="669cd-119">Here are a couple of examples of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id="users/{id}"

DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id="groups/{id}"
```

##### <span data-ttu-id="669cd-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="669cd-120">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="669cd-121">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="669cd-121">Here is an example of the response.</span></span> 
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->