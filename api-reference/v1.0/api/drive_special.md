<span data-ttu-id="b3bdc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3bdc-p103">Bearer {token}. Required.</span></span> | Bearer {токен}. Обязательный. |


## <span data-ttu-id="b3bdc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3bdc-128">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="b3bdc-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3bdc-129">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="b3bdc-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3bdc-130">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="b3bdc-131">В случае успеха этот метод возвратит код отклика `200 OK` и объект [driveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b3bdc-131">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <span data-ttu-id="b3bdc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b3bdc-132">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="b3bdc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3bdc-133">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="b3bdc-134">Ниже приведен пример запроса на получение списка дисков пользователя.</span><span class="sxs-lookup"><span data-stu-id="b3bdc-134">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <span data-ttu-id="b3bdc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3bdc-135">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="b3bdc-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3bdc-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <span data-ttu-id="b3bdc-137">Заметки</span><span class="sxs-lookup"><span data-stu-id="b3bdc-137">Remarks</span></span>
<a id="remarks" class="xliff"></a>

<span data-ttu-id="b3bdc-138">Чтобы получить список дочерних элементов для специальной папки, можно запросить коллекцию `children` или с помощью параметра [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) развернуть этот список.</span><span class="sxs-lookup"><span data-stu-id="b3bdc-138">To request the children of a special folder, you can request the `children` collection or use the [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) option to expand the children collection.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
