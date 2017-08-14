<span data-ttu-id="bb19a-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bb19a-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a><span data-ttu-id="bb19a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bb19a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb19a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb19a-131">Request</span></span>
<span data-ttu-id="bb19a-132">Ниже приведен пример запроса на удаление вложения из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="bb19a-132">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="bb19a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb19a-133">Response</span></span>
<span data-ttu-id="bb19a-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bb19a-134">Here is an example of the response.</span></span>
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
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
