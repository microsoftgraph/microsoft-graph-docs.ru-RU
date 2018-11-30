---
title: Тип ресурса targetResourcePolicy
description: 'Указывает политику, которая была влияют активности аудита. На основе targetResource ресурсов.   '
ms.openlocfilehash: 20486c535d0df4b3745f5cfc3414b320a9374075
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080090"
---
# <a name="targetresourcepolicy-resource-type"></a><span data-ttu-id="7c133-104">Тип ресурса targetResourcePolicy</span><span class="sxs-lookup"><span data-stu-id="7c133-104">targetResourcePolicy resource type</span></span>
<span data-ttu-id="7c133-105">Указывает политику, которая была влияют активности аудита.</span><span class="sxs-lookup"><span data-stu-id="7c133-105">Indicates the policy that was impacted by the audit activity.</span></span> <span data-ttu-id="7c133-106">На основе [targetResource](targetresource.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7c133-106">Derived from the [targetResource](targetresource.md) resource.</span></span>   



## <a name="properties"></a><span data-ttu-id="7c133-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c133-107">Properties</span></span>
| <span data-ttu-id="7c133-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c133-108">Property</span></span>     | <span data-ttu-id="7c133-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7c133-109">Type</span></span>   |<span data-ttu-id="7c133-110">Description</span><span class="sxs-lookup"><span data-stu-id="7c133-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c133-111">policyType</span><span class="sxs-lookup"><span data-stu-id="7c133-111">policyType</span></span>|<span data-ttu-id="7c133-112">String</span><span class="sxs-lookup"><span data-stu-id="7c133-112">String</span></span>|<span data-ttu-id="7c133-113">Указывает имя политики, измененные или был targetted для изменения</span><span class="sxs-lookup"><span data-stu-id="7c133-113">Indicates the Policy Name that changed or was targetted for change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c133-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c133-114">JSON representation</span></span>

<span data-ttu-id="7c133-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c133-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourcePolicy"
}-->

```json
{
  "policyType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourcePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->