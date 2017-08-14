<span data-ttu-id="8775f-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8775f-p101">Bearer {token}. Required.</span></span>  | Bearer {токен}. Обязательный. |
| <span data-ttu-id="8775f-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8775f-114">Content-Type</span></span>  | <span data-ttu-id="8775f-115">application/json</span><span class="sxs-lookup"><span data-stu-id="8775f-115">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8775f-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8775f-116">Request body</span></span>
<span data-ttu-id="8775f-117">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8775f-117">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="8775f-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="8775f-118">Response</span></span>

<span data-ttu-id="8775f-119">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`.</span><span class="sxs-lookup"><span data-stu-id="8775f-119">If successful, this method returns `204, No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8775f-120">Пример</span><span class="sxs-lookup"><span data-stu-id="8775f-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8775f-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="8775f-121">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="8775f-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="8775f-122">Response</span></span>
<span data-ttu-id="8775f-123">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="8775f-123">Note: The response object shown here may be truncated for brevity.</span></span> 
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