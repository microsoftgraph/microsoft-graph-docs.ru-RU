---
title: Тип ресурса filterOperatorSchema
description: Описывает оператор, который может использоваться в фильтре.
localization_priority: Normal
ms.openlocfilehash: 366e00b5d21efeaf67e3e799c5b1c2412a68e268
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573685"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="e691f-103">Тип ресурса filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="e691f-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e691f-104">Описывает оператор, который можно использовать в [Фильтр](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="e691f-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e691f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e691f-105">Properties</span></span>

| <span data-ttu-id="e691f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e691f-106">Property</span></span>                   | <span data-ttu-id="e691f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e691f-107">Type</span></span>                      | <span data-ttu-id="e691f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e691f-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="e691f-109">арность</span><span class="sxs-lookup"><span data-stu-id="e691f-109">arity</span></span>                       | <span data-ttu-id="e691f-110">microsoft.graph.scopeOperatorType</span><span class="sxs-lookup"><span data-stu-id="e691f-110">microsoft.graph.scopeOperatorType</span></span>         |<span data-ttu-id="e691f-111">Арность оператора.</span><span class="sxs-lookup"><span data-stu-id="e691f-111">Arity of the operator.</span></span> <span data-ttu-id="e691f-112">Возможные значения: `Binary`, `Unary`.</span><span class="sxs-lookup"><span data-stu-id="e691f-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="e691f-113">Значение по умолчанию — `Binary`.</span><span class="sxs-lookup"><span data-stu-id="e691f-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="e691f-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="e691f-114">multivaluedComparisonType</span></span>   | <span data-ttu-id="e691f-115">microsoft.graph.scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="e691f-115">microsoft.graph.scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="e691f-116">Возможные значения: `All`, `Any`.</span><span class="sxs-lookup"><span data-stu-id="e691f-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="e691f-117">Применяется только к многозначных атрибутов.</span><span class="sxs-lookup"><span data-stu-id="e691f-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="e691f-118">`All`означает, что все значения должны соответствовать условие.</span><span class="sxs-lookup"><span data-stu-id="e691f-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="e691f-119">`Any`означает, что по крайней мере одно значение должен удовлетворяют условию.</span><span class="sxs-lookup"><span data-stu-id="e691f-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="e691f-120">Значение по умолчанию — `All`.</span><span class="sxs-lookup"><span data-stu-id="e691f-120">The default is `All`.</span></span>|
|<span data-ttu-id="e691f-121">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="e691f-121">supportedAttributeTypes</span></span>     | <span data-ttu-id="e691f-122">attributeType семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="e691f-122">attributeType collection</span></span>         |<span data-ttu-id="e691f-123">Атрибут типы, которые поддерживаются оператором.</span><span class="sxs-lookup"><span data-stu-id="e691f-123">Attribute types supported by the operator.</span></span> <span data-ttu-id="e691f-124">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="e691f-124">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e691f-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e691f-125">JSON representation</span></span>

<span data-ttu-id="e691f-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e691f-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "microsoft.graph.scopeOperatorType",
  "multivaluedComparisonType": "microsoft.graph.scopeOperatorMultiValuedComparisonType",  
  "supportedAttributeTypes": ["attributeType"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filteroperatorschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
