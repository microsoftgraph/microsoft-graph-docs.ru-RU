<span data-ttu-id="067b1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="067b1-p103">Bearer {token}. Required.</span></span> | Bearer {токен}. Обязательный. |


## <a name="request-body"></a><span data-ttu-id="067b1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="067b1-128">Request body</span></span>
<span data-ttu-id="067b1-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="067b1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="067b1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="067b1-130">Response</span></span>

<span data-ttu-id="067b1-131">В случае успеха этот метод возвратит код отклика `200 OK` и объект [driveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="067b1-131">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="067b1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="067b1-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="067b1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="067b1-133">Request</span></span>
<span data-ttu-id="067b1-134">Ниже приведен пример запроса на получение списка дисков пользователя.</span><span class="sxs-lookup"><span data-stu-id="067b1-134">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a><span data-ttu-id="067b1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="067b1-135">Response</span></span>
<span data-ttu-id="067b1-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="067b1-136">Here is an example of the response.</span></span>
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

## <a name="remarks"></a><span data-ttu-id="067b1-137">Заметки</span><span class="sxs-lookup"><span data-stu-id="067b1-137">Remarks</span></span>

<span data-ttu-id="067b1-138">Чтобы получить список дочерних элементов для специальной папки, можно запросить коллекцию `children` или с помощью параметра [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) развернуть этот список.</span><span class="sxs-lookup"><span data-stu-id="067b1-138">To request the children of a special folder, you can request the `children` collection or use the [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) option to expand the children collection.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
