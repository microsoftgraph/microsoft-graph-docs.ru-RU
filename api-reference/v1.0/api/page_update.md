<span data-ttu-id="1f0b7-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`.  Для запроса PATCH не возвращается никаких данных JSON.</span><span class="sxs-lookup"><span data-stu-id="1f0b7-p103">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
При успешном выполнении этот метод возвращает код отклика `204 No Content`.  Для запроса PATCH не возвращается никаких данных JSON.
## <span data-ttu-id="1f0b7-123">Пример</span><span class="sxs-lookup"><span data-stu-id="1f0b7-123">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="1f0b7-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f0b7-124">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="1f0b7-125">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f0b7-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <span data-ttu-id="1f0b7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f0b7-126">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="1f0b7-127">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1f0b7-127">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
