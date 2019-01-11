---
title: Тип ресурса filterClause
description: Представляет один утверждения, в котором объект-кандидат должны соответствовать и вычисляется на любой `true` (объект должна удовлетворять утверждение) или `false` (объект не удовлетворяет утверждение).
localization_priority: Normal
ms.openlocfilehash: 89807a6086f661388c8d5b1d5f82bfe973c3af39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833861"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="600fb-103">Тип ресурса filterClause</span><span class="sxs-lookup"><span data-stu-id="600fb-103">filterClause resource type</span></span>

> <span data-ttu-id="600fb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="600fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="600fb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="600fb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="600fb-106">Представляет один утверждения, в котором объект-кандидат должны соответствовать и вычисляется на любой `true` (объект должна удовлетворять утверждение) или `false` (объект не удовлетворяет утверждение).</span><span class="sxs-lookup"><span data-stu-id="600fb-106">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="600fb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="600fb-107">Properties</span></span>
| <span data-ttu-id="600fb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="600fb-108">Property</span></span>     | <span data-ttu-id="600fb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="600fb-109">Type</span></span>   |<span data-ttu-id="600fb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="600fb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="600fb-111">operatorName</span><span class="sxs-lookup"><span data-stu-id="600fb-111">operatorName</span></span>|<span data-ttu-id="600fb-112">Строка</span><span class="sxs-lookup"><span data-stu-id="600fb-112">String</span></span>|<span data-ttu-id="600fb-113">Имя оператор, который должен применяться к исходной и целевой операндов.</span><span class="sxs-lookup"><span data-stu-id="600fb-113">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="600fb-114">Должен быть один из поддерживаемых операторов.</span><span class="sxs-lookup"><span data-stu-id="600fb-114">Must be one of the supported operators.</span></span> <span data-ttu-id="600fb-115">Для обнаружения поддерживаемых операторов.</span><span class="sxs-lookup"><span data-stu-id="600fb-115">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="600fb-116">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="600fb-116">sourceOperandName</span></span>|<span data-ttu-id="600fb-117">Строка</span><span class="sxs-lookup"><span data-stu-id="600fb-117">String</span></span>|<span data-ttu-id="600fb-118">Имя источника операнд (операнд проверяемой).</span><span class="sxs-lookup"><span data-stu-id="600fb-118">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="600fb-119">Операнд имя источника должно соответствовать одному из имен атрибутов в объекте источника.</span><span class="sxs-lookup"><span data-stu-id="600fb-119">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="600fb-120">targetOperand</span><span class="sxs-lookup"><span data-stu-id="600fb-120">targetOperand</span></span>|[<span data-ttu-id="600fb-121">filterOperand</span><span class="sxs-lookup"><span data-stu-id="600fb-121">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="600fb-122">Значения, которые исходный операнд проверяется.</span><span class="sxs-lookup"><span data-stu-id="600fb-122">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="600fb-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="600fb-123">JSON representation</span></span>

<span data-ttu-id="600fb-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="600fb-124">The following is a JSON representation of the resource.</span></span>

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
