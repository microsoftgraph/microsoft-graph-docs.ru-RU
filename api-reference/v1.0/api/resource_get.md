<span data-ttu-id="6d2f0-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d2f0-p101">Bearer token. Required.</span></span>  | Bearer {токен}. Обязательный. |

## <span data-ttu-id="6d2f0-115">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="6d2f0-115">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="6d2f0-116">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d2f0-116">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="6d2f0-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d2f0-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="6d2f0-118">При успешном выполнении это метод возвращает код отклика `200 OK` и двоичные данные изображения или файла в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6d2f0-118">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="6d2f0-119">Примечание. Изображения не будут отображаться непосредственно в браузере, так как для их получения необходима авторизация (как и для остальной части содержимого страницы).</span><span class="sxs-lookup"><span data-stu-id="6d2f0-119">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <span data-ttu-id="6d2f0-120">Пример</span><span class="sxs-lookup"><span data-stu-id="6d2f0-120">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="6d2f0-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d2f0-121">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="6d2f0-122">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d2f0-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <span data-ttu-id="6d2f0-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d2f0-123">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="6d2f0-124">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6d2f0-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
