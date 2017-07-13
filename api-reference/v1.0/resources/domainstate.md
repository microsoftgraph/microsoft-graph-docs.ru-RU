<span data-ttu-id="f7cdc-p102">Тип асинхронной операции. Возможные значения: *ForceDelete* или *Verification*.</span><span class="sxs-lookup"><span data-stu-id="f7cdc-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> | Тип асинхронной операции. Возможные значения: *ForceDelete* или *Verification*. |
| <span data-ttu-id="f7cdc-115">status</span><span class="sxs-lookup"><span data-stu-id="f7cdc-115">status</span></span> | <span data-ttu-id="f7cdc-116">String</span><span class="sxs-lookup"><span data-stu-id="f7cdc-116">String</span></span> | <span data-ttu-id="f7cdc-117">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="f7cdc-117">Current status of the operation.</span></span> <br> <span data-ttu-id="f7cdc-118">*Scheduled* — операция запланирована, но еще не запущена.</span><span class="sxs-lookup"><span data-stu-id="f7cdc-118">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="f7cdc-119">*InProgress* — операция запущена и в настоящее время выполняется.</span><span class="sxs-lookup"><span data-stu-id="f7cdc-119">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="f7cdc-120">*Failed* — не удалось выполнить операцию.</span><span class="sxs-lookup"><span data-stu-id="f7cdc-120">*Failed* - Operation has failed.</span></span> |

## <span data-ttu-id="f7cdc-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f7cdc-121">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="f7cdc-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7cdc-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->