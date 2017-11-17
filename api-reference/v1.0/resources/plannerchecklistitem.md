<span data-ttu-id="fd05c-p104">Используется для указания относительного порядка элементов в списке. Используемый формат описан [здесь](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="fd05c-p104">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|Используется для указания относительного порядка элементов в списке. Используемый формат описан [здесь](planner_order_hint_format.md).|
|<span data-ttu-id="fd05c-125">title</span><span class="sxs-lookup"><span data-stu-id="fd05c-125">title</span></span>|<span data-ttu-id="fd05c-126">Строка</span><span class="sxs-lookup"><span data-stu-id="fd05c-126">String</span></span>|<span data-ttu-id="fd05c-127">Название элемента списка</span><span class="sxs-lookup"><span data-stu-id="fd05c-127">Title of the checklist item</span></span>|

## <span data-ttu-id="fd05c-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fd05c-128">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="fd05c-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd05c-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->