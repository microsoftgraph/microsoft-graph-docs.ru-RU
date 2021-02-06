---
title: Тип ресурса filterOperatorSchema
description: Описывает оператор, который можно использовать в фильтре.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 1128b12ffcadd36f2fdd2f34d27f95d973cdfd9d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131889"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="8dd97-103">Тип ресурса filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="8dd97-103">filterOperatorSchema resource type</span></span>

<span data-ttu-id="8dd97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dd97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dd97-105">Описывает оператор, который можно использовать в [фильтре.](synchronization-filter.md)</span><span class="sxs-lookup"><span data-stu-id="8dd97-105">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8dd97-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8dd97-106">Properties</span></span>

| <span data-ttu-id="8dd97-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dd97-107">Property</span></span>                   | <span data-ttu-id="8dd97-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8dd97-108">Type</span></span>                      | <span data-ttu-id="8dd97-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8dd97-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="8dd97-110">arity</span><span class="sxs-lookup"><span data-stu-id="8dd97-110">arity</span></span>                       |<span data-ttu-id="8dd97-111">Строка</span><span class="sxs-lookup"><span data-stu-id="8dd97-111">String</span></span>          |<span data-ttu-id="8dd97-112">Arity of the operator.</span><span class="sxs-lookup"><span data-stu-id="8dd97-112">Arity of the operator.</span></span> <span data-ttu-id="8dd97-113">Возможные значения: `Binary`, `Unary`.</span><span class="sxs-lookup"><span data-stu-id="8dd97-113">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="8dd97-114">Значение по `Binary` умолчанию: .</span><span class="sxs-lookup"><span data-stu-id="8dd97-114">The default is `Binary`.</span></span>|
|<span data-ttu-id="8dd97-115">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="8dd97-115">multivaluedComparisonType</span></span>   |<span data-ttu-id="8dd97-116">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="8dd97-116">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="8dd97-117">Возможные значения: `All`, `Any`.</span><span class="sxs-lookup"><span data-stu-id="8dd97-117">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="8dd97-118">Применяется только к многоценным атрибутам.</span><span class="sxs-lookup"><span data-stu-id="8dd97-118">Applies only to multivalued attributes.</span></span> <span data-ttu-id="8dd97-119">`All` означает, что все значения должны удовлетворять условию.</span><span class="sxs-lookup"><span data-stu-id="8dd97-119">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="8dd97-120">`Any` означает, что условие должно удовлетворять хотя бы одному значению.</span><span class="sxs-lookup"><span data-stu-id="8dd97-120">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="8dd97-121">Значение по `All` умолчанию: .</span><span class="sxs-lookup"><span data-stu-id="8dd97-121">The default is `All`.</span></span>|
|<span data-ttu-id="8dd97-122">name</span><span class="sxs-lookup"><span data-stu-id="8dd97-122">name</span></span>                        |<span data-ttu-id="8dd97-123">String</span><span class="sxs-lookup"><span data-stu-id="8dd97-123">String</span></span>                     |<span data-ttu-id="8dd97-124">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="8dd97-124">Operator name.</span></span> |
|<span data-ttu-id="8dd97-125">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="8dd97-125">supportedAttributeTypes</span></span>     |<span data-ttu-id="8dd97-126">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="8dd97-126">String collection</span></span>         |<span data-ttu-id="8dd97-127">Типы атрибутов, поддерживаемые оператором.</span><span class="sxs-lookup"><span data-stu-id="8dd97-127">Attribute types supported by the operator.</span></span> <span data-ttu-id="8dd97-128">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="8dd97-128">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8dd97-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8dd97-129">JSON representation</span></span>

<span data-ttu-id="8dd97-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8dd97-130">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


