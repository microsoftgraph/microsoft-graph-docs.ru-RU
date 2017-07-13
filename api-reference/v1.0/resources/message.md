<span data-ttu-id="7e93a-p122">Коллекция однозначных расширенных свойств, определенных для сообщения. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7e93a-p122">The collection of single-value extended properties defined for the message. Read-only. Nullable.</span></span>| Коллекция однозначных расширенных свойств, определенных для сообщения. Только для чтения. Допускается значение null.|


## <span data-ttu-id="7e93a-330">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e93a-330">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="7e93a-331">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e93a-331">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "parentFolderId": "string",
  "receivedDateTime": "String (timestamp)",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```

## <span data-ttu-id="7e93a-332">См. также</span><span class="sxs-lookup"><span data-stu-id="7e93a-332">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="7e93a-333">Получение параметров почтового ящика</span><span class="sxs-lookup"><span data-stu-id="7e93a-333">Get mailbox settings</span></span>](../api/user_get_mailboxsettings.md) 
- [<span data-ttu-id="7e93a-334">Обновление параметров почтового ящика</span><span class="sxs-lookup"><span data-stu-id="7e93a-334">Update mailbox settings</span></span>](../api/user_update_mailboxsettings.md)
- [<span data-ttu-id="7e93a-335">Отслеживание изменений данных Microsoft Graph с помощью запроса изменений</span><span class="sxs-lookup"><span data-stu-id="7e93a-335">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="7e93a-336">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="7e93a-336">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)
- [<span data-ttu-id="7e93a-337">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="7e93a-337">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="7e93a-338">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="7e93a-338">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="7e93a-339">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="7e93a-339">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
