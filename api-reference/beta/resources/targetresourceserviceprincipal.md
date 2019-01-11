---
title: Тип ресурса targetResourceServicePrincipal
description: Указывает ServicePrincipalId для ресурсов, на которые оказывает активности аудита. На основе targetResource ресурсов.
localization_priority: Normal
ms.openlocfilehash: 37bd63851ca9169afb669c710ef4cb2c150ea615
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839601"
---
# <a name="targetresourceserviceprincipal-resource-type"></a><span data-ttu-id="3e8c6-104">Тип ресурса targetResourceServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="3e8c6-104">targetResourceServicePrincipal resource type</span></span>
<span data-ttu-id="3e8c6-105">Указывает ServicePrincipalId для ресурсов, на которые оказывает активности аудита.</span><span class="sxs-lookup"><span data-stu-id="3e8c6-105">Indicates the ServicePrincipalId for the resource that impacted the audit activity.</span></span> <span data-ttu-id="3e8c6-106">На основе [targetResource](targetresource.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3e8c6-106">Derived from the [targetResource](targetresource.md) resource.</span></span>



## <a name="properties"></a><span data-ttu-id="3e8c6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e8c6-107">Properties</span></span>
| <span data-ttu-id="3e8c6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e8c6-108">Property</span></span>     | <span data-ttu-id="3e8c6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3e8c6-109">Type</span></span>   |<span data-ttu-id="3e8c6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3e8c6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e8c6-111">appId</span><span class="sxs-lookup"><span data-stu-id="3e8c6-111">appId</span></span>|<span data-ttu-id="3e8c6-112">String</span><span class="sxs-lookup"><span data-stu-id="3e8c6-112">String</span></span>|<span data-ttu-id="3e8c6-113">Указывает уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="3e8c6-113">Indicates the Unique Id of the application.</span></span> <span data-ttu-id="3e8c6-114">Указатель идентификатор приложения для приложения содержится код.</span><span class="sxs-lookup"><span data-stu-id="3e8c6-114">Refers to App Id for a specfic app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e8c6-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e8c6-115">JSON representation</span></span>

<span data-ttu-id="3e8c6-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e8c6-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceServicePrincipal"
}-->

```json
{
  "appId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
