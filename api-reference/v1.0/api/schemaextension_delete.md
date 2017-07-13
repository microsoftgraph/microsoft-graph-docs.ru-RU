<span data-ttu-id="d0b1f-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d0b1f-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

## <span data-ttu-id="d0b1f-119">Пример</span><span class="sxs-lookup"><span data-stu-id="d0b1f-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="d0b1f-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0b1f-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="d0b1f-121">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0b1f-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <span data-ttu-id="d0b1f-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0b1f-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="d0b1f-123">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d0b1f-123">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <span data-ttu-id="d0b1f-124">См. также</span><span class="sxs-lookup"><span data-stu-id="d0b1f-124">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="d0b1f-125">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="d0b1f-125">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="d0b1f-126">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="d0b1f-126">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->