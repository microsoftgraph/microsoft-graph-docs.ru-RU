<span data-ttu-id="89c53-p103">Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, то для предоставления доступа к плану [группы](group.md) используйте API Групп. Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого.</span><span class="sxs-lookup"><span data-stu-id="89c53-p103">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, то для предоставления доступа к плану [группы](group.md) используйте API Групп. Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого. |

## <span data-ttu-id="89c53-132">Связи</span><span class="sxs-lookup"><span data-stu-id="89c53-132">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="89c53-133">Нет</span><span class="sxs-lookup"><span data-stu-id="89c53-133">None</span></span>


## <span data-ttu-id="89c53-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89c53-134">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="89c53-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89c53-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->