---
title: Тип ресурса provisionedPlan
description: Свойство **provisionedPlans** объектов user и organization представляет собой коллекцию объектов **provisionedPlan**.
localization_priority: Normal
author: davidmu1
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: bb91d03665a7f768727450ec06d9dca6ae21bef3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129914"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="a6656-103">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="a6656-103">provisionedPlan resource type</span></span>

<span data-ttu-id="a6656-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6656-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a6656-105">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="a6656-105">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="a6656-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6656-106">Properties</span></span>
| <span data-ttu-id="a6656-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6656-107">Property</span></span>     | <span data-ttu-id="a6656-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a6656-108">Type</span></span>   |<span data-ttu-id="a6656-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a6656-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6656-110">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="a6656-110">capabilityStatus</span></span>|<span data-ttu-id="a6656-111">String</span><span class="sxs-lookup"><span data-stu-id="a6656-111">String</span></span>|<span data-ttu-id="a6656-112">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="a6656-112">For example, “Enabled”.</span></span>|
|<span data-ttu-id="a6656-113">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="a6656-113">provisioningStatus</span></span>|<span data-ttu-id="a6656-114">String</span><span class="sxs-lookup"><span data-stu-id="a6656-114">String</span></span>|<span data-ttu-id="a6656-115">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="a6656-115">For example, “Success”.</span></span>|
|<span data-ttu-id="a6656-116">service</span><span class="sxs-lookup"><span data-stu-id="a6656-116">service</span></span>|<span data-ttu-id="a6656-117">String</span><span class="sxs-lookup"><span data-stu-id="a6656-117">String</span></span>|<span data-ttu-id="a6656-118">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="a6656-118">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6656-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6656-119">JSON representation</span></span>

<span data-ttu-id="a6656-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6656-120">Here is a JSON representation of the resource</span></span>

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

