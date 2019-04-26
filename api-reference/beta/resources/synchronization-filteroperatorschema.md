---
title: Тип ресурса Филтероператорсчема
description: Описывает оператор, который можно использовать в фильтре.
localization_priority: Normal
ms.openlocfilehash: 0f0ada4aaa02efa2484ffa75d88b2c8256f15fe8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342867"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="179f8-103">Тип ресурса Филтероператорсчема</span><span class="sxs-lookup"><span data-stu-id="179f8-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="179f8-104">Описывает оператор, который можно использовать в фильтре [](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="179f8-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="179f8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="179f8-105">Properties</span></span>

| <span data-ttu-id="179f8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="179f8-106">Property</span></span>                   | <span data-ttu-id="179f8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="179f8-107">Type</span></span>                      | <span data-ttu-id="179f8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="179f8-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="179f8-109">равн</span><span class="sxs-lookup"><span data-stu-id="179f8-109">arity</span></span>                       |<span data-ttu-id="179f8-110">String</span><span class="sxs-lookup"><span data-stu-id="179f8-110">String</span></span>          |<span data-ttu-id="179f8-111">Арность оператора.</span><span class="sxs-lookup"><span data-stu-id="179f8-111">Arity of the operator.</span></span> <span data-ttu-id="179f8-112">Возможные значения: `Binary`, `Unary`.</span><span class="sxs-lookup"><span data-stu-id="179f8-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="179f8-113">Значение по умолчанию: `Binary`.</span><span class="sxs-lookup"><span data-stu-id="179f8-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="179f8-114">Мултивалуедкомпарисонтипе</span><span class="sxs-lookup"><span data-stu-id="179f8-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="179f8-115">Скопеоператормултивалуедкомпарисонтипе</span><span class="sxs-lookup"><span data-stu-id="179f8-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="179f8-116">Возможные значения: `All`, `Any`.</span><span class="sxs-lookup"><span data-stu-id="179f8-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="179f8-117">Применяется только к многозначным атрибутам.</span><span class="sxs-lookup"><span data-stu-id="179f8-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="179f8-118">`All`означает, что все значения должны удовлетворять условию.</span><span class="sxs-lookup"><span data-stu-id="179f8-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="179f8-119">`Any`Указывает, что по крайней мере одно значение должно удовлетворять условию.</span><span class="sxs-lookup"><span data-stu-id="179f8-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="179f8-120">Значение по умолчанию: `All`.</span><span class="sxs-lookup"><span data-stu-id="179f8-120">The default is `All`.</span></span>|
|<span data-ttu-id="179f8-121">name</span><span class="sxs-lookup"><span data-stu-id="179f8-121">name</span></span>                        |<span data-ttu-id="179f8-122">String</span><span class="sxs-lookup"><span data-stu-id="179f8-122">String</span></span>                     |<span data-ttu-id="179f8-123">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="179f8-123">Operator name.</span></span> |
|<span data-ttu-id="179f8-124">Суппортедаттрибутетипес</span><span class="sxs-lookup"><span data-stu-id="179f8-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="179f8-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="179f8-125">String collection</span></span>         |<span data-ttu-id="179f8-126">Типы атрибутов, поддерживаемые оператором.</span><span class="sxs-lookup"><span data-stu-id="179f8-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="179f8-127">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="179f8-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="179f8-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="179f8-128">JSON representation</span></span>

<span data-ttu-id="179f8-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="179f8-129">The following is a JSON representation of the resource.</span></span>

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
