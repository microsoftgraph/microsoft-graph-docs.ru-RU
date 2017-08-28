# <a name="assignedplan-resource-type"></a><span data-ttu-id="77ab0-101">Тип ресурса assignedPlan</span><span class="sxs-lookup"><span data-stu-id="77ab0-101">assignedPlan resource type</span></span>

<span data-ttu-id="77ab0-102">Свойство **assignedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="77ab0-102">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="77ab0-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="77ab0-103">Properties</span></span>
| <span data-ttu-id="77ab0-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="77ab0-104">Property</span></span>     | <span data-ttu-id="77ab0-105">Тип</span><span class="sxs-lookup"><span data-stu-id="77ab0-105">Type</span></span>   |<span data-ttu-id="77ab0-106">Описание</span><span class="sxs-lookup"><span data-stu-id="77ab0-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77ab0-107">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="77ab0-107">assignedDateTime</span></span>|<span data-ttu-id="77ab0-108">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77ab0-108">DateTimeOffset</span></span>|<span data-ttu-id="77ab0-p101">Дата и время назначения плана. Пример: 2013-01-02T19:32:30Z. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="77ab0-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="77ab0-112">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="77ab0-112">capabilityStatus</span></span>|<span data-ttu-id="77ab0-113">String</span><span class="sxs-lookup"><span data-stu-id="77ab0-113">String</span></span>|<span data-ttu-id="77ab0-114">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="77ab0-114">For example, “Enabled”.</span></span>|
|<span data-ttu-id="77ab0-115">service</span><span class="sxs-lookup"><span data-stu-id="77ab0-115">service</span></span>|<span data-ttu-id="77ab0-116">String</span><span class="sxs-lookup"><span data-stu-id="77ab0-116">String</span></span>|<span data-ttu-id="77ab0-117">Имя службы, например "Exchange".</span><span class="sxs-lookup"><span data-stu-id="77ab0-117">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="77ab0-118">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="77ab0-118">servicePlanId</span></span>|<span data-ttu-id="77ab0-119">Guid</span><span class="sxs-lookup"><span data-stu-id="77ab0-119">Guid</span></span>|<span data-ttu-id="77ab0-120">Идентификатор GUID, определяющий план обслуживания.</span><span class="sxs-lookup"><span data-stu-id="77ab0-120">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77ab0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77ab0-121">JSON representation</span></span>

<span data-ttu-id="77ab0-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77ab0-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
