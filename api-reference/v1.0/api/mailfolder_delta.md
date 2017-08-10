<span data-ttu-id="e78a7-p110">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e78a7-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "wellKnownName": "wellKnownName-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="e78a7-158">См. также</span><span class="sxs-lookup"><span data-stu-id="e78a7-158">See also</span></span>

- [<span data-ttu-id="e78a7-159">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="e78a7-159">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="e78a7-160">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="e78a7-160">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->