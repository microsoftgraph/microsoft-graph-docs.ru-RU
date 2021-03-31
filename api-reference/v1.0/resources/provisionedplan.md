---
title: Тип ресурса provisionedPlan
description: Свойство **provisionedPlans** объектов user и organization представляет собой коллекцию объектов **provisionedPlan**.
localization_priority: Normal
author: Jumaodhiss
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6b8236a6948b0941cfe3c6f304a037c8cfc41a7e
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469425"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="d77a3-103">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="d77a3-103">provisionedPlan resource type</span></span>

<span data-ttu-id="d77a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d77a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d77a3-105">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="d77a3-105">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="d77a3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d77a3-106">Properties</span></span>
| <span data-ttu-id="d77a3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d77a3-107">Property</span></span>     | <span data-ttu-id="d77a3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d77a3-108">Type</span></span>   |<span data-ttu-id="d77a3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d77a3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d77a3-110">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="d77a3-110">capabilityStatus</span></span>|<span data-ttu-id="d77a3-111">String</span><span class="sxs-lookup"><span data-stu-id="d77a3-111">String</span></span>|<span data-ttu-id="d77a3-112">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="d77a3-112">For example, “Enabled”.</span></span>|
|<span data-ttu-id="d77a3-113">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="d77a3-113">provisioningStatus</span></span>|<span data-ttu-id="d77a3-114">String</span><span class="sxs-lookup"><span data-stu-id="d77a3-114">String</span></span>|<span data-ttu-id="d77a3-115">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="d77a3-115">For example, “Success”.</span></span>|
|<span data-ttu-id="d77a3-116">service</span><span class="sxs-lookup"><span data-stu-id="d77a3-116">service</span></span>|<span data-ttu-id="d77a3-117">String</span><span class="sxs-lookup"><span data-stu-id="d77a3-117">String</span></span>|<span data-ttu-id="d77a3-118">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="d77a3-118">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d77a3-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d77a3-119">JSON representation</span></span>

<span data-ttu-id="d77a3-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d77a3-120">Here is a JSON representation of the resource</span></span>

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

