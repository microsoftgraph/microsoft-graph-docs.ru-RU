<span data-ttu-id="197a9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="197a9-p102">Bearer token. Required.</span></span>  | Bearer {токен}. Обязательный.  |
| <span data-ttu-id="197a9-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="197a9-115">Content-Type</span></span>   | <span data-ttu-id="197a9-116">application/json</span><span class="sxs-lookup"><span data-stu-id="197a9-116">application/json</span></span>  | 

## <span data-ttu-id="197a9-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="197a9-117">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="197a9-118">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="197a9-118">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="197a9-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="197a9-119">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="197a9-120">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="197a9-120">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <span data-ttu-id="197a9-121">Пример</span><span class="sxs-lookup"><span data-stu-id="197a9-121">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="197a9-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="197a9-122">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="197a9-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="197a9-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <span data-ttu-id="197a9-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="197a9-124">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="197a9-125">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="197a9-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
