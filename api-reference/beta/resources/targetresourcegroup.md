---
title: Тип ресурса targetResourceGroup
description: 'Указывает тип группы, которая изменилась из-за загрузки аудита. Содержит значения, как объединенные группам и Azure AD '
ms.openlocfilehash: 3427f2401a0e93767f0c563842be323f66d9f21b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078090"
---
# <a name="targetresourcegroup-resource-type"></a><span data-ttu-id="54ea4-104">Тип ресурса targetResourceGroup</span><span class="sxs-lookup"><span data-stu-id="54ea4-104">targetResourceGroup resource type</span></span>
<span data-ttu-id="54ea4-105">Указывает тип группы, которая изменилась из-за загрузки аудита.</span><span class="sxs-lookup"><span data-stu-id="54ea4-105">Indicates the type of group that was impacted due to the audit activity.</span></span> <span data-ttu-id="54ea4-106">Содержит значения, как объединенные группам и Azure AD</span><span class="sxs-lookup"><span data-stu-id="54ea4-106">Includes values like unified groups versus Azure AD</span></span> 



## <a name="properties"></a><span data-ttu-id="54ea4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="54ea4-107">Properties</span></span>
| <span data-ttu-id="54ea4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="54ea4-108">Property</span></span>     | <span data-ttu-id="54ea4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="54ea4-109">Type</span></span>   |<span data-ttu-id="54ea4-110">Description</span><span class="sxs-lookup"><span data-stu-id="54ea4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54ea4-111">groupType</span><span class="sxs-lookup"><span data-stu-id="54ea4-111">groupType</span></span>|<span data-ttu-id="54ea4-112">String</span><span class="sxs-lookup"><span data-stu-id="54ea4-112">String</span></span>| <span data-ttu-id="54ea4-113">Возможные значения: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="54ea4-113">Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54ea4-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54ea4-114">JSON representation</span></span>

<span data-ttu-id="54ea4-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54ea4-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceGroup"
}-->

```json
{
  "groupType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->