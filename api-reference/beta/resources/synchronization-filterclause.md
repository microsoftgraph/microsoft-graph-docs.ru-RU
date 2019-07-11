---
title: Тип ресурса Филтерклаусе
description: Представляет одно утверждение, которое должен удовлетворять объект-кандидат, и оценивается как `true` (объект соответствует утверждению) или `false` (объект не соответствует утверждению).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 788dcd8741d89639ce2c57511ae54e466815e366
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621426"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="796ba-103">Тип ресурса Филтерклаусе</span><span class="sxs-lookup"><span data-stu-id="796ba-103">filterClause resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="796ba-104">Представляет одно утверждение, которое должен удовлетворять объект-кандидат, и оценивается как `true` (объект соответствует утверждению) или `false` (объект не соответствует утверждению).</span><span class="sxs-lookup"><span data-stu-id="796ba-104">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="796ba-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="796ba-105">Properties</span></span>
| <span data-ttu-id="796ba-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="796ba-106">Property</span></span>     | <span data-ttu-id="796ba-107">Тип</span><span class="sxs-lookup"><span data-stu-id="796ba-107">Type</span></span>   |<span data-ttu-id="796ba-108">Описание</span><span class="sxs-lookup"><span data-stu-id="796ba-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="796ba-109">Операторнаме</span><span class="sxs-lookup"><span data-stu-id="796ba-109">operatorName</span></span>|<span data-ttu-id="796ba-110">String</span><span class="sxs-lookup"><span data-stu-id="796ba-110">String</span></span>|<span data-ttu-id="796ba-111">Имя оператора, применяемого к исходному и целевому операндам.</span><span class="sxs-lookup"><span data-stu-id="796ba-111">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="796ba-112">Должен быть одним из поддерживаемых операторов.</span><span class="sxs-lookup"><span data-stu-id="796ba-112">Must be one of the supported operators.</span></span> <span data-ttu-id="796ba-113">Могут быть обнаружены поддерживаемые операторы.</span><span class="sxs-lookup"><span data-stu-id="796ba-113">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="796ba-114">Саурцеоперанднаме</span><span class="sxs-lookup"><span data-stu-id="796ba-114">sourceOperandName</span></span>|<span data-ttu-id="796ba-115">String</span><span class="sxs-lookup"><span data-stu-id="796ba-115">String</span></span>|<span data-ttu-id="796ba-116">Имя исходного операнда (тестируемого операнда).</span><span class="sxs-lookup"><span data-stu-id="796ba-116">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="796ba-117">Имя исходного операнда должно быть соответствующим одному из имен атрибутов исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="796ba-117">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="796ba-118">Таржетоперанд</span><span class="sxs-lookup"><span data-stu-id="796ba-118">targetOperand</span></span>|[<span data-ttu-id="796ba-119">Филтероперанд</span><span class="sxs-lookup"><span data-stu-id="796ba-119">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="796ba-120">Значения, по которым будет выполняться тестирование исходного операнда.</span><span class="sxs-lookup"><span data-stu-id="796ba-120">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="796ba-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="796ba-121">JSON representation</span></span>

<span data-ttu-id="796ba-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="796ba-122">The following is a JSON representation of the resource.</span></span>

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
