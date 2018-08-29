# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="5e8a4-101">Тип ресурса plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="5e8a4-101">plannerOrderHintsByAssignee resource type</span></span>

<span data-ttu-id="5e8a4-p101">**plannerOrderHintsByAssignee** — это ресурс, который содержит [указания в отношении порядка](planner_order_hint_format.md) расположения исполнителей задачи [plannerTask](plannerTask.md) в представлении "Кому назначено" на доске задач. Это открытый тип. Свойства — это идентификаторы исполнителей, а значения — указания в отношении порядка расположения.</span><span class="sxs-lookup"><span data-stu-id="5e8a4-p101">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner_order_hint_format.md) for assignees in a [plannerTask](plannerTask.md) resource, to indicate the order of the task in Assigned To view of the Task Board. This type is an open type. The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="5e8a4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e8a4-105">Properties</span></span>
<span data-ttu-id="5e8a4-p102">Свойства открытого типа может задавать клиент. Он должен указать идентификаторы исполнителей как имена свойств, а допустимое [указание в отношении порядка расположения](planner_order_hint_format.md) как значение. Свойства этого типа невозможно удалить. Служба будет автоматически удалять значения после обновления заданий в содержащем их объекте [plannerTask](plannerTask.md).</span><span class="sxs-lookup"><span data-stu-id="5e8a4-p102">Properties of an Open Type can be defined by the client. In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner_order_hint_format.md) as the value. Properties cannot be removed from this type. The service will automatically remove values as the assignments on the containing [plannerTask](plannerTask.md) are updated.</span></span>

<span data-ttu-id="5e8a4-110">Пример:</span><span class="sxs-lookup"><span data-stu-id="5e8a4-110">Example:</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->