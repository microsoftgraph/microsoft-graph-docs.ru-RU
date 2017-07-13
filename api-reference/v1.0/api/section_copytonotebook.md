<span data-ttu-id="552f6-p105">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation_get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="552f6-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>
В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation_get.md), опросите конечную точку Operation-Location.

## <span data-ttu-id="552f6-138">Пример</span><span class="sxs-lookup"><span data-stu-id="552f6-138">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="552f6-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="552f6-139">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="552f6-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="552f6-140">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="552f6-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="552f6-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <span data-ttu-id="552f6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="552f6-142">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="552f6-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="552f6-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->