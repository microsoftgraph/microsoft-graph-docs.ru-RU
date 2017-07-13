<span data-ttu-id="920ab-p105">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="920ab-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.

## <span data-ttu-id="920ab-133">Пример</span><span class="sxs-lookup"><span data-stu-id="920ab-133">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="920ab-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="920ab-134">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="920ab-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="920ab-135">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="920ab-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="920ab-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json
Content-length: 512

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```

##### <span data-ttu-id="920ab-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="920ab-137">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="920ab-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="920ab-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
