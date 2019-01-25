---
title: Тип ресурса filterClause
description: Представляет один утверждения, в котором объект-кандидат должны соответствовать и вычисляется на любой `true` (объект должна удовлетворять утверждение) или `false` (объект не удовлетворяет утверждение).
localization_priority: Normal
ms.openlocfilehash: 62623cee5b2991acbe162561940adb1afd3574a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523871"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="23e19-103">Тип ресурса filterClause</span><span class="sxs-lookup"><span data-stu-id="23e19-103">filterClause resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23e19-104">Представляет один утверждения, в котором объект-кандидат должны соответствовать и вычисляется на любой `true` (объект должна удовлетворять утверждение) или `false` (объект не удовлетворяет утверждение).</span><span class="sxs-lookup"><span data-stu-id="23e19-104">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="23e19-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="23e19-105">Properties</span></span>
| <span data-ttu-id="23e19-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="23e19-106">Property</span></span>     | <span data-ttu-id="23e19-107">Тип</span><span class="sxs-lookup"><span data-stu-id="23e19-107">Type</span></span>   |<span data-ttu-id="23e19-108">Описание</span><span class="sxs-lookup"><span data-stu-id="23e19-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23e19-109">operatorName</span><span class="sxs-lookup"><span data-stu-id="23e19-109">operatorName</span></span>|<span data-ttu-id="23e19-110">String</span><span class="sxs-lookup"><span data-stu-id="23e19-110">String</span></span>|<span data-ttu-id="23e19-111">Имя оператор, который должен применяться к исходной и целевой операндов.</span><span class="sxs-lookup"><span data-stu-id="23e19-111">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="23e19-112">Должен быть один из поддерживаемых операторов.</span><span class="sxs-lookup"><span data-stu-id="23e19-112">Must be one of the supported operators.</span></span> <span data-ttu-id="23e19-113">Для обнаружения поддерживаемых операторов.</span><span class="sxs-lookup"><span data-stu-id="23e19-113">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="23e19-114">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="23e19-114">sourceOperandName</span></span>|<span data-ttu-id="23e19-115">String</span><span class="sxs-lookup"><span data-stu-id="23e19-115">String</span></span>|<span data-ttu-id="23e19-116">Имя источника операнд (операнд проверяемой).</span><span class="sxs-lookup"><span data-stu-id="23e19-116">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="23e19-117">Операнд имя источника должно соответствовать одному из имен атрибутов в объекте источника.</span><span class="sxs-lookup"><span data-stu-id="23e19-117">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="23e19-118">targetOperand</span><span class="sxs-lookup"><span data-stu-id="23e19-118">targetOperand</span></span>|[<span data-ttu-id="23e19-119">filterOperand</span><span class="sxs-lookup"><span data-stu-id="23e19-119">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="23e19-120">Значения, которые исходный операнд проверяется.</span><span class="sxs-lookup"><span data-stu-id="23e19-120">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23e19-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23e19-121">JSON representation</span></span>

<span data-ttu-id="23e19-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23e19-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterClause"
}-->

```json
{
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {"@odata.type": "microsoft.graph.filterOperand"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filterclause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
