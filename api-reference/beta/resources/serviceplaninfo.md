---
title: Тип ресурса servicePlanInfo
description: Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта subscribedSku представляет собой коллекцию объектов **servicePlanInfo**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3b74ddbb26e61dd1c97342a61b30a3fff9ee1851
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008483"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="01cc7-104">Тип ресурса servicePlanInfo</span><span class="sxs-lookup"><span data-stu-id="01cc7-104">servicePlanInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01cc7-105">Содержит сведения о плане обслуживания, связанном с подписанным SKU.</span><span class="sxs-lookup"><span data-stu-id="01cc7-105">Contains information about a service plan associated with a subscribed SKU.</span></span> <span data-ttu-id="01cc7-106">Свойство **servicePlans** объекта [subscribedSku](subscribedsku.md) представляет собой коллекцию объектов **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="01cc7-106">The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="01cc7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="01cc7-107">Properties</span></span>
| <span data-ttu-id="01cc7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="01cc7-108">Property</span></span>     | <span data-ttu-id="01cc7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="01cc7-109">Type</span></span>   |<span data-ttu-id="01cc7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="01cc7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01cc7-111">Сервицепланид</span><span class="sxs-lookup"><span data-stu-id="01cc7-111">servicePlanId</span></span>|<span data-ttu-id="01cc7-112">Guid</span><span class="sxs-lookup"><span data-stu-id="01cc7-112">Guid</span></span>|<span data-ttu-id="01cc7-113">Уникальный идентификатор плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="01cc7-113">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="01cc7-114">Сервицепланнаме</span><span class="sxs-lookup"><span data-stu-id="01cc7-114">servicePlanName</span></span>|<span data-ttu-id="01cc7-115">String</span><span class="sxs-lookup"><span data-stu-id="01cc7-115">String</span></span>|<span data-ttu-id="01cc7-116">Имя плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="01cc7-116">The name of the service plan.</span></span>|
|<span data-ttu-id="01cc7-117">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="01cc7-117">provisioningStatus</span></span>|<span data-ttu-id="01cc7-118">String</span><span class="sxs-lookup"><span data-stu-id="01cc7-118">String</span></span>|<span data-ttu-id="01cc7-119">Состояние подготовки плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="01cc7-119">The provisioning status of the service plan.</span></span> <span data-ttu-id="01cc7-120">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="01cc7-120">Possible values:</span></span><br/><span data-ttu-id="01cc7-121">"Success" — служба полностью подготовлена.</span><span class="sxs-lookup"><span data-stu-id="01cc7-121">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="01cc7-122">"Disabled" — служба отключена.</span><span class="sxs-lookup"><span data-stu-id="01cc7-122">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="01cc7-123">"PendingInput" — служба еще не подготовлена; ожидается подтверждение службы.</span><span class="sxs-lookup"><span data-stu-id="01cc7-123">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="01cc7-124">"Пендингактиватион" — служба подготовлена, но требует явной активации администратором (например, Intune_O365 Plan).</span><span class="sxs-lookup"><span data-stu-id="01cc7-124">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan).</span></span><br/><span data-ttu-id="01cc7-125">"Пендингпровисионинг" — Корпорация Майкрософт добавила новую службу в SKU продукта и еще не активировалась в клиенте.</span><span class="sxs-lookup"><span data-stu-id="01cc7-125">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="01cc7-126">Тег</span><span class="sxs-lookup"><span data-stu-id="01cc7-126">appliesTo</span></span>|<span data-ttu-id="01cc7-127">String</span><span class="sxs-lookup"><span data-stu-id="01cc7-127">String</span></span>|<span data-ttu-id="01cc7-128">Объект, которому можно назначить план обслуживания.</span><span class="sxs-lookup"><span data-stu-id="01cc7-128">The object the service plan can be assigned to.</span></span> <span data-ttu-id="01cc7-129">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="01cc7-129">Possible values:</span></span><br/><span data-ttu-id="01cc7-130">"User" — план обслуживания можно назначить отдельным пользователям.</span><span class="sxs-lookup"><span data-stu-id="01cc7-130">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="01cc7-131">"Company" — план обслуживания можно назначить всему клиенту.</span><span class="sxs-lookup"><span data-stu-id="01cc7-131">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01cc7-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01cc7-132">JSON representation</span></span>

<span data-ttu-id="01cc7-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01cc7-133">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
