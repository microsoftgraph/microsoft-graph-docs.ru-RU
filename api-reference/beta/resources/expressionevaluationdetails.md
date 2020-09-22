---
title: Тип ресурса Експрессионевалуатиондетаилс
description: Представляет сведения о выражении, сведения о результатах и свойствах.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f2d14d19bee60581c65d43e81b5ec69acc53df0a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026978"
---
# <a name="expressionevaluationdetails-resource-type"></a><span data-ttu-id="46387-103">Тип ресурса Експрессионевалуатиондетаилс</span><span class="sxs-lookup"><span data-stu-id="46387-103">expressionEvaluationDetails resource type</span></span>

<span data-ttu-id="46387-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46387-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46387-105">Представляет сведения о выражении, сведения о результатах и свойствах.</span><span class="sxs-lookup"><span data-stu-id="46387-105">Represents the expression details, result, and property details.</span></span>

## <a name="properties"></a><span data-ttu-id="46387-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="46387-106">Properties</span></span>

| <span data-ttu-id="46387-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="46387-107">Property</span></span>     | <span data-ttu-id="46387-108">Тип</span><span class="sxs-lookup"><span data-stu-id="46387-108">Type</span></span>        | <span data-ttu-id="46387-109">Описание</span><span class="sxs-lookup"><span data-stu-id="46387-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="46387-110">выражение</span><span class="sxs-lookup"><span data-stu-id="46387-110">expression</span></span> | <span data-ttu-id="46387-111">String</span><span class="sxs-lookup"><span data-stu-id="46387-111">String</span></span> | <span data-ttu-id="46387-112">Представляет выражение, которое было оценено.</span><span class="sxs-lookup"><span data-stu-id="46387-112">Represents expression which has been evaluated.</span></span> |
| <span data-ttu-id="46387-113">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="46387-113">expressionEvaluationDetails</span></span> | <span data-ttu-id="46387-114">Коллекция Експрессионевалуатиондетаилс</span><span class="sxs-lookup"><span data-stu-id="46387-114">expressionEvaluationDetails collection</span></span> | <span data-ttu-id="46387-115">Представляет сведения об оценке выражения.</span><span class="sxs-lookup"><span data-stu-id="46387-115">Represents the details of the evaluation of the expression.</span></span> |
| <span data-ttu-id="46387-116">експрессионресулт</span><span class="sxs-lookup"><span data-stu-id="46387-116">expressionResult</span></span> | <span data-ttu-id="46387-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="46387-117">Boolean</span></span> | <span data-ttu-id="46387-118">Представляет значение результата текущего выражения.</span><span class="sxs-lookup"><span data-stu-id="46387-118">Represents the value of the result of the current expression.</span></span> |
| <span data-ttu-id="46387-119">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="46387-119">propertyToEvaluate</span></span> | [<span data-ttu-id="46387-120">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="46387-120">propertyToEvaluate</span></span>](propertytoevaluate.md) | <span data-ttu-id="46387-121">Определяет имя свойства и значение этого свойства.</span><span class="sxs-lookup"><span data-stu-id="46387-121">Defines the name of the property and the value of that property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="46387-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46387-122">JSON representation</span></span>

<span data-ttu-id="46387-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46387-123">The following is a JSON representation of the resource.</span></span>

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


