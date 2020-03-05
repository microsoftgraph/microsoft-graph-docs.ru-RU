---
title: Тип ресурса Филтерклаусе
description: Представляет одно утверждение, которое должен удовлетворять объект-кандидат, и оценивается как `true` (объект соответствует утверждению) или `false` (объект не соответствует утверждению).
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 66ccbc4e445b6fa90dad1bac55c00f894bbd934b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520193"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="0a31f-103">Тип ресурса Филтерклаусе</span><span class="sxs-lookup"><span data-stu-id="0a31f-103">filterClause resource type</span></span>

<span data-ttu-id="0a31f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0a31f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a31f-105">Представляет одно утверждение, которое должен удовлетворять объект-кандидат, и оценивается как `true` (объект соответствует утверждению) или `false` (объект не соответствует утверждению).</span><span class="sxs-lookup"><span data-stu-id="0a31f-105">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="0a31f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a31f-106">Properties</span></span>
| <span data-ttu-id="0a31f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a31f-107">Property</span></span>     | <span data-ttu-id="0a31f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0a31f-108">Type</span></span>   |<span data-ttu-id="0a31f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0a31f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a31f-110">операторнаме</span><span class="sxs-lookup"><span data-stu-id="0a31f-110">operatorName</span></span>|<span data-ttu-id="0a31f-111">String</span><span class="sxs-lookup"><span data-stu-id="0a31f-111">String</span></span>|<span data-ttu-id="0a31f-112">Имя оператора, применяемого к исходному и целевому операндам.</span><span class="sxs-lookup"><span data-stu-id="0a31f-112">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="0a31f-113">Должен быть одним из поддерживаемых операторов.</span><span class="sxs-lookup"><span data-stu-id="0a31f-113">Must be one of the supported operators.</span></span> <span data-ttu-id="0a31f-114">Могут быть обнаружены поддерживаемые операторы.</span><span class="sxs-lookup"><span data-stu-id="0a31f-114">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="0a31f-115">саурцеоперанднаме</span><span class="sxs-lookup"><span data-stu-id="0a31f-115">sourceOperandName</span></span>|<span data-ttu-id="0a31f-116">String</span><span class="sxs-lookup"><span data-stu-id="0a31f-116">String</span></span>|<span data-ttu-id="0a31f-117">Имя исходного операнда (тестируемого операнда).</span><span class="sxs-lookup"><span data-stu-id="0a31f-117">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="0a31f-118">Имя исходного операнда должно быть соответствующим одному из имен атрибутов исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="0a31f-118">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="0a31f-119">таржетоперанд</span><span class="sxs-lookup"><span data-stu-id="0a31f-119">targetOperand</span></span>|[<span data-ttu-id="0a31f-120">филтероперанд</span><span class="sxs-lookup"><span data-stu-id="0a31f-120">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="0a31f-121">Значения, по которым будет выполняться тестирование исходного операнда.</span><span class="sxs-lookup"><span data-stu-id="0a31f-121">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a31f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a31f-122">JSON representation</span></span>

<span data-ttu-id="0a31f-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a31f-123">The following is a JSON representation of the resource.</span></span>

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
