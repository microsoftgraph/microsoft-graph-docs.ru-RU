<span data-ttu-id="5c24d-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5c24d-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a><span data-ttu-id="5c24d-124">Пример</span><span class="sxs-lookup"><span data-stu-id="5c24d-124">Example</span></span>
<span data-ttu-id="5c24d-125">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5c24d-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5c24d-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c24d-126">Request</span></span>
<span data-ttu-id="5c24d-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c24d-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="5c24d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c24d-128">Response</span></span>
<span data-ttu-id="5c24d-129">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5c24d-129">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->