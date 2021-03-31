---
title: Тип ресурса provisionedPlan
description: Свойство **provisionedPlans** объектов user и organization представляет собой коллекцию объектов **provisionedPlan**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: 1fed61db1de92ba330d233725774e4978abe72ff
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469439"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="0505d-103">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="0505d-103">provisionedPlan resource type</span></span>

<span data-ttu-id="0505d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0505d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0505d-105">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="0505d-105">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="0505d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0505d-106">Properties</span></span>
| <span data-ttu-id="0505d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0505d-107">Property</span></span>     | <span data-ttu-id="0505d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0505d-108">Type</span></span>   |<span data-ttu-id="0505d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0505d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0505d-110">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="0505d-110">capabilityStatus</span></span>|<span data-ttu-id="0505d-111">String</span><span class="sxs-lookup"><span data-stu-id="0505d-111">String</span></span>|<span data-ttu-id="0505d-112">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="0505d-112">For example, “Enabled”.</span></span>|
|<span data-ttu-id="0505d-113">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="0505d-113">provisioningStatus</span></span>|<span data-ttu-id="0505d-114">String</span><span class="sxs-lookup"><span data-stu-id="0505d-114">String</span></span>|<span data-ttu-id="0505d-115">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="0505d-115">For example, “Success”.</span></span>|
|<span data-ttu-id="0505d-116">service</span><span class="sxs-lookup"><span data-stu-id="0505d-116">service</span></span>|<span data-ttu-id="0505d-117">String</span><span class="sxs-lookup"><span data-stu-id="0505d-117">String</span></span>|<span data-ttu-id="0505d-118">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="0505d-118">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0505d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0505d-119">JSON representation</span></span>

<span data-ttu-id="0505d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0505d-120">Here is a JSON representation of the resource</span></span>

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


