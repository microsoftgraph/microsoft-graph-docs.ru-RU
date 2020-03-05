---
title: Тип ресурса Филтероператорсчема
description: Описывает оператор, который можно использовать в фильтре.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 868ecf1e57deb624ab8b276d3f10cd39176efa5b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520172"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="f9666-103">Тип ресурса Филтероператорсчема</span><span class="sxs-lookup"><span data-stu-id="f9666-103">filterOperatorSchema resource type</span></span>

<span data-ttu-id="f9666-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f9666-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9666-105">Описывает оператор, который можно использовать в [фильтре](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="f9666-105">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f9666-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9666-106">Properties</span></span>

| <span data-ttu-id="f9666-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9666-107">Property</span></span>                   | <span data-ttu-id="f9666-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f9666-108">Type</span></span>                      | <span data-ttu-id="f9666-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f9666-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="f9666-110">равн</span><span class="sxs-lookup"><span data-stu-id="f9666-110">arity</span></span>                       |<span data-ttu-id="f9666-111">String</span><span class="sxs-lookup"><span data-stu-id="f9666-111">String</span></span>          |<span data-ttu-id="f9666-112">Арность оператора.</span><span class="sxs-lookup"><span data-stu-id="f9666-112">Arity of the operator.</span></span> <span data-ttu-id="f9666-113">Возможные значения: `Binary`, `Unary`.</span><span class="sxs-lookup"><span data-stu-id="f9666-113">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="f9666-114">Значение по умолчанию: `Binary`.</span><span class="sxs-lookup"><span data-stu-id="f9666-114">The default is `Binary`.</span></span>|
|<span data-ttu-id="f9666-115">мултивалуедкомпарисонтипе</span><span class="sxs-lookup"><span data-stu-id="f9666-115">multivaluedComparisonType</span></span>   |<span data-ttu-id="f9666-116">скопеоператормултивалуедкомпарисонтипе</span><span class="sxs-lookup"><span data-stu-id="f9666-116">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="f9666-117">Возможные значения: `All`, `Any`.</span><span class="sxs-lookup"><span data-stu-id="f9666-117">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="f9666-118">Применяется только к многозначным атрибутам.</span><span class="sxs-lookup"><span data-stu-id="f9666-118">Applies only to multivalued attributes.</span></span> <span data-ttu-id="f9666-119">`All`означает, что все значения должны удовлетворять условию.</span><span class="sxs-lookup"><span data-stu-id="f9666-119">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="f9666-120">`Any`Указывает, что по крайней мере одно значение должно удовлетворять условию.</span><span class="sxs-lookup"><span data-stu-id="f9666-120">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="f9666-121">Значение по умолчанию: `All`.</span><span class="sxs-lookup"><span data-stu-id="f9666-121">The default is `All`.</span></span>|
|<span data-ttu-id="f9666-122">name</span><span class="sxs-lookup"><span data-stu-id="f9666-122">name</span></span>                        |<span data-ttu-id="f9666-123">String</span><span class="sxs-lookup"><span data-stu-id="f9666-123">String</span></span>                     |<span data-ttu-id="f9666-124">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="f9666-124">Operator name.</span></span> |
|<span data-ttu-id="f9666-125">суппортедаттрибутетипес</span><span class="sxs-lookup"><span data-stu-id="f9666-125">supportedAttributeTypes</span></span>     |<span data-ttu-id="f9666-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f9666-126">String collection</span></span>         |<span data-ttu-id="f9666-127">Типы атрибутов, поддерживаемые оператором.</span><span class="sxs-lookup"><span data-stu-id="f9666-127">Attribute types supported by the operator.</span></span> <span data-ttu-id="f9666-128">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="f9666-128">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9666-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9666-129">JSON representation</span></span>

<span data-ttu-id="f9666-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9666-130">The following is a JSON representation of the resource.</span></span>

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
