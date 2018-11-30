---
title: Тип ресурса filterClause
description: Представляет один утверждения, в котором объект-кандидат должны соответствовать и вычисляется на любой `true` (объект должна удовлетворять утверждение) или `false` (объект не удовлетворяет утверждение).
ms.openlocfilehash: 0861324849f224c4e750f0c7b926464280b9a377
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076033"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="1fc6c-103">Тип ресурса filterClause</span><span class="sxs-lookup"><span data-stu-id="1fc6c-103">filterClause resource type</span></span>

> <span data-ttu-id="1fc6c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1fc6c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fc6c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fc6c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1fc6c-106">Представляет один утверждения, в котором объект-кандидат должны соответствовать и вычисляется на любой `true` (объект должна удовлетворять утверждение) или `false` (объект не удовлетворяет утверждение).</span><span class="sxs-lookup"><span data-stu-id="1fc6c-106">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="1fc6c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1fc6c-107">Properties</span></span>
| <span data-ttu-id="1fc6c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fc6c-108">Property</span></span>     | <span data-ttu-id="1fc6c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1fc6c-109">Type</span></span>   |<span data-ttu-id="1fc6c-110">Description</span><span class="sxs-lookup"><span data-stu-id="1fc6c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fc6c-111">operatorName</span><span class="sxs-lookup"><span data-stu-id="1fc6c-111">operatorName</span></span>|<span data-ttu-id="1fc6c-112">String</span><span class="sxs-lookup"><span data-stu-id="1fc6c-112">String</span></span>|<span data-ttu-id="1fc6c-113">Имя оператор, который должен применяться к исходной и целевой операндов.</span><span class="sxs-lookup"><span data-stu-id="1fc6c-113">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="1fc6c-114">Должен быть один из поддерживаемых операторов.</span><span class="sxs-lookup"><span data-stu-id="1fc6c-114">Must be one of the supported operators.</span></span> <span data-ttu-id="1fc6c-115">Для обнаружения поддерживаемых операторов.</span><span class="sxs-lookup"><span data-stu-id="1fc6c-115">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="1fc6c-116">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="1fc6c-116">sourceOperandName</span></span>|<span data-ttu-id="1fc6c-117">String</span><span class="sxs-lookup"><span data-stu-id="1fc6c-117">String</span></span>|<span data-ttu-id="1fc6c-118">Имя источника операнд (операнд проверяемой).</span><span class="sxs-lookup"><span data-stu-id="1fc6c-118">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="1fc6c-119">Операнд имя источника должно соответствовать одному из имен атрибутов в объекте источника.</span><span class="sxs-lookup"><span data-stu-id="1fc6c-119">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="1fc6c-120">targetOperand</span><span class="sxs-lookup"><span data-stu-id="1fc6c-120">targetOperand</span></span>|[<span data-ttu-id="1fc6c-121">filterOperand</span><span class="sxs-lookup"><span data-stu-id="1fc6c-121">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="1fc6c-122">Значения, которые исходный операнд проверяется.</span><span class="sxs-lookup"><span data-stu-id="1fc6c-122">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fc6c-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1fc6c-123">JSON representation</span></span>

<span data-ttu-id="1fc6c-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fc6c-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->