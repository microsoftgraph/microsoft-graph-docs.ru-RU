<span data-ttu-id="bcce3-p120">Ошибки возвращаются с HTTP-кодом и объектом ошибки. Ошибки `code` и `message` объясняют причины возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="bcce3-p120">Errors are returned with an HTTP error code and an error object. An error `code` and `message` explain the reason for the error.</span></span> 

Ошибки возвращаются с HTTP-кодом и объектом ошибки. Ошибки `code` и `message` объясняют причины возникновения ошибки.
 
<span data-ttu-id="bcce3-277">Пример.</span><span class="sxs-lookup"><span data-stu-id="bcce3-277">The following is an example.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 400 Bad Request
Content-Type: application/json

{
  "error": {
    "code": "ItemAlreadyExists",
    "message": "A resource with the same name or identifier already exists.",
    "innerError": {
      "request-id": "214ca7ea-9ea4-442e-9c67-71fdda0a559c",
      "date": "2016-07-28T03:56:09"
    }
  }
}
```

