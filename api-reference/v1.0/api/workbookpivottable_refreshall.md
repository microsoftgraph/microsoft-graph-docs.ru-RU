<span data-ttu-id="cd23c-p103">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. Метод не возвращает никакие данные в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd23c-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `200, OK`. Метод не возвращает никакие данные в тексте отклика.

## <a name="example"></a><span data-ttu-id="cd23c-119">Пример</span><span class="sxs-lookup"><span data-stu-id="cd23c-119">Example</span></span>
<span data-ttu-id="cd23c-120">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cd23c-120">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cd23c-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd23c-121">Request</span></span>
<span data-ttu-id="cd23c-122">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd23c-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="cd23c-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd23c-123">Response</span></span>
<span data-ttu-id="cd23c-124">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cd23c-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
