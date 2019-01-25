---
title: Тип ресурса filterOperatorSchema
description: Описывает оператор, который может использоваться в фильтре.
localization_priority: Normal
ms.openlocfilehash: 04bee90f81c0098832cd4b6355be266668d0f69b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515197"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="f47f0-103">Тип ресурса filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="f47f0-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f47f0-104">Описывает оператор, который можно использовать в [Фильтр](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="f47f0-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f47f0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f47f0-105">Properties</span></span>

| <span data-ttu-id="f47f0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f47f0-106">Property</span></span>                   | <span data-ttu-id="f47f0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f47f0-107">Type</span></span>                      | <span data-ttu-id="f47f0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f47f0-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="f47f0-109">арность</span><span class="sxs-lookup"><span data-stu-id="f47f0-109">arity</span></span>                       |<span data-ttu-id="f47f0-110">String</span><span class="sxs-lookup"><span data-stu-id="f47f0-110">String</span></span>          |<span data-ttu-id="f47f0-111">Арность оператора.</span><span class="sxs-lookup"><span data-stu-id="f47f0-111">Arity of the operator.</span></span> <span data-ttu-id="f47f0-112">Возможные значения: `Binary`, `Unary`.</span><span class="sxs-lookup"><span data-stu-id="f47f0-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="f47f0-113">Значение по умолчанию — `Binary`.</span><span class="sxs-lookup"><span data-stu-id="f47f0-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="f47f0-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="f47f0-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="f47f0-115">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="f47f0-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="f47f0-116">Возможные значения: `All`, `Any`.</span><span class="sxs-lookup"><span data-stu-id="f47f0-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="f47f0-117">Применяется только к многозначных атрибутов.</span><span class="sxs-lookup"><span data-stu-id="f47f0-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="f47f0-118">`All`означает, что все значения должны соответствовать условие.</span><span class="sxs-lookup"><span data-stu-id="f47f0-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="f47f0-119">`Any`означает, что по крайней мере одно значение должен удовлетворяют условию.</span><span class="sxs-lookup"><span data-stu-id="f47f0-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="f47f0-120">Значение по умолчанию — `All`.</span><span class="sxs-lookup"><span data-stu-id="f47f0-120">The default is `All`.</span></span>|
|<span data-ttu-id="f47f0-121">name</span><span class="sxs-lookup"><span data-stu-id="f47f0-121">name</span></span>                        |<span data-ttu-id="f47f0-122">String</span><span class="sxs-lookup"><span data-stu-id="f47f0-122">String</span></span>                     |<span data-ttu-id="f47f0-123">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="f47f0-123">Operator name.</span></span> |
|<span data-ttu-id="f47f0-124">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="f47f0-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="f47f0-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f47f0-125">String collection</span></span>         |<span data-ttu-id="f47f0-126">Атрибут типы, которые поддерживаются оператором.</span><span class="sxs-lookup"><span data-stu-id="f47f0-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="f47f0-127">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="f47f0-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f47f0-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f47f0-128">JSON representation</span></span>

<span data-ttu-id="f47f0-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f47f0-129">The following is a JSON representation of the resource.</span></span>

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
