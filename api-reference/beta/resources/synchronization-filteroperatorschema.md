---
title: Тип ресурса filterOperatorSchema
description: Описывает оператор, который может использоваться в фильтре.
ms.openlocfilehash: 1a4e21aea2b65073a00c9797065f6788a66e2334
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076037"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="ba1d3-103">Тип ресурса filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="ba1d3-103">filterOperatorSchema resource type</span></span>

> <span data-ttu-id="ba1d3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba1d3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba1d3-106">Описывает оператор, который можно использовать в [Фильтр](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="ba1d3-106">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ba1d3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba1d3-107">Properties</span></span>

| <span data-ttu-id="ba1d3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba1d3-108">Property</span></span>                   | <span data-ttu-id="ba1d3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ba1d3-109">Type</span></span>                      | <span data-ttu-id="ba1d3-110">Description</span><span class="sxs-lookup"><span data-stu-id="ba1d3-110">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="ba1d3-111">арность</span><span class="sxs-lookup"><span data-stu-id="ba1d3-111">arity</span></span>                       |<span data-ttu-id="ba1d3-112">String</span><span class="sxs-lookup"><span data-stu-id="ba1d3-112">String</span></span>          |<span data-ttu-id="ba1d3-113">Арность оператора.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-113">Arity of the operator.</span></span> <span data-ttu-id="ba1d3-114">Возможные значения: `Binary`, `Unary`.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-114">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="ba1d3-115">Значение по умолчанию — `Binary`.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-115">The default is `Binary`.</span></span>|
|<span data-ttu-id="ba1d3-116">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="ba1d3-116">multivaluedComparisonType</span></span>   |<span data-ttu-id="ba1d3-117">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="ba1d3-117">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="ba1d3-118">Возможные значения: `All`, `Any`.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-118">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="ba1d3-119">Применяется только к многозначных атрибутов.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-119">Applies only to multivalued attributes.</span></span> <span data-ttu-id="ba1d3-120">`All`означает, что все значения должны соответствовать условие.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-120">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="ba1d3-121">`Any`означает, что по крайней мере одно значение должен удовлетворяют условию.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-121">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="ba1d3-122">Значение по умолчанию — `All`.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-122">The default is `All`.</span></span>|
|<span data-ttu-id="ba1d3-123">name</span><span class="sxs-lookup"><span data-stu-id="ba1d3-123">name</span></span>                        |<span data-ttu-id="ba1d3-124">String</span><span class="sxs-lookup"><span data-stu-id="ba1d3-124">String</span></span>                     |<span data-ttu-id="ba1d3-125">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-125">Operator name.</span></span> |
|<span data-ttu-id="ba1d3-126">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="ba1d3-126">supportedAttributeTypes</span></span>     |<span data-ttu-id="ba1d3-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ba1d3-127">String collection</span></span>         |<span data-ttu-id="ba1d3-128">Атрибут типы, которые поддерживаются оператором.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-128">Attribute types supported by the operator.</span></span> <span data-ttu-id="ba1d3-129">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-129">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba1d3-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba1d3-130">JSON representation</span></span>

<span data-ttu-id="ba1d3-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba1d3-131">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->