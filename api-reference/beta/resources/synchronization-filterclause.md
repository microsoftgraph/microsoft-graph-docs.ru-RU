---
title: Тип ресурса Филтерклаусе
description: Представляет одно утверждение, которое должен удовлетворять объект-кандидат, и оценивается как `true` (объект соответствует утверждению) или `false` (объект не соответствует утверждению).
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 83b9c68bd86f716b47a3ba3774022ff3ba520770
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007937"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="7537b-103">Тип ресурса Филтерклаусе</span><span class="sxs-lookup"><span data-stu-id="7537b-103">filterClause resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7537b-104">Представляет одно утверждение, которое должен удовлетворять объект-кандидат, и оценивается как `true` (объект соответствует утверждению) или `false` (объект не соответствует утверждению).</span><span class="sxs-lookup"><span data-stu-id="7537b-104">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="7537b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7537b-105">Properties</span></span>
| <span data-ttu-id="7537b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7537b-106">Property</span></span>     | <span data-ttu-id="7537b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7537b-107">Type</span></span>   |<span data-ttu-id="7537b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7537b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7537b-109">Операторнаме</span><span class="sxs-lookup"><span data-stu-id="7537b-109">operatorName</span></span>|<span data-ttu-id="7537b-110">String</span><span class="sxs-lookup"><span data-stu-id="7537b-110">String</span></span>|<span data-ttu-id="7537b-111">Имя оператора, применяемого к исходному и целевому операндам.</span><span class="sxs-lookup"><span data-stu-id="7537b-111">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="7537b-112">Должен быть одним из поддерживаемых операторов.</span><span class="sxs-lookup"><span data-stu-id="7537b-112">Must be one of the supported operators.</span></span> <span data-ttu-id="7537b-113">Могут быть обнаружены поддерживаемые операторы.</span><span class="sxs-lookup"><span data-stu-id="7537b-113">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="7537b-114">Саурцеоперанднаме</span><span class="sxs-lookup"><span data-stu-id="7537b-114">sourceOperandName</span></span>|<span data-ttu-id="7537b-115">String</span><span class="sxs-lookup"><span data-stu-id="7537b-115">String</span></span>|<span data-ttu-id="7537b-116">Имя исходного операнда (тестируемого операнда).</span><span class="sxs-lookup"><span data-stu-id="7537b-116">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="7537b-117">Имя исходного операнда должно быть соответствующим одному из имен атрибутов исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="7537b-117">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="7537b-118">Таржетоперанд</span><span class="sxs-lookup"><span data-stu-id="7537b-118">targetOperand</span></span>|[<span data-ttu-id="7537b-119">Филтероперанд</span><span class="sxs-lookup"><span data-stu-id="7537b-119">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="7537b-120">Значения, по которым будет выполняться тестирование исходного операнда.</span><span class="sxs-lookup"><span data-stu-id="7537b-120">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7537b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7537b-121">JSON representation</span></span>

<span data-ttu-id="7537b-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7537b-122">The following is a JSON representation of the resource.</span></span>

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
