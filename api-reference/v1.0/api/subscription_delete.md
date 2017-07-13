<span data-ttu-id="a7ea7-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7ea7-p101">Bearer token. Required.</span></span>  | Bearer {токен}. Обязательный. |

## <span data-ttu-id="a7ea7-114">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="a7ea7-114">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="a7ea7-115">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7ea7-115">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="a7ea7-116">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7ea7-116">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a7ea7-117">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a7ea7-117">If successful, this method returns a `204 No Content` response code.</span></span>
## <span data-ttu-id="a7ea7-118">Пример</span><span class="sxs-lookup"><span data-stu-id="a7ea7-118">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="a7ea7-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7ea7-119">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="a7ea7-120">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7ea7-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <span data-ttu-id="a7ea7-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7ea7-121">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a7ea7-122">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a7ea7-122">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
