<span data-ttu-id="032cf-p104">Значение указания, используемое для упорядочения задач в представлении AssignedTo доски задач, когда задача не назначена ни одному пользователю либо когда в словаре orderHintsByAssignee нет указания порядка для пользователя, которому назначена задача. Используемый формат описан [здесь](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="032cf-p104">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|Значение указания, используемое для упорядочения задач в представлении AssignedTo доски задач, когда задача не назначена ни одному пользователю либо когда в словаре orderHintsByAssignee нет указания порядка для пользователя, которому назначена задача. Используемый формат описан [здесь](planner_order_hint_format.md).|

## <span data-ttu-id="032cf-133">Связи</span><span class="sxs-lookup"><span data-stu-id="032cf-133">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="032cf-134">Нет</span><span class="sxs-lookup"><span data-stu-id="032cf-134">None</span></span>


## <span data-ttu-id="032cf-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="032cf-135">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="032cf-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="032cf-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->