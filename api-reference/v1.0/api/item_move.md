<span data-ttu-id="a6c20-p103">**Примечание.** При перемещении элементов в корень OneDrive не следует использовать синтаксис `"id:" "root"`. Нужно использовать действительный идентификатор корневой папки или путь `{"path": "/drive/root"}` для родительской ссылки.</span><span class="sxs-lookup"><span data-stu-id="a6c20-p103">**Note:** When moving items to the root of a OneDrive you cannot use the `"id:" "root"` syntax. You either need to use the real ID of the root folder, or use `{"path": "/drive/root"}` for the parent reference.</span></span>

**Примечание.** При перемещении элементов в корень OneDrive не следует использовать синтаксис `"id:" "root"`. Нужно использовать действительный идентификатор корневой папки или путь `{"path": "/drive/root"}` для родительской ссылки.

## <span data-ttu-id="a6c20-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6c20-125">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a6c20-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6c20-126">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <span data-ttu-id="a6c20-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a6c20-127">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="a6c20-128">В этом примере элемент, определяемый идентификатором элемента {item-id}, перемещается в папку **Документы** в OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="a6c20-128">This example moves an item specified by {item-id} into the **Documents** folder in the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

## <span data-ttu-id="a6c20-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6c20-129">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a6c20-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a6c20-130">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
