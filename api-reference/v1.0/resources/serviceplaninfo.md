---
title: Тип ресурса servicePlanInfo
description: Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта subscribedSku представляет собой коллекцию объектов **servicePlanInfo**.
ms.openlocfilehash: 70d49eb22542e9bc22ee28df5bc77b3bf6146b6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026284"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="56c58-104">Тип ресурса servicePlanInfo</span><span class="sxs-lookup"><span data-stu-id="56c58-104">servicePlanInfo resource type</span></span>

<span data-ttu-id="56c58-p102">Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта [subscribedSku](subscribedsku.md) представляет собой коллекцию объектов **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="56c58-p102">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="56c58-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="56c58-107">Properties</span></span>
| <span data-ttu-id="56c58-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="56c58-108">Property</span></span>     | <span data-ttu-id="56c58-109">Тип</span><span class="sxs-lookup"><span data-stu-id="56c58-109">Type</span></span>   |<span data-ttu-id="56c58-110">Описание</span><span class="sxs-lookup"><span data-stu-id="56c58-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56c58-111">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="56c58-111">servicePlanId</span></span>|<span data-ttu-id="56c58-112">Guid</span><span class="sxs-lookup"><span data-stu-id="56c58-112">Guid</span></span>|<span data-ttu-id="56c58-113">Уникальный идентификатор плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="56c58-113">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="56c58-114">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="56c58-114">servicePlanName</span></span>|<span data-ttu-id="56c58-115">String</span><span class="sxs-lookup"><span data-stu-id="56c58-115">String</span></span>|<span data-ttu-id="56c58-116">Имя плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="56c58-116">The name of the service plan.</span></span>|
|<span data-ttu-id="56c58-117">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="56c58-117">provisioningStatus</span></span>|<span data-ttu-id="56c58-118">String</span><span class="sxs-lookup"><span data-stu-id="56c58-118">String</span></span>|<span data-ttu-id="56c58-p103">Состояние подготовки плана обслуживания. Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="56c58-p103">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="56c58-121">"Success" — служба полностью подготовлена.</span><span class="sxs-lookup"><span data-stu-id="56c58-121">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="56c58-122">"Disabled" — служба отключена.</span><span class="sxs-lookup"><span data-stu-id="56c58-122">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="56c58-123">"PendingInput" — служба еще не подготовлена, ожидается подтверждение.</span><span class="sxs-lookup"><span data-stu-id="56c58-123">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="56c58-124">"PendingActivation" — служба подготовлена, но требует явной активации администратором (например, план обслуживания Intune_O365)</span><span class="sxs-lookup"><span data-stu-id="56c58-124">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="56c58-125">"PendingProvisioning" — Майкрософт добавила в продукт новую службу, но она пока не активирована в клиенте.</span><span class="sxs-lookup"><span data-stu-id="56c58-125">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="56c58-126">appliesTo</span><span class="sxs-lookup"><span data-stu-id="56c58-126">appliesTo</span></span>|<span data-ttu-id="56c58-127">String</span><span class="sxs-lookup"><span data-stu-id="56c58-127">String</span></span>|<span data-ttu-id="56c58-p104">Объект, которому может быть назначен план обслуживания. Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="56c58-p104">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="56c58-130">"User" — план обслуживания можно назначить отдельным пользователям.</span><span class="sxs-lookup"><span data-stu-id="56c58-130">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="56c58-131">"Company" — план обслуживания можно назначить всему клиенту.</span><span class="sxs-lookup"><span data-stu-id="56c58-131">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56c58-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="56c58-132">JSON representation</span></span>

<span data-ttu-id="56c58-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56c58-133">Here is a JSON representation of the resource</span></span>

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
