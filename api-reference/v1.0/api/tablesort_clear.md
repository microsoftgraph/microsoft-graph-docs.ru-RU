<span data-ttu-id="e711e-p103">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e711e-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.

## <span data-ttu-id="e711e-118">Пример</span><span class="sxs-lookup"><span data-stu-id="e711e-118">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="e711e-119">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e711e-119">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="e711e-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="e711e-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="e711e-121">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e711e-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <span data-ttu-id="e711e-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="e711e-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="e711e-123">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e711e-123">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->