<span data-ttu-id="0a5ba-p105">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0a5ba-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.

## <span data-ttu-id="0a5ba-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0a5ba-135">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="0a5ba-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0a5ba-136">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="0a5ba-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a5ba-137">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="0a5ba-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a5ba-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <span data-ttu-id="0a5ba-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a5ba-139">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="0a5ba-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0a5ba-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
