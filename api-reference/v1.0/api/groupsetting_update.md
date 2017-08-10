<span data-ttu-id="533b5-p102">Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений.</span><span class="sxs-lookup"><span data-stu-id="533b5-p102">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> | Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений. |

## <a name="response"></a><span data-ttu-id="533b5-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="533b5-126">Response</span></span>

<span data-ttu-id="533b5-127">В случае успешного выполнения этот метод возвращает код отклика `204 OK` и обновленный объект [groupSetting](../resources/groupsetting.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="533b5-127">If successful, this method returns a `204 OK` response code and [directoryObject](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="533b5-128">Пример</span><span class="sxs-lookup"><span data-stu-id="533b5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="533b5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="533b5-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="533b5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="533b5-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->