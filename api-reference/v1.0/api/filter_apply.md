<span data-ttu-id="cf233-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cf233-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.

## <span data-ttu-id="cf233-124">Пример</span><span class="sxs-lookup"><span data-stu-id="cf233-124">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="cf233-125">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cf233-125">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="cf233-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf233-126">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="cf233-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf233-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <span data-ttu-id="cf233-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf233-128">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="cf233-129">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cf233-129">Here is an example of the response.</span></span> 
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->