---
title: Тип ресурса targetResourceServicePrincipal
description: Указывает ServicePrincipalId для ресурсов, на которые оказывает активности аудита. На основе targetResource ресурсов.
ms.openlocfilehash: 6d6e19997f4bfead771fc0230207df62dde6c6cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080732"
---
# <a name="targetresourceserviceprincipal-resource-type"></a><span data-ttu-id="97347-104">Тип ресурса targetResourceServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="97347-104">targetResourceServicePrincipal resource type</span></span>
<span data-ttu-id="97347-105">Указывает ServicePrincipalId для ресурсов, на которые оказывает активности аудита.</span><span class="sxs-lookup"><span data-stu-id="97347-105">Indicates the ServicePrincipalId for the resource that impacted the audit activity.</span></span> <span data-ttu-id="97347-106">На основе [targetResource](targetresource.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="97347-106">Derived from the [targetResource](targetresource.md) resource.</span></span>



## <a name="properties"></a><span data-ttu-id="97347-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="97347-107">Properties</span></span>
| <span data-ttu-id="97347-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="97347-108">Property</span></span>     | <span data-ttu-id="97347-109">Тип</span><span class="sxs-lookup"><span data-stu-id="97347-109">Type</span></span>   |<span data-ttu-id="97347-110">Description</span><span class="sxs-lookup"><span data-stu-id="97347-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97347-111">appId</span><span class="sxs-lookup"><span data-stu-id="97347-111">appId</span></span>|<span data-ttu-id="97347-112">String</span><span class="sxs-lookup"><span data-stu-id="97347-112">String</span></span>|<span data-ttu-id="97347-113">Указывает уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="97347-113">Indicates the Unique Id of the application.</span></span> <span data-ttu-id="97347-114">Указатель идентификатор приложения для приложения содержится код.</span><span class="sxs-lookup"><span data-stu-id="97347-114">Refers to App Id for a specfic app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97347-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97347-115">JSON representation</span></span>

<span data-ttu-id="97347-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97347-116">Here is a JSON representation of the resource.</span></span>

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