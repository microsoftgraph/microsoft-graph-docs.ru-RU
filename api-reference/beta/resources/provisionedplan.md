---
title: Тип ресурса provisionedPlan
description: Свойство **provisionedPlans** объектов user и organization представляет собой коллекцию объектов **provisionedPlan**.
ms.openlocfilehash: efaf4dc2916189e2bf6a8078a693059369f7cb2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078394"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="3de6a-103">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="3de6a-103">provisionedPlan resource type</span></span>

> <span data-ttu-id="3de6a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3de6a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3de6a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3de6a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3de6a-106">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="3de6a-106">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="3de6a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3de6a-107">Properties</span></span>
| <span data-ttu-id="3de6a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3de6a-108">Property</span></span>     | <span data-ttu-id="3de6a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3de6a-109">Type</span></span>   |<span data-ttu-id="3de6a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3de6a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3de6a-111">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="3de6a-111">capabilityStatus</span></span>|<span data-ttu-id="3de6a-112">String</span><span class="sxs-lookup"><span data-stu-id="3de6a-112">String</span></span>|<span data-ttu-id="3de6a-113">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="3de6a-113">For example, “Enabled”.</span></span>|
|<span data-ttu-id="3de6a-114">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="3de6a-114">provisioningStatus</span></span>|<span data-ttu-id="3de6a-115">String</span><span class="sxs-lookup"><span data-stu-id="3de6a-115">String</span></span>|<span data-ttu-id="3de6a-116">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="3de6a-116">For example, “Success”.</span></span>|
|<span data-ttu-id="3de6a-117">service</span><span class="sxs-lookup"><span data-stu-id="3de6a-117">service</span></span>|<span data-ttu-id="3de6a-118">String</span><span class="sxs-lookup"><span data-stu-id="3de6a-118">String</span></span>|<span data-ttu-id="3de6a-119">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="3de6a-119">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3de6a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3de6a-120">JSON representation</span></span>

<span data-ttu-id="3de6a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3de6a-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedplan"
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