---
title: Тип ресурса provisionedPlan
description: Свойство **provisionedPlans** объектов **user** и organization представляет собой коллекцию объектов provisionedPlan.
localization_priority: Normal
ms.openlocfilehash: 5f9d9c5b2dfffb86643c5e355799f46382bc38cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527817"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="26d65-103">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="26d65-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26d65-104">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="26d65-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="26d65-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="26d65-105">Properties</span></span>
| <span data-ttu-id="26d65-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="26d65-106">Property</span></span>     | <span data-ttu-id="26d65-107">Тип</span><span class="sxs-lookup"><span data-stu-id="26d65-107">Type</span></span>   |<span data-ttu-id="26d65-108">Описание</span><span class="sxs-lookup"><span data-stu-id="26d65-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26d65-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="26d65-109">capabilityStatus</span></span>|<span data-ttu-id="26d65-110">Строка</span><span class="sxs-lookup"><span data-stu-id="26d65-110">String</span></span>|<span data-ttu-id="26d65-111">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="26d65-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="26d65-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="26d65-112">provisioningStatus</span></span>|<span data-ttu-id="26d65-113">String</span><span class="sxs-lookup"><span data-stu-id="26d65-113">String</span></span>|<span data-ttu-id="26d65-114">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="26d65-114">For example, “Success”.</span></span>|
|<span data-ttu-id="26d65-115">service</span><span class="sxs-lookup"><span data-stu-id="26d65-115">service</span></span>|<span data-ttu-id="26d65-116">String</span><span class="sxs-lookup"><span data-stu-id="26d65-116">String</span></span>|<span data-ttu-id="26d65-117">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="26d65-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26d65-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26d65-118">JSON representation</span></span>

<span data-ttu-id="26d65-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26d65-119">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/provisionedplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
