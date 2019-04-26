---
title: Тип ресурса Филтерклаусе
description: Представляет одно утверждение, которое должен удовлетворять объект-кандидат, и оценивается как `true` (объект соответствует утверждению) или `false` (объект не соответствует утверждению).
localization_priority: Normal
ms.openlocfilehash: 657651af512fff0b1daf08985e0f14983ca253f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342977"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="3d50e-103">Тип ресурса Филтерклаусе</span><span class="sxs-lookup"><span data-stu-id="3d50e-103">filterClause resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d50e-104">Представляет одно утверждение, которое должен удовлетворять объект-кандидат, и оценивается как `true` (объект соответствует утверждению) или `false` (объект не соответствует утверждению).</span><span class="sxs-lookup"><span data-stu-id="3d50e-104">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="3d50e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d50e-105">Properties</span></span>
| <span data-ttu-id="3d50e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d50e-106">Property</span></span>     | <span data-ttu-id="3d50e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3d50e-107">Type</span></span>   |<span data-ttu-id="3d50e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3d50e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d50e-109">Операторнаме</span><span class="sxs-lookup"><span data-stu-id="3d50e-109">operatorName</span></span>|<span data-ttu-id="3d50e-110">String</span><span class="sxs-lookup"><span data-stu-id="3d50e-110">String</span></span>|<span data-ttu-id="3d50e-111">Имя оператора, применяемого к исходному и целевому операндам.</span><span class="sxs-lookup"><span data-stu-id="3d50e-111">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="3d50e-112">Должен быть одним из поддерживаемых операторов.</span><span class="sxs-lookup"><span data-stu-id="3d50e-112">Must be one of the supported operators.</span></span> <span data-ttu-id="3d50e-113">Могут быть обнаружены поддерживаемые операторы.</span><span class="sxs-lookup"><span data-stu-id="3d50e-113">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="3d50e-114">Саурцеоперанднаме</span><span class="sxs-lookup"><span data-stu-id="3d50e-114">sourceOperandName</span></span>|<span data-ttu-id="3d50e-115">String</span><span class="sxs-lookup"><span data-stu-id="3d50e-115">String</span></span>|<span data-ttu-id="3d50e-116">Имя исходного операнда (тестируемого операнда).</span><span class="sxs-lookup"><span data-stu-id="3d50e-116">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="3d50e-117">Имя исходного операнда должно быть соответствующим одному из имен атрибутов исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="3d50e-117">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="3d50e-118">Таржетоперанд</span><span class="sxs-lookup"><span data-stu-id="3d50e-118">targetOperand</span></span>|[<span data-ttu-id="3d50e-119">Филтероперанд</span><span class="sxs-lookup"><span data-stu-id="3d50e-119">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="3d50e-120">Значения, по которым будет выполняться тестирование исходного операнда.</span><span class="sxs-lookup"><span data-stu-id="3d50e-120">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d50e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d50e-121">JSON representation</span></span>

<span data-ttu-id="3d50e-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d50e-122">The following is a JSON representation of the resource.</span></span>

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
