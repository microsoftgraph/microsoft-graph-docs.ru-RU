---
title: Тип ресурса targetResourceGroup
description: 'Указывает тип группы, которая изменилась из-за загрузки аудита. Содержит значения, как объединенные группам и Azure AD '
localization_priority: Normal
ms.openlocfilehash: 2cc7e0adb1a93394b64375d05dfb6a6e349bac55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851186"
---
# <a name="targetresourcegroup-resource-type"></a><span data-ttu-id="c931f-104">Тип ресурса targetResourceGroup</span><span class="sxs-lookup"><span data-stu-id="c931f-104">targetResourceGroup resource type</span></span>
<span data-ttu-id="c931f-105">Указывает тип группы, которая изменилась из-за загрузки аудита.</span><span class="sxs-lookup"><span data-stu-id="c931f-105">Indicates the type of group that was impacted due to the audit activity.</span></span> <span data-ttu-id="c931f-106">Содержит значения, как объединенные группам и Azure AD</span><span class="sxs-lookup"><span data-stu-id="c931f-106">Includes values like unified groups versus Azure AD</span></span> 



## <a name="properties"></a><span data-ttu-id="c931f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c931f-107">Properties</span></span>
| <span data-ttu-id="c931f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c931f-108">Property</span></span>     | <span data-ttu-id="c931f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c931f-109">Type</span></span>   |<span data-ttu-id="c931f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c931f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c931f-111">groupType</span><span class="sxs-lookup"><span data-stu-id="c931f-111">groupType</span></span>|<span data-ttu-id="c931f-112">Строка</span><span class="sxs-lookup"><span data-stu-id="c931f-112">String</span></span>| <span data-ttu-id="c931f-113">Возможные значения: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c931f-113">Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c931f-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c931f-114">JSON representation</span></span>

<span data-ttu-id="c931f-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c931f-115">Here is a JSON representation of the resource.</span></span>

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
