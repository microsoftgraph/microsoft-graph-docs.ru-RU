---
title: Тип ресурса provisionedPlan
description: Свойство **provisionedPlans** объектов user и organization представляет собой коллекцию объектов **provisionedPlan**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 78ce5deac88c07a5f180c972d80a7c8e8798cab8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521350"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="5dacf-103">Тип ресурса provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="5dacf-103">provisionedPlan resource type</span></span>

<span data-ttu-id="5dacf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5dacf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dacf-105">Свойство **provisionedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="5dacf-105">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="5dacf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5dacf-106">Properties</span></span>
| <span data-ttu-id="5dacf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5dacf-107">Property</span></span>     | <span data-ttu-id="5dacf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5dacf-108">Type</span></span>   |<span data-ttu-id="5dacf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5dacf-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dacf-110">капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="5dacf-110">capabilityStatus</span></span>|<span data-ttu-id="5dacf-111">String</span><span class="sxs-lookup"><span data-stu-id="5dacf-111">String</span></span>|<span data-ttu-id="5dacf-112">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="5dacf-112">For example, “Enabled”.</span></span>|
|<span data-ttu-id="5dacf-113">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="5dacf-113">provisioningStatus</span></span>|<span data-ttu-id="5dacf-114">String</span><span class="sxs-lookup"><span data-stu-id="5dacf-114">String</span></span>|<span data-ttu-id="5dacf-115">Пример: "Success".</span><span class="sxs-lookup"><span data-stu-id="5dacf-115">For example, “Success”.</span></span>|
|<span data-ttu-id="5dacf-116">service</span><span class="sxs-lookup"><span data-stu-id="5dacf-116">service</span></span>|<span data-ttu-id="5dacf-117">String</span><span class="sxs-lookup"><span data-stu-id="5dacf-117">String</span></span>|<span data-ttu-id="5dacf-118">Имя службы, например “AccessControlS2S”.</span><span class="sxs-lookup"><span data-stu-id="5dacf-118">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5dacf-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5dacf-119">JSON representation</span></span>

<span data-ttu-id="5dacf-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5dacf-120">Here is a JSON representation of the resource</span></span>

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
