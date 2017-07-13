<span data-ttu-id="dbfa6-p103">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dbfa6-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.

## <span data-ttu-id="dbfa6-125">Пример</span><span class="sxs-lookup"><span data-stu-id="dbfa6-125">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="dbfa6-126">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dbfa6-126">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="dbfa6-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbfa6-127">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="dbfa6-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbfa6-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "datetime-value",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "datetime-value",
    "lastModifiedDateTime": "datetime-value",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "datetime-value",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```

##### <span data-ttu-id="dbfa6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbfa6-129">Response</span></span>
<a id="response" class="xliff"></a>
##### <span data-ttu-id="dbfa6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbfa6-130">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="dbfa6-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dbfa6-131">Here is an example of the response.</span></span>
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
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
