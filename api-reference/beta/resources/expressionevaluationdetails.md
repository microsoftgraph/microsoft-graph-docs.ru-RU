---
title: Тип ресурса expressionEvaluationDetails
description: Представляет сведения об выражениях, результатах и свойствах.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 01cc4aa4bd6de88541d3886efe54e5da71228448
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129494"
---
# <a name="expressionevaluationdetails-resource-type"></a><span data-ttu-id="cedfa-103">Тип ресурса expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="cedfa-103">expressionEvaluationDetails resource type</span></span>

<span data-ttu-id="cedfa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cedfa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cedfa-105">Представляет сведения об выражениях, результатах и свойствах.</span><span class="sxs-lookup"><span data-stu-id="cedfa-105">Represents the expression details, result, and property details.</span></span>

## <a name="properties"></a><span data-ttu-id="cedfa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cedfa-106">Properties</span></span>

| <span data-ttu-id="cedfa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cedfa-107">Property</span></span>     | <span data-ttu-id="cedfa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cedfa-108">Type</span></span>        | <span data-ttu-id="cedfa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cedfa-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cedfa-110">выражение</span><span class="sxs-lookup"><span data-stu-id="cedfa-110">expression</span></span> | <span data-ttu-id="cedfa-111">Строка</span><span class="sxs-lookup"><span data-stu-id="cedfa-111">String</span></span> | <span data-ttu-id="cedfa-112">Представляет выражение, которое было оценено.</span><span class="sxs-lookup"><span data-stu-id="cedfa-112">Represents expression which has been evaluated.</span></span> |
| <span data-ttu-id="cedfa-113">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="cedfa-113">expressionEvaluationDetails</span></span> | <span data-ttu-id="cedfa-114">Коллекция expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="cedfa-114">expressionEvaluationDetails collection</span></span> | <span data-ttu-id="cedfa-115">Представляет сведения об оценке выражения.</span><span class="sxs-lookup"><span data-stu-id="cedfa-115">Represents the details of the evaluation of the expression.</span></span> |
| <span data-ttu-id="cedfa-116">expressionResult</span><span class="sxs-lookup"><span data-stu-id="cedfa-116">expressionResult</span></span> | <span data-ttu-id="cedfa-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="cedfa-117">Boolean</span></span> | <span data-ttu-id="cedfa-118">Представляет значение результата текущего выражения.</span><span class="sxs-lookup"><span data-stu-id="cedfa-118">Represents the value of the result of the current expression.</span></span> |
| <span data-ttu-id="cedfa-119">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="cedfa-119">propertyToEvaluate</span></span> | [<span data-ttu-id="cedfa-120">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="cedfa-120">propertyToEvaluate</span></span>](propertytoevaluate.md) | <span data-ttu-id="cedfa-121">Определяет имя свойства и его значение.</span><span class="sxs-lookup"><span data-stu-id="cedfa-121">Defines the name of the property and the value of that property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cedfa-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cedfa-122">JSON representation</span></span>

<span data-ttu-id="cedfa-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cedfa-123">The following is a JSON representation of the resource.</span></span>

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


