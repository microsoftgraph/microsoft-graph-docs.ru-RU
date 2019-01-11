---
title: Тип ресурса targetResourcePolicy
description: 'Указывает политику, которая была влияют активности аудита. На основе targetResource ресурсов.   '
localization_priority: Normal
ms.openlocfilehash: 355e6ac11741a2aa7aeb780bdac4b7be373092af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813141"
---
# <a name="targetresourcepolicy-resource-type"></a><span data-ttu-id="e4769-104">Тип ресурса targetResourcePolicy</span><span class="sxs-lookup"><span data-stu-id="e4769-104">targetResourcePolicy resource type</span></span>
<span data-ttu-id="e4769-105">Указывает политику, которая была влияют активности аудита.</span><span class="sxs-lookup"><span data-stu-id="e4769-105">Indicates the policy that was impacted by the audit activity.</span></span> <span data-ttu-id="e4769-106">На основе [targetResource](targetresource.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e4769-106">Derived from the [targetResource](targetresource.md) resource.</span></span>   



## <a name="properties"></a><span data-ttu-id="e4769-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4769-107">Properties</span></span>
| <span data-ttu-id="e4769-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4769-108">Property</span></span>     | <span data-ttu-id="e4769-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e4769-109">Type</span></span>   |<span data-ttu-id="e4769-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e4769-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4769-111">policyType</span><span class="sxs-lookup"><span data-stu-id="e4769-111">policyType</span></span>|<span data-ttu-id="e4769-112">Строка</span><span class="sxs-lookup"><span data-stu-id="e4769-112">String</span></span>|<span data-ttu-id="e4769-113">Указывает имя политики, измененные или был targetted для изменения</span><span class="sxs-lookup"><span data-stu-id="e4769-113">Indicates the Policy Name that changed or was targetted for change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4769-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4769-114">JSON representation</span></span>

<span data-ttu-id="e4769-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4769-115">Here is a JSON representation of the resource.</span></span>

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
