---
title: Тип ресурса provisionedPlan
description: Свойство **provisionedPlans** объектов user и organization представляет собой коллекцию объектов **provisionedPlan**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: davidmu1
ms.openlocfilehash: da1ecc796c3978195ee974eda4290c7cf9b37f2e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026504"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="f064d-103">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="f064d-103">provisionedPlan resource type</span></span>

<span data-ttu-id="f064d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f064d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f064d-105">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="f064d-105">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="f064d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f064d-106">Properties</span></span>
| <span data-ttu-id="f064d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f064d-107">Property</span></span>     | <span data-ttu-id="f064d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f064d-108">Type</span></span>   |<span data-ttu-id="f064d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f064d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f064d-110">капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="f064d-110">capabilityStatus</span></span>|<span data-ttu-id="f064d-111">String</span><span class="sxs-lookup"><span data-stu-id="f064d-111">String</span></span>|<span data-ttu-id="f064d-112">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="f064d-112">For example, “Enabled”.</span></span>|
|<span data-ttu-id="f064d-113">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="f064d-113">provisioningStatus</span></span>|<span data-ttu-id="f064d-114">String</span><span class="sxs-lookup"><span data-stu-id="f064d-114">String</span></span>|<span data-ttu-id="f064d-115">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="f064d-115">For example, “Success”.</span></span>|
|<span data-ttu-id="f064d-116">service</span><span class="sxs-lookup"><span data-stu-id="f064d-116">service</span></span>|<span data-ttu-id="f064d-117">String</span><span class="sxs-lookup"><span data-stu-id="f064d-117">String</span></span>|<span data-ttu-id="f064d-118">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="f064d-118">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f064d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f064d-119">JSON representation</span></span>

<span data-ttu-id="f064d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f064d-120">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


