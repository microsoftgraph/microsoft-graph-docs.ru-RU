---
title: Тип ресурса filterClause
description: Представляет одно утверждение, которое должен удовлетворять объект-кандидат.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: fc633f6e25373713679da30a5b319ab8ae99fb04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131924"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="98ec6-103">Тип ресурса filterClause</span><span class="sxs-lookup"><span data-stu-id="98ec6-103">filterClause resource type</span></span>

<span data-ttu-id="98ec6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98ec6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98ec6-105">Представляет одно утверждение, которое должно удовлетворяться объектом-кандидатом, и оценивается либо (объект удовлетворяет утверждению), либо (объект не удовлетворяет `true` `false` утверждению).</span><span class="sxs-lookup"><span data-stu-id="98ec6-105">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="98ec6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="98ec6-106">Properties</span></span>
| <span data-ttu-id="98ec6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="98ec6-107">Property</span></span>     | <span data-ttu-id="98ec6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="98ec6-108">Type</span></span>   |<span data-ttu-id="98ec6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="98ec6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98ec6-110">operatorName</span><span class="sxs-lookup"><span data-stu-id="98ec6-110">operatorName</span></span>|<span data-ttu-id="98ec6-111">Строка</span><span class="sxs-lookup"><span data-stu-id="98ec6-111">String</span></span>|<span data-ttu-id="98ec6-112">Имя оператора, применяемого к исходным и целевым операндам.</span><span class="sxs-lookup"><span data-stu-id="98ec6-112">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="98ec6-113">Должен быть одним из поддерживаемых операторов.</span><span class="sxs-lookup"><span data-stu-id="98ec6-113">Must be one of the supported operators.</span></span> <span data-ttu-id="98ec6-114">Поддерживаемые операторы можно обнаружить.</span><span class="sxs-lookup"><span data-stu-id="98ec6-114">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="98ec6-115">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="98ec6-115">sourceOperandName</span></span>|<span data-ttu-id="98ec6-116">Строка</span><span class="sxs-lookup"><span data-stu-id="98ec6-116">String</span></span>|<span data-ttu-id="98ec6-117">Имя операнда источника (проверяемого операнда).</span><span class="sxs-lookup"><span data-stu-id="98ec6-117">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="98ec6-118">Имя операнда источника должно соответствовать одному из имен атрибутов в объекте-источнике.</span><span class="sxs-lookup"><span data-stu-id="98ec6-118">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="98ec6-119">targetOperand</span><span class="sxs-lookup"><span data-stu-id="98ec6-119">targetOperand</span></span>|[<span data-ttu-id="98ec6-120">filterOperand</span><span class="sxs-lookup"><span data-stu-id="98ec6-120">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="98ec6-121">Значения, с которые будет тестироваться исходный операнд.</span><span class="sxs-lookup"><span data-stu-id="98ec6-121">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98ec6-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="98ec6-122">JSON representation</span></span>

<span data-ttu-id="98ec6-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98ec6-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


