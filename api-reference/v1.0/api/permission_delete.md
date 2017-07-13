<span data-ttu-id="c4ecd-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c4ecd-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <span data-ttu-id="c4ecd-123">Пример</span><span class="sxs-lookup"><span data-stu-id="c4ecd-123">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="c4ecd-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4ecd-124">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="c4ecd-125">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4ecd-125">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permission"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/root/items/{item-id}/permissions/{perm-id}
```

##### <span data-ttu-id="c4ecd-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4ecd-126">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="c4ecd-127">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4ecd-127">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <span data-ttu-id="c4ecd-128">Заметки</span><span class="sxs-lookup"><span data-stu-id="c4ecd-128">Remarks</span></span>
<a id="remarks" class="xliff"></a>

* <span data-ttu-id="c4ecd-129">[Диски](../resources/drive.md), у которых для свойства **driveType** задано значение `personal` (личное хранилище OneDrive), не могут создавать и изменять разрешения в корневом ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="c4ecd-129">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
