---
title: Тип ресурса servicePlanInfo
description: Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта subscribedSku представляет собой коллекцию объектов **servicePlanInfo**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: krbain
ms.openlocfilehash: f79e943f0303d28542f3f0932b1e59e59c481fc5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133618"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="50331-104">Тип ресурса servicePlanInfo</span><span class="sxs-lookup"><span data-stu-id="50331-104">servicePlanInfo resource type</span></span>

<span data-ttu-id="50331-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50331-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50331-106">Содержит сведения о плане обслуживания, связанном с подписанным SKU.</span><span class="sxs-lookup"><span data-stu-id="50331-106">Contains information about a service plan associated with a subscribed SKU.</span></span> <span data-ttu-id="50331-107">Свойство **servicePlans** объекта [subscribedSku](subscribedsku.md) представляет собой коллекцию объектов **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="50331-107">The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="50331-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="50331-108">Properties</span></span>
| <span data-ttu-id="50331-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="50331-109">Property</span></span>     | <span data-ttu-id="50331-110">Тип</span><span class="sxs-lookup"><span data-stu-id="50331-110">Type</span></span>   |<span data-ttu-id="50331-111">Описание</span><span class="sxs-lookup"><span data-stu-id="50331-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50331-112">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="50331-112">servicePlanId</span></span>|<span data-ttu-id="50331-113">Guid</span><span class="sxs-lookup"><span data-stu-id="50331-113">Guid</span></span>|<span data-ttu-id="50331-114">Уникальный идентификатор плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="50331-114">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="50331-115">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="50331-115">servicePlanName</span></span>|<span data-ttu-id="50331-116">String</span><span class="sxs-lookup"><span data-stu-id="50331-116">String</span></span>|<span data-ttu-id="50331-117">Имя плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="50331-117">The name of the service plan.</span></span>|
|<span data-ttu-id="50331-118">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="50331-118">provisioningStatus</span></span>|<span data-ttu-id="50331-119">String</span><span class="sxs-lookup"><span data-stu-id="50331-119">String</span></span>|<span data-ttu-id="50331-120">Состояние подготовки плана обслуживания.</span><span class="sxs-lookup"><span data-stu-id="50331-120">The provisioning status of the service plan.</span></span> <span data-ttu-id="50331-121">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="50331-121">Possible values:</span></span><br/><span data-ttu-id="50331-122">"Успешно" — служба полностью завершена.</span><span class="sxs-lookup"><span data-stu-id="50331-122">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="50331-123">"Отключено" — служба отключена.</span><span class="sxs-lookup"><span data-stu-id="50331-123">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="50331-124">"PendingInput" — служба еще не завершена; ожидает подтверждения службы.</span><span class="sxs-lookup"><span data-stu-id="50331-124">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="50331-125">"PendingActivation" — служба уже предусмотрена, но требует явной активации администратором (например, Intune_O365 службы).</span><span class="sxs-lookup"><span data-stu-id="50331-125">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan).</span></span><br/><span data-ttu-id="50331-126">"PendingProvisioning" — корпорация Майкрософт добавила новую службу в SKU продукта и еще не была активирована в клиенте.</span><span class="sxs-lookup"><span data-stu-id="50331-126">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="50331-127">appliesTo</span><span class="sxs-lookup"><span data-stu-id="50331-127">appliesTo</span></span>|<span data-ttu-id="50331-128">String</span><span class="sxs-lookup"><span data-stu-id="50331-128">String</span></span>|<span data-ttu-id="50331-129">Объект, который может быть назначен плану обслуживания.</span><span class="sxs-lookup"><span data-stu-id="50331-129">The object the service plan can be assigned to.</span></span> <span data-ttu-id="50331-130">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="50331-130">Possible values:</span></span><br/><span data-ttu-id="50331-131">"Пользователь" — план обслуживания может быть назначен отдельным пользователям.</span><span class="sxs-lookup"><span data-stu-id="50331-131">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="50331-132">"Компания" — план обслуживания может быть назначен всему арендатору.</span><span class="sxs-lookup"><span data-stu-id="50331-132">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50331-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="50331-133">JSON representation</span></span>

<span data-ttu-id="50331-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50331-134">Here is a JSON representation of the resource</span></span>

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


