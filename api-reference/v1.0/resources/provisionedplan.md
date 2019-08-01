---
title: Тип ресурса provisionedPlan
description: Свойство **provisionedPlans** объектов user и organization представляет собой коллекцию объектов **provisionedPlan**.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3560aab132448a0d13c4b4abe2590d4802cdf9f3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034995"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="77f55-103">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="77f55-103">provisionedPlan resource type</span></span>

<span data-ttu-id="77f55-104">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="77f55-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="77f55-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="77f55-105">Properties</span></span>
| <span data-ttu-id="77f55-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="77f55-106">Property</span></span>     | <span data-ttu-id="77f55-107">Тип</span><span class="sxs-lookup"><span data-stu-id="77f55-107">Type</span></span>   |<span data-ttu-id="77f55-108">Описание</span><span class="sxs-lookup"><span data-stu-id="77f55-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77f55-109">Капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="77f55-109">capabilityStatus</span></span>|<span data-ttu-id="77f55-110">String</span><span class="sxs-lookup"><span data-stu-id="77f55-110">String</span></span>|<span data-ttu-id="77f55-111">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="77f55-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="77f55-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="77f55-112">provisioningStatus</span></span>|<span data-ttu-id="77f55-113">String</span><span class="sxs-lookup"><span data-stu-id="77f55-113">String</span></span>|<span data-ttu-id="77f55-114">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="77f55-114">For example, “Success”.</span></span>|
|<span data-ttu-id="77f55-115">service</span><span class="sxs-lookup"><span data-stu-id="77f55-115">service</span></span>|<span data-ttu-id="77f55-116">String</span><span class="sxs-lookup"><span data-stu-id="77f55-116">String</span></span>|<span data-ttu-id="77f55-117">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="77f55-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77f55-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77f55-118">JSON representation</span></span>

<span data-ttu-id="77f55-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77f55-119">Here is a JSON representation of the resource</span></span>

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
