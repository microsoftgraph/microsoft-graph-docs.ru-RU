# <a name="provisionedplan-resource-type"></a><span data-ttu-id="280e3-101">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="280e3-101">provisionedPlan resource type</span></span>

<span data-ttu-id="280e3-102">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="280e3-102">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="280e3-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="280e3-103">Properties</span></span>
| <span data-ttu-id="280e3-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="280e3-104">Property</span></span>     | <span data-ttu-id="280e3-105">Тип</span><span class="sxs-lookup"><span data-stu-id="280e3-105">Type</span></span>   |<span data-ttu-id="280e3-106">Описание</span><span class="sxs-lookup"><span data-stu-id="280e3-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="280e3-107">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="280e3-107">capabilityStatus</span></span>|<span data-ttu-id="280e3-108">String</span><span class="sxs-lookup"><span data-stu-id="280e3-108">String</span></span>|<span data-ttu-id="280e3-109">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="280e3-109">For example, “Enabled”.</span></span>|
|<span data-ttu-id="280e3-110">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="280e3-110">provisioningStatus</span></span>|<span data-ttu-id="280e3-111">String</span><span class="sxs-lookup"><span data-stu-id="280e3-111">String</span></span>|<span data-ttu-id="280e3-112">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="280e3-112">For example, “Success”.</span></span>|
|<span data-ttu-id="280e3-113">service</span><span class="sxs-lookup"><span data-stu-id="280e3-113">service</span></span>|<span data-ttu-id="280e3-114">String</span><span class="sxs-lookup"><span data-stu-id="280e3-114">String</span></span>|<span data-ttu-id="280e3-115">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="280e3-115">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="280e3-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="280e3-116">JSON representation</span></span>

<span data-ttu-id="280e3-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="280e3-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedplan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->