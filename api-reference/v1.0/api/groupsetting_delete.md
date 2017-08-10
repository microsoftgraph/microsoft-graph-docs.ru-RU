<span data-ttu-id="ec309-p102">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает никакие данные в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec309-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает никакие данные в тексте отклика.

## <a name="example"></a><span data-ttu-id="ec309-120">Пример</span><span class="sxs-lookup"><span data-stu-id="ec309-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec309-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec309-121">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="ec309-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec309-122">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->