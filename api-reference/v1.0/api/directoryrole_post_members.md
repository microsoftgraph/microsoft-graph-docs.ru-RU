<span data-ttu-id="abfb9-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abfb9-p101">Bearer token. Required.</span></span>  | Bearer {токен}. Обязательный. |
| <span data-ttu-id="abfb9-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="abfb9-114">Content-Type</span></span>  | <span data-ttu-id="abfb9-115">application/json</span><span class="sxs-lookup"><span data-stu-id="abfb9-115">application/json</span></span>  |

## <span data-ttu-id="abfb9-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abfb9-116">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="abfb9-117">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abfb9-117">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <span data-ttu-id="abfb9-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="abfb9-118">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="abfb9-119">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`.</span><span class="sxs-lookup"><span data-stu-id="abfb9-119">If successful, this method returns `204, No Content` response code.</span></span>

## <span data-ttu-id="abfb9-120">Пример</span><span class="sxs-lookup"><span data-stu-id="abfb9-120">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="abfb9-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="abfb9-121">Request</span></span>
<a id="request" class="xliff"></a>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <span data-ttu-id="abfb9-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="abfb9-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="abfb9-123">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="abfb9-123">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->