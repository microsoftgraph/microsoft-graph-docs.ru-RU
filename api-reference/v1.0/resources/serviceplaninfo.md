# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="3df5f-101">Тип ресурса servicePlanInfo</span><span class="sxs-lookup"><span data-stu-id="3df5f-101">servicePlanInfo resource type</span></span>

<span data-ttu-id="3df5f-p101">Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта [subscribedSku](subscribedsku.md) представляет собой коллекцию объектов **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="3df5f-p101">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="3df5f-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="3df5f-104">Properties</span></span>
| <span data-ttu-id="3df5f-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="3df5f-105">Property</span></span>     | <span data-ttu-id="3df5f-106">Тип</span><span class="sxs-lookup"><span data-stu-id="3df5f-106">Type</span></span>   |<span data-ttu-id="3df5f-107">Описание</span><span class="sxs-lookup"><span data-stu-id="3df5f-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3df5f-108">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="3df5f-108">servicePlanId</span></span>|<span data-ttu-id="3df5f-109">Guid</span><span class="sxs-lookup"><span data-stu-id="3df5f-109">Guid</span></span>|<span data-ttu-id="3df5f-110">Уникальный идентификатор плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="3df5f-110">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="3df5f-111">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="3df5f-111">servicePlanName</span></span>|<span data-ttu-id="3df5f-112">String</span><span class="sxs-lookup"><span data-stu-id="3df5f-112">String</span></span>|<span data-ttu-id="3df5f-113">Имя плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="3df5f-113">The name of the service plan.</span></span>|
|<span data-ttu-id="3df5f-114">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="3df5f-114">provisioningStatus</span></span>|<span data-ttu-id="3df5f-115">String</span><span class="sxs-lookup"><span data-stu-id="3df5f-115">String</span></span>|<span data-ttu-id="3df5f-p102">Состояние подготовки плана обслуживания. Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="3df5f-p102">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="3df5f-118">"Success" — служба полностью подготовлена.</span><span class="sxs-lookup"><span data-stu-id="3df5f-118">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="3df5f-119">"Disabled" — служба отключена.</span><span class="sxs-lookup"><span data-stu-id="3df5f-119">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="3df5f-120">"PendingInput" — служба еще не подготовлена, ожидается подтверждение.</span><span class="sxs-lookup"><span data-stu-id="3df5f-120">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="3df5f-121">"PendingActivation" — служба подготовлена, но требует явной активации администратором (например, план обслуживания Intune_O365)</span><span class="sxs-lookup"><span data-stu-id="3df5f-121">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="3df5f-122">"PendingProvisioning" — Майкрософт добавила в продукт новую службу, но она пока не активирована в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3df5f-122">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="3df5f-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="3df5f-123">appliesTo</span></span>|<span data-ttu-id="3df5f-124">String</span><span class="sxs-lookup"><span data-stu-id="3df5f-124">String</span></span>|<span data-ttu-id="3df5f-p103">Объект, которому может быть назначен план обслуживания. Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="3df5f-p103">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="3df5f-127">"User" — план обслуживания можно назначить отдельным пользователям.</span><span class="sxs-lookup"><span data-stu-id="3df5f-127">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="3df5f-128">"Company" — план обслуживания можно назначить всему клиенту.</span><span class="sxs-lookup"><span data-stu-id="3df5f-128">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3df5f-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3df5f-129">JSON representation</span></span>

<span data-ttu-id="3df5f-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3df5f-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
