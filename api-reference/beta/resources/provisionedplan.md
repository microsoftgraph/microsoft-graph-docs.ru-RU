---
title: Тип ресурса provisionedPlan
description: Свойство **provisionedPlans** объектов user и organization представляет собой коллекцию объектов **provisionedPlan**.
localization_priority: Normal
ms.openlocfilehash: 5f9d9c5b2dfffb86643c5e355799f46382bc38cd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563355"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="0b470-103">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="0b470-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b470-104">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="0b470-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="0b470-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b470-105">Properties</span></span>
| <span data-ttu-id="0b470-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b470-106">Property</span></span>     | <span data-ttu-id="0b470-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0b470-107">Type</span></span>   |<span data-ttu-id="0b470-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0b470-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b470-109">Капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="0b470-109">capabilityStatus</span></span>|<span data-ttu-id="0b470-110">String</span><span class="sxs-lookup"><span data-stu-id="0b470-110">String</span></span>|<span data-ttu-id="0b470-111">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="0b470-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="0b470-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="0b470-112">provisioningStatus</span></span>|<span data-ttu-id="0b470-113">String</span><span class="sxs-lookup"><span data-stu-id="0b470-113">String</span></span>|<span data-ttu-id="0b470-114">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="0b470-114">For example, “Success”.</span></span>|
|<span data-ttu-id="0b470-115">service</span><span class="sxs-lookup"><span data-stu-id="0b470-115">service</span></span>|<span data-ttu-id="0b470-116">String</span><span class="sxs-lookup"><span data-stu-id="0b470-116">String</span></span>|<span data-ttu-id="0b470-117">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="0b470-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b470-118">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0b470-118">JSON representation</span></span>

<span data-ttu-id="0b470-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b470-119">Here is a JSON representation of the resource</span></span>

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
