<span data-ttu-id="abd14-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abd14-p102">Bearer token. Required.</span></span>  | Bearer {токен}. Обязательный.  |

## <span data-ttu-id="abd14-115">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abd14-115">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="abd14-116">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="abd14-116">In the request body, supply the id of a user or group object.</span></span>


## <span data-ttu-id="abd14-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="abd14-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="abd14-118">Этот метод возвращает код отклика `204, No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="abd14-118">This method returns `204, No Content` response code and no response body.</span></span>

## <span data-ttu-id="abd14-119">Пример</span><span class="sxs-lookup"><span data-stu-id="abd14-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="abd14-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="abd14-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="abd14-121">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abd14-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <span data-ttu-id="abd14-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="abd14-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="abd14-123">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="abd14-123">Here is an example of the response.</span></span>
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
