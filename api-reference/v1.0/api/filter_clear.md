<span data-ttu-id="caee8-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="caee8-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a><span data-ttu-id="caee8-117">Пример</span><span class="sxs-lookup"><span data-stu-id="caee8-117">Example</span></span>
<span data-ttu-id="caee8-118">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="caee8-118">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="caee8-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="caee8-119">Request</span></span>
<span data-ttu-id="caee8-120">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="caee8-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="caee8-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="caee8-121">Response</span></span>
<span data-ttu-id="caee8-122">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="caee8-122">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->