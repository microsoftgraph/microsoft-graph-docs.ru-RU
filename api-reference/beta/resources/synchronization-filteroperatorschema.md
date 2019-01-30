---
title: Тип ресурса filterOperatorSchema
description: Описывает оператор, который может использоваться в фильтре.
localization_priority: Normal
ms.openlocfilehash: 04bee90f81c0098832cd4b6355be266668d0f69b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641822"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="7ad44-103">Тип ресурса filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="7ad44-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ad44-104">Описывает оператор, который можно использовать в [Фильтр](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="7ad44-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7ad44-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ad44-105">Properties</span></span>

| <span data-ttu-id="7ad44-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ad44-106">Property</span></span>                   | <span data-ttu-id="7ad44-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7ad44-107">Type</span></span>                      | <span data-ttu-id="7ad44-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7ad44-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="7ad44-109">арность</span><span class="sxs-lookup"><span data-stu-id="7ad44-109">arity</span></span>                       |<span data-ttu-id="7ad44-110">String</span><span class="sxs-lookup"><span data-stu-id="7ad44-110">String</span></span>          |<span data-ttu-id="7ad44-111">Арность оператора.</span><span class="sxs-lookup"><span data-stu-id="7ad44-111">Arity of the operator.</span></span> <span data-ttu-id="7ad44-112">Возможные значения: `Binary`, `Unary`.</span><span class="sxs-lookup"><span data-stu-id="7ad44-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="7ad44-113">Значение по умолчанию — `Binary`.</span><span class="sxs-lookup"><span data-stu-id="7ad44-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="7ad44-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="7ad44-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="7ad44-115">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="7ad44-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="7ad44-116">Возможные значения: `All`, `Any`.</span><span class="sxs-lookup"><span data-stu-id="7ad44-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="7ad44-117">Применяется только к многозначных атрибутов.</span><span class="sxs-lookup"><span data-stu-id="7ad44-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="7ad44-118">`All`означает, что все значения должны соответствовать условие.</span><span class="sxs-lookup"><span data-stu-id="7ad44-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="7ad44-119">`Any`означает, что по крайней мере одно значение должен удовлетворяют условию.</span><span class="sxs-lookup"><span data-stu-id="7ad44-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="7ad44-120">Значение по умолчанию — `All`.</span><span class="sxs-lookup"><span data-stu-id="7ad44-120">The default is `All`.</span></span>|
|<span data-ttu-id="7ad44-121">name</span><span class="sxs-lookup"><span data-stu-id="7ad44-121">name</span></span>                        |<span data-ttu-id="7ad44-122">String</span><span class="sxs-lookup"><span data-stu-id="7ad44-122">String</span></span>                     |<span data-ttu-id="7ad44-123">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="7ad44-123">Operator name.</span></span> |
|<span data-ttu-id="7ad44-124">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="7ad44-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="7ad44-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7ad44-125">String collection</span></span>         |<span data-ttu-id="7ad44-126">Атрибут типы, которые поддерживаются оператором.</span><span class="sxs-lookup"><span data-stu-id="7ad44-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="7ad44-127">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="7ad44-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ad44-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ad44-128">JSON representation</span></span>

<span data-ttu-id="7ad44-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ad44-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "String",
  "multivaluedComparisonType": "String",
  "name": "String",
  "supportedAttributeTypes": ["String"]
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
