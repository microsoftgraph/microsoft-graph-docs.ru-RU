<span data-ttu-id="cfec9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfec9-p102">Bearer token. Required.</span></span>  | Bearer {токен}. Обязательный. |

## <span data-ttu-id="cfec9-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfec9-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="cfec9-118">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cfec9-118">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <span data-ttu-id="cfec9-119">Пример</span><span class="sxs-lookup"><span data-stu-id="cfec9-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="cfec9-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfec9-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="cfec9-121">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfec9-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <span data-ttu-id="cfec9-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfec9-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="cfec9-123">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cfec9-123">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
