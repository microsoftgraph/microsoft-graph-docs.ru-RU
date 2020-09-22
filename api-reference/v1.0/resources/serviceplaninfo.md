---
title: Тип ресурса servicePlanInfo
description: Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта subscribedSku представляет собой коллекцию объектов **servicePlanInfo**.
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6176174a046618176627e8bbe7b8a984c58a3c22
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991861"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="dbab7-104">Тип ресурса servicePlanInfo</span><span class="sxs-lookup"><span data-stu-id="dbab7-104">servicePlanInfo resource type</span></span>

<span data-ttu-id="dbab7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbab7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dbab7-106">Содержит сведения о плане обслуживания, связанном с подписанным SKU.</span><span class="sxs-lookup"><span data-stu-id="dbab7-106">Contains information about a service plan associated with a subscribed SKU.</span></span> <span data-ttu-id="dbab7-107">Свойство **servicePlans** объекта [subscribedSku](subscribedsku.md) представляет собой коллекцию объектов **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="dbab7-107">The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="dbab7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbab7-108">Properties</span></span>
| <span data-ttu-id="dbab7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbab7-109">Property</span></span>     | <span data-ttu-id="dbab7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dbab7-110">Type</span></span>   |<span data-ttu-id="dbab7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dbab7-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbab7-112">сервицепланид</span><span class="sxs-lookup"><span data-stu-id="dbab7-112">servicePlanId</span></span>|<span data-ttu-id="dbab7-113">Guid</span><span class="sxs-lookup"><span data-stu-id="dbab7-113">Guid</span></span>|<span data-ttu-id="dbab7-114">Уникальный идентификатор плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="dbab7-114">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="dbab7-115">сервицепланнаме</span><span class="sxs-lookup"><span data-stu-id="dbab7-115">servicePlanName</span></span>|<span data-ttu-id="dbab7-116">String</span><span class="sxs-lookup"><span data-stu-id="dbab7-116">String</span></span>|<span data-ttu-id="dbab7-117">Имя плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="dbab7-117">The name of the service plan.</span></span>|
|<span data-ttu-id="dbab7-118">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="dbab7-118">provisioningStatus</span></span>|<span data-ttu-id="dbab7-119">String</span><span class="sxs-lookup"><span data-stu-id="dbab7-119">String</span></span>|<span data-ttu-id="dbab7-120">Состояние подготовки плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="dbab7-120">The provisioning status of the service plan.</span></span> <span data-ttu-id="dbab7-121">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="dbab7-121">Possible values:</span></span><br/><span data-ttu-id="dbab7-122">"Success" — служба полностью подготовлена.</span><span class="sxs-lookup"><span data-stu-id="dbab7-122">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="dbab7-123">"Disabled" — служба отключена.</span><span class="sxs-lookup"><span data-stu-id="dbab7-123">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="dbab7-124">"PendingInput" — служба еще не подготовлена; ожидается подтверждение службы.</span><span class="sxs-lookup"><span data-stu-id="dbab7-124">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="dbab7-125">"Пендингактиватион" — служба подготовлена, но требует явной активации администратором (например, Intune_O365 план обслуживания).</span><span class="sxs-lookup"><span data-stu-id="dbab7-125">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="dbab7-126">"Пендингпровисионинг" — Корпорация Майкрософт добавила новую службу в SKU продукта и еще не активировалась в клиенте.</span><span class="sxs-lookup"><span data-stu-id="dbab7-126">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="dbab7-127">Тег</span><span class="sxs-lookup"><span data-stu-id="dbab7-127">appliesTo</span></span>|<span data-ttu-id="dbab7-128">String</span><span class="sxs-lookup"><span data-stu-id="dbab7-128">String</span></span>|<span data-ttu-id="dbab7-129">Объект, которому можно назначить план обслуживания.</span><span class="sxs-lookup"><span data-stu-id="dbab7-129">The object the service plan can be assigned to.</span></span> <span data-ttu-id="dbab7-130">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="dbab7-130">Possible values:</span></span><br/><span data-ttu-id="dbab7-131">"User" — план обслуживания можно назначить отдельным пользователям.</span><span class="sxs-lookup"><span data-stu-id="dbab7-131">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="dbab7-132">"Company" — план обслуживания можно назначить всему клиенту.</span><span class="sxs-lookup"><span data-stu-id="dbab7-132">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbab7-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dbab7-133">JSON representation</span></span>

<span data-ttu-id="dbab7-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbab7-134">Here is a JSON representation of the resource</span></span>

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

