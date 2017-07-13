<span data-ttu-id="9d57f-p107">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.  Разрешено вносить изменения только в виде дополнений.</span><span class="sxs-lookup"><span data-stu-id="9d57f-p107">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.  Разрешено вносить изменения только в виде дополнений.|

## <span data-ttu-id="9d57f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d57f-142">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="9d57f-143">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9d57f-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <span data-ttu-id="9d57f-144">Пример</span><span class="sxs-lookup"><span data-stu-id="9d57f-144">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="9d57f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d57f-145">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="9d57f-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d57f-146">Here is an example of the request.</span></span>
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

##### <span data-ttu-id="9d57f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d57f-147">Response</span></span>
<a id="response" class="xliff"></a>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <span data-ttu-id="9d57f-148">См. также</span><span class="sxs-lookup"><span data-stu-id="9d57f-148">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="9d57f-149">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="9d57f-149">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="9d57f-150">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="9d57f-150">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->