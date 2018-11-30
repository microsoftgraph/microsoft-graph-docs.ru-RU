---
title: Тип ресурса provisionedPlan
description: Свойство **provisionedPlans** объектов user и organization представляет собой коллекцию объектов **provisionedPlan**.
ms.openlocfilehash: 7808e3a17e471123f702381fb52535e53682e276
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027031"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="5df3e-103">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="5df3e-103">provisionedPlan resource type</span></span>

<span data-ttu-id="5df3e-104">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="5df3e-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="5df3e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5df3e-105">Properties</span></span>
| <span data-ttu-id="5df3e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5df3e-106">Property</span></span>     | <span data-ttu-id="5df3e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5df3e-107">Type</span></span>   |<span data-ttu-id="5df3e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5df3e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5df3e-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="5df3e-109">capabilityStatus</span></span>|<span data-ttu-id="5df3e-110">String</span><span class="sxs-lookup"><span data-stu-id="5df3e-110">String</span></span>|<span data-ttu-id="5df3e-111">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="5df3e-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="5df3e-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="5df3e-112">provisioningStatus</span></span>|<span data-ttu-id="5df3e-113">String</span><span class="sxs-lookup"><span data-stu-id="5df3e-113">String</span></span>|<span data-ttu-id="5df3e-114">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="5df3e-114">For example, “Success”.</span></span>|
|<span data-ttu-id="5df3e-115">service</span><span class="sxs-lookup"><span data-stu-id="5df3e-115">service</span></span>|<span data-ttu-id="5df3e-116">String</span><span class="sxs-lookup"><span data-stu-id="5df3e-116">String</span></span>|<span data-ttu-id="5df3e-117">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="5df3e-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5df3e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5df3e-118">JSON representation</span></span>

<span data-ttu-id="5df3e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5df3e-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
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