---
title: тип ресурса expressionEvaluationDetails
description: Представляет сведения об выражениях, результатах и свойствах.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a2e2b2620f30234c23753ef743f14e55e29f6f91
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679902"
---
# <a name="expressionevaluationdetails-resource-type"></a><span data-ttu-id="8539d-103">тип ресурса expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="8539d-103">expressionEvaluationDetails resource type</span></span>

<span data-ttu-id="8539d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8539d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8539d-105">Представляет сведения об выражениях, результатах и свойствах.</span><span class="sxs-lookup"><span data-stu-id="8539d-105">Represents the expression details, result, and property details.</span></span>

## <a name="properties"></a><span data-ttu-id="8539d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8539d-106">Properties</span></span>

| <span data-ttu-id="8539d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8539d-107">Property</span></span>     | <span data-ttu-id="8539d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8539d-108">Type</span></span>        | <span data-ttu-id="8539d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8539d-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8539d-110">выражение</span><span class="sxs-lookup"><span data-stu-id="8539d-110">expression</span></span> | <span data-ttu-id="8539d-111">String</span><span class="sxs-lookup"><span data-stu-id="8539d-111">String</span></span> | <span data-ttu-id="8539d-112">Представляет выражение, которое было оценено.</span><span class="sxs-lookup"><span data-stu-id="8539d-112">Represents expression which has been evaluated.</span></span> |
| <span data-ttu-id="8539d-113">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="8539d-113">expressionEvaluationDetails</span></span> | <span data-ttu-id="8539d-114">коллекция expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="8539d-114">expressionEvaluationDetails collection</span></span> | <span data-ttu-id="8539d-115">Представляет сведения об оценке выражения.</span><span class="sxs-lookup"><span data-stu-id="8539d-115">Represents the details of the evaluation of the expression.</span></span> |
| <span data-ttu-id="8539d-116">expressionResult</span><span class="sxs-lookup"><span data-stu-id="8539d-116">expressionResult</span></span> | <span data-ttu-id="8539d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="8539d-117">Boolean</span></span> | <span data-ttu-id="8539d-118">Представляет значение результата текущего выражения.</span><span class="sxs-lookup"><span data-stu-id="8539d-118">Represents the value of the result of the current expression.</span></span> |
| <span data-ttu-id="8539d-119">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="8539d-119">propertyToEvaluate</span></span> | [<span data-ttu-id="8539d-120">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="8539d-120">propertyToEvaluate</span></span>](propertytoevaluate.md) | <span data-ttu-id="8539d-121">Определяет имя свойства и значение этого свойства.</span><span class="sxs-lookup"><span data-stu-id="8539d-121">Defines the name of the property and the value of that property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8539d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8539d-122">JSON representation</span></span>

<span data-ttu-id="8539d-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8539d-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionEvaluationDetails",
  "baseType": null
}-->

```json
{
  "expression": "String",
  "expressionEvaluationDetails": [{"@odata.type": "microsoft.graph.expressionEvaluationDetails"}],
  "expressionResult": true,
  "propertyToEvaluate": {"@odata.type": "microsoft.graph.propertyToEvaluate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expressionEvaluationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


