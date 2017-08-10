<span data-ttu-id="a151e-p142">Цепочки бесед группы. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a151e-p142">The group's conversation threads. Nullable.</span></span>| Цепочки бесед группы. Допускается значение null.|


## <a name="json-representation"></a><span data-ttu-id="a151e-436">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a151e-436">JSON representation</span></span>

<span data-ttu-id="a151e-437">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a151e-437">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "events",
    "extensions",
    "memberOf",
    "members",
    "onenote",
    "owners",
    "photo",
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group"
}-->

```json
{
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "id": "string (identifier)",
  "isSubscribedByMail": true,
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": ["string"],
  "securityEnabled": true,
  "unseenCount": 1024,
  "visibility": "string",
  "acceptedSenders": [ { "@odata.type": "microsoft.graph.directoryObject"} ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "conversations": [ { "@odata.type": "microsoft.graph.conversation" }],
  "createdOnBehalfOf": { "@odata.type": "microsoft.graph.directoryObject" },
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "events": [ { "@odata.type": "microsoft.graph.event" }],
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "members": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "owners": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "rejectedSenders": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "sites": [ { "@odata.type": "microsoft.graph.site" } ],
  "threads": [ { "@odata.type": "microsoft.graph.conversationThread" }]
}

```

## <a name="see-also"></a><span data-ttu-id="a151e-438">См. также</span><span class="sxs-lookup"><span data-stu-id="a151e-438">See also</span></span>

- [<span data-ttu-id="a151e-439">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="a151e-439">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="a151e-440">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="a151e-440">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="a151e-441">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="a151e-441">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
