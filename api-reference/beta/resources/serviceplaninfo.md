---
title: Тип ресурса servicePlanInfo
description: Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта **subscribedSku** представляет собой коллекцию объектов servicePlanInfo.
localization_priority: Normal
ms.openlocfilehash: e759082984cc66f7d3efec3cbb7cbee11561f253
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512607"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="4b23a-104">Тип ресурса servicePlanInfo</span><span class="sxs-lookup"><span data-stu-id="4b23a-104">servicePlanInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b23a-p102">Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта [subscribedSku](subscribedsku.md) представляет собой коллекцию объектов **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="4b23a-p102">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="4b23a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b23a-107">Properties</span></span>
| <span data-ttu-id="4b23a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b23a-108">Property</span></span>     | <span data-ttu-id="4b23a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4b23a-109">Type</span></span>   |<span data-ttu-id="4b23a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4b23a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b23a-111">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="4b23a-111">servicePlanId</span></span>|<span data-ttu-id="4b23a-112">Guid</span><span class="sxs-lookup"><span data-stu-id="4b23a-112">Guid</span></span>|<span data-ttu-id="4b23a-113">Уникальный идентификатор плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="4b23a-113">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="4b23a-114">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="4b23a-114">servicePlanName</span></span>|<span data-ttu-id="4b23a-115">String</span><span class="sxs-lookup"><span data-stu-id="4b23a-115">String</span></span>|<span data-ttu-id="4b23a-116">Имя плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="4b23a-116">The name of the service plan.</span></span>|
|<span data-ttu-id="4b23a-117">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="4b23a-117">provisioningStatus</span></span>|<span data-ttu-id="4b23a-118">String</span><span class="sxs-lookup"><span data-stu-id="4b23a-118">String</span></span>|<span data-ttu-id="4b23a-p103">Состояние подготовки плана обслуживания. Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="4b23a-p103">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="4b23a-121">"Success" — служба полностью подготовлена.</span><span class="sxs-lookup"><span data-stu-id="4b23a-121">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="4b23a-122">"Disabled" — служба отключена.</span><span class="sxs-lookup"><span data-stu-id="4b23a-122">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="4b23a-123">"PendingInput" — служба еще не подготовлена, ожидается подтверждение.</span><span class="sxs-lookup"><span data-stu-id="4b23a-123">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="4b23a-124">«PendingActivation» - служба подготовки, но требует явные активации администратором (например, план обслуживания Intune_O365).</span><span class="sxs-lookup"><span data-stu-id="4b23a-124">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan).</span></span><br/><span data-ttu-id="4b23a-125">"PendingProvisioning" — Майкрософт добавила в продукт новую службу, но она пока не активирована в клиенте.</span><span class="sxs-lookup"><span data-stu-id="4b23a-125">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="4b23a-126">appliesTo</span><span class="sxs-lookup"><span data-stu-id="4b23a-126">appliesTo</span></span>|<span data-ttu-id="4b23a-127">String</span><span class="sxs-lookup"><span data-stu-id="4b23a-127">String</span></span>|<span data-ttu-id="4b23a-p104">Объект, которому может быть назначен план обслуживания. Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="4b23a-p104">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="4b23a-130">"User" — план обслуживания можно назначить отдельным пользователям.</span><span class="sxs-lookup"><span data-stu-id="4b23a-130">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="4b23a-131">"Company" — план обслуживания можно назначить всему клиенту.</span><span class="sxs-lookup"><span data-stu-id="4b23a-131">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b23a-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4b23a-132">JSON representation</span></span>

<span data-ttu-id="4b23a-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b23a-133">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/serviceplaninfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
