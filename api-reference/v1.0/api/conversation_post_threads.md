<span data-ttu-id="0b2f4-p103">В случае успеха этот метод возвратит код отклика `201, Created` и `id` новой цепочки в теле отклика. Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b2f4-p103">If successful, this method returns `201, Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>

В случае успеха этот метод возвратит код отклика `201, Created` и `id` новой цепочки в теле отклика. Ниже приведен пример отклика. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
