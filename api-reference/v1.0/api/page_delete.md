<span data-ttu-id="89967-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="89967-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <span data-ttu-id="89967-118">Пример</span><span class="sxs-lookup"><span data-stu-id="89967-118">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="89967-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="89967-119">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="89967-120">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89967-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <span data-ttu-id="89967-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="89967-121">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="89967-122">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="89967-122">Here is an example of the response.</span></span>
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
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->