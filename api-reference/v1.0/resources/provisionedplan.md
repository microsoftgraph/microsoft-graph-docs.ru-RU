---
title: Тип ресурса provisionedPlan
description: Свойство **provisionedPlans** объектов user и organization представляет собой коллекцию объектов **provisionedPlan**.
localization_priority: Normal
ms.openlocfilehash: dd8d4f5b406a2291a829d7c11d4948bd9a08d453
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579666"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="47808-103">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="47808-103">provisionedPlan resource type</span></span>

<span data-ttu-id="47808-104">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="47808-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="47808-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="47808-105">Properties</span></span>
| <span data-ttu-id="47808-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="47808-106">Property</span></span>     | <span data-ttu-id="47808-107">Тип</span><span class="sxs-lookup"><span data-stu-id="47808-107">Type</span></span>   |<span data-ttu-id="47808-108">Описание</span><span class="sxs-lookup"><span data-stu-id="47808-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47808-109">Капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="47808-109">capabilityStatus</span></span>|<span data-ttu-id="47808-110">String</span><span class="sxs-lookup"><span data-stu-id="47808-110">String</span></span>|<span data-ttu-id="47808-111">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="47808-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="47808-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="47808-112">provisioningStatus</span></span>|<span data-ttu-id="47808-113">String</span><span class="sxs-lookup"><span data-stu-id="47808-113">String</span></span>|<span data-ttu-id="47808-114">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="47808-114">For example, “Success”.</span></span>|
|<span data-ttu-id="47808-115">service</span><span class="sxs-lookup"><span data-stu-id="47808-115">service</span></span>|<span data-ttu-id="47808-116">String</span><span class="sxs-lookup"><span data-stu-id="47808-116">String</span></span>|<span data-ttu-id="47808-117">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="47808-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47808-118">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="47808-118">JSON representation</span></span>

<span data-ttu-id="47808-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47808-119">Here is a JSON representation of the resource</span></span>

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
