---
title: Тип ресурса Филтероператорсчема
description: Описывает оператор, который можно использовать в фильтре.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2ed9ef208f888026224293ff86a36b62a3486d48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007895"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="7e18b-103">Тип ресурса Филтероператорсчема</span><span class="sxs-lookup"><span data-stu-id="7e18b-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e18b-104">Описывает оператор, который можно использовать в фильтре [](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="7e18b-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7e18b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e18b-105">Properties</span></span>

| <span data-ttu-id="7e18b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e18b-106">Property</span></span>                   | <span data-ttu-id="7e18b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7e18b-107">Type</span></span>                      | <span data-ttu-id="7e18b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7e18b-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="7e18b-109">равн</span><span class="sxs-lookup"><span data-stu-id="7e18b-109">arity</span></span>                       |<span data-ttu-id="7e18b-110">String</span><span class="sxs-lookup"><span data-stu-id="7e18b-110">String</span></span>          |<span data-ttu-id="7e18b-111">Арность оператора.</span><span class="sxs-lookup"><span data-stu-id="7e18b-111">Arity of the operator.</span></span> <span data-ttu-id="7e18b-112">Возможные значения: `Binary`, `Unary`.</span><span class="sxs-lookup"><span data-stu-id="7e18b-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="7e18b-113">Значение по умолчанию: `Binary`.</span><span class="sxs-lookup"><span data-stu-id="7e18b-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="7e18b-114">Мултивалуедкомпарисонтипе</span><span class="sxs-lookup"><span data-stu-id="7e18b-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="7e18b-115">Скопеоператормултивалуедкомпарисонтипе</span><span class="sxs-lookup"><span data-stu-id="7e18b-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="7e18b-116">Возможные значения: `All`, `Any`.</span><span class="sxs-lookup"><span data-stu-id="7e18b-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="7e18b-117">Применяется только к многозначным атрибутам.</span><span class="sxs-lookup"><span data-stu-id="7e18b-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="7e18b-118">`All`означает, что все значения должны удовлетворять условию.</span><span class="sxs-lookup"><span data-stu-id="7e18b-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="7e18b-119">`Any`Указывает, что по крайней мере одно значение должно удовлетворять условию.</span><span class="sxs-lookup"><span data-stu-id="7e18b-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="7e18b-120">Значение по умолчанию: `All`.</span><span class="sxs-lookup"><span data-stu-id="7e18b-120">The default is `All`.</span></span>|
|<span data-ttu-id="7e18b-121">name</span><span class="sxs-lookup"><span data-stu-id="7e18b-121">name</span></span>                        |<span data-ttu-id="7e18b-122">String</span><span class="sxs-lookup"><span data-stu-id="7e18b-122">String</span></span>                     |<span data-ttu-id="7e18b-123">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="7e18b-123">Operator name.</span></span> |
|<span data-ttu-id="7e18b-124">Суппортедаттрибутетипес</span><span class="sxs-lookup"><span data-stu-id="7e18b-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="7e18b-125">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7e18b-125">String collection</span></span>         |<span data-ttu-id="7e18b-126">Типы атрибутов, поддерживаемые оператором.</span><span class="sxs-lookup"><span data-stu-id="7e18b-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="7e18b-127">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="7e18b-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e18b-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e18b-128">JSON representation</span></span>

<span data-ttu-id="7e18b-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e18b-129">The following is a JSON representation of the resource.</span></span>

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
