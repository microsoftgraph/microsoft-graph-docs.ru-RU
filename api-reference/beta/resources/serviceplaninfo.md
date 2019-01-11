---
title: Тип ресурса servicePlanInfo
description: Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта subscribedSku представляет собой коллекцию объектов **servicePlanInfo**.
localization_priority: Normal
ms.openlocfilehash: f0cb96a11b280fcda4e97a6dad30a9e5200c2e88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842681"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="ad1a3-104">Тип ресурса servicePlanInfo</span><span class="sxs-lookup"><span data-stu-id="ad1a3-104">servicePlanInfo resource type</span></span>

> <span data-ttu-id="ad1a3-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad1a3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad1a3-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad1a3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad1a3-p103">Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта [subscribedSku](subscribedsku.md) представляет собой коллекцию объектов **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="ad1a3-p103">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="ad1a3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad1a3-109">Properties</span></span>
| <span data-ttu-id="ad1a3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad1a3-110">Property</span></span>     | <span data-ttu-id="ad1a3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ad1a3-111">Type</span></span>   |<span data-ttu-id="ad1a3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ad1a3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad1a3-113">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="ad1a3-113">servicePlanId</span></span>|<span data-ttu-id="ad1a3-114">Guid</span><span class="sxs-lookup"><span data-stu-id="ad1a3-114">Guid</span></span>|<span data-ttu-id="ad1a3-115">Уникальный идентификатор плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="ad1a3-115">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="ad1a3-116">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="ad1a3-116">servicePlanName</span></span>|<span data-ttu-id="ad1a3-117">String</span><span class="sxs-lookup"><span data-stu-id="ad1a3-117">String</span></span>|<span data-ttu-id="ad1a3-118">Имя плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="ad1a3-118">The name of the service plan.</span></span>|
|<span data-ttu-id="ad1a3-119">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="ad1a3-119">provisioningStatus</span></span>|<span data-ttu-id="ad1a3-120">String</span><span class="sxs-lookup"><span data-stu-id="ad1a3-120">String</span></span>|<span data-ttu-id="ad1a3-p104">Состояние подготовки плана обслуживания. Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="ad1a3-p104">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="ad1a3-123">"Success" — служба полностью подготовлена.</span><span class="sxs-lookup"><span data-stu-id="ad1a3-123">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="ad1a3-124">"Disabled" — служба отключена.</span><span class="sxs-lookup"><span data-stu-id="ad1a3-124">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="ad1a3-125">"PendingInput" — служба еще не подготовлена, ожидается подтверждение.</span><span class="sxs-lookup"><span data-stu-id="ad1a3-125">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="ad1a3-126">«PendingActivation» - служба подготовки, но требует явные активации администратором (например, план обслуживания Intune_O365).</span><span class="sxs-lookup"><span data-stu-id="ad1a3-126">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan).</span></span><br/><span data-ttu-id="ad1a3-127">"PendingProvisioning" — Майкрософт добавила в продукт новую службу, но она пока не активирована в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ad1a3-127">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="ad1a3-128">appliesTo</span><span class="sxs-lookup"><span data-stu-id="ad1a3-128">appliesTo</span></span>|<span data-ttu-id="ad1a3-129">String</span><span class="sxs-lookup"><span data-stu-id="ad1a3-129">String</span></span>|<span data-ttu-id="ad1a3-p105">Объект, которому может быть назначен план обслуживания. Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="ad1a3-p105">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="ad1a3-132">"User" — план обслуживания можно назначить отдельным пользователям.</span><span class="sxs-lookup"><span data-stu-id="ad1a3-132">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="ad1a3-133">"Company" — план обслуживания можно назначить всему клиенту.</span><span class="sxs-lookup"><span data-stu-id="ad1a3-133">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad1a3-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ad1a3-134">JSON representation</span></span>

<span data-ttu-id="ad1a3-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad1a3-135">Here is a JSON representation of the resource</span></span>

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
