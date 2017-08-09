<span data-ttu-id="c3d13-p107">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.  Разрешено вносить изменения только в виде дополнений.</span><span class="sxs-lookup"><span data-stu-id="c3d13-p107">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.  Разрешено вносить изменения только в виде дополнений.|

## <a name="response"></a><span data-ttu-id="c3d13-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3d13-142">Response</span></span>

<span data-ttu-id="c3d13-143">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c3d13-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c3d13-144">Пример</span><span class="sxs-lookup"><span data-stu-id="c3d13-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c3d13-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3d13-145">Request</span></span>

<span data-ttu-id="c3d13-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3d13-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <a name="response"></a><span data-ttu-id="c3d13-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3d13-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="c3d13-148">См. также</span><span class="sxs-lookup"><span data-stu-id="c3d13-148">See also</span></span>

- [<span data-ttu-id="c3d13-149">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="c3d13-149">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="c3d13-150">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="c3d13-150">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->