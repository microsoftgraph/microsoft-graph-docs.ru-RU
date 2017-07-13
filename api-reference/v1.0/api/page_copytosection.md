<span data-ttu-id="ebac1-p104">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation_get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="ebac1-p104">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>
В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation_get.md), опросите конечную точку Operation-Location.

## <span data-ttu-id="ebac1-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ebac1-134">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="ebac1-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ebac1-135">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="ebac1-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebac1-136">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="ebac1-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebac1-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <span data-ttu-id="ebac1-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebac1-138">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="ebac1-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ebac1-139">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->