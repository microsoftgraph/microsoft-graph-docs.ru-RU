---
title: Тип ресурса provisionedPlan
description: Свойство **provisionedPlans** объектов user и organization представляет собой коллекцию объектов **provisionedPlan**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: davidmu1
ms.openlocfilehash: bfb7ace1f42886a5c1335480ebb9de45b333793b
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810540"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="1dd40-103">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="1dd40-103">provisionedPlan resource type</span></span>

<span data-ttu-id="1dd40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dd40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dd40-105">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="1dd40-105">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="1dd40-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1dd40-106">Properties</span></span>
| <span data-ttu-id="1dd40-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1dd40-107">Property</span></span>     | <span data-ttu-id="1dd40-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1dd40-108">Type</span></span>   |<span data-ttu-id="1dd40-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1dd40-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dd40-110">капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="1dd40-110">capabilityStatus</span></span>|<span data-ttu-id="1dd40-111">String</span><span class="sxs-lookup"><span data-stu-id="1dd40-111">String</span></span>|<span data-ttu-id="1dd40-112">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="1dd40-112">For example, “Enabled”.</span></span>|
|<span data-ttu-id="1dd40-113">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="1dd40-113">provisioningStatus</span></span>|<span data-ttu-id="1dd40-114">String</span><span class="sxs-lookup"><span data-stu-id="1dd40-114">String</span></span>|<span data-ttu-id="1dd40-115">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="1dd40-115">For example, “Success”.</span></span>|
|<span data-ttu-id="1dd40-116">service</span><span class="sxs-lookup"><span data-stu-id="1dd40-116">service</span></span>|<span data-ttu-id="1dd40-117">String</span><span class="sxs-lookup"><span data-stu-id="1dd40-117">String</span></span>|<span data-ttu-id="1dd40-118">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="1dd40-118">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1dd40-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1dd40-119">JSON representation</span></span>

<span data-ttu-id="1dd40-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1dd40-120">Here is a JSON representation of the resource</span></span>

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
