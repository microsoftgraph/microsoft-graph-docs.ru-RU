---
title: Тип ресурса Филтероператорсчема
description: Описывает оператор, который можно использовать в фильтре.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 694af6455cc7b2dbf1f6f6ae811713b5b9d61265
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079699"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="2f488-103">Тип ресурса Филтероператорсчема</span><span class="sxs-lookup"><span data-stu-id="2f488-103">filterOperatorSchema resource type</span></span>

<span data-ttu-id="2f488-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f488-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f488-105">Описывает оператор, который можно использовать в [фильтре](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="2f488-105">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2f488-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f488-106">Properties</span></span>

| <span data-ttu-id="2f488-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f488-107">Property</span></span>                   | <span data-ttu-id="2f488-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2f488-108">Type</span></span>                      | <span data-ttu-id="2f488-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2f488-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="2f488-110">равн</span><span class="sxs-lookup"><span data-stu-id="2f488-110">arity</span></span>                       |<span data-ttu-id="2f488-111">String</span><span class="sxs-lookup"><span data-stu-id="2f488-111">String</span></span>          |<span data-ttu-id="2f488-112">Арность оператора.</span><span class="sxs-lookup"><span data-stu-id="2f488-112">Arity of the operator.</span></span> <span data-ttu-id="2f488-113">Возможные значения: `Binary`, `Unary`.</span><span class="sxs-lookup"><span data-stu-id="2f488-113">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="2f488-114">Значение по умолчанию: `Binary` .</span><span class="sxs-lookup"><span data-stu-id="2f488-114">The default is `Binary`.</span></span>|
|<span data-ttu-id="2f488-115">мултивалуедкомпарисонтипе</span><span class="sxs-lookup"><span data-stu-id="2f488-115">multivaluedComparisonType</span></span>   |<span data-ttu-id="2f488-116">скопеоператормултивалуедкомпарисонтипе</span><span class="sxs-lookup"><span data-stu-id="2f488-116">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="2f488-117">Возможные значения: `All`, `Any`.</span><span class="sxs-lookup"><span data-stu-id="2f488-117">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="2f488-118">Применяется только к многозначным атрибутам.</span><span class="sxs-lookup"><span data-stu-id="2f488-118">Applies only to multivalued attributes.</span></span> <span data-ttu-id="2f488-119">`All` означает, что все значения должны удовлетворять условию.</span><span class="sxs-lookup"><span data-stu-id="2f488-119">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="2f488-120">`Any` Указывает, что по крайней мере одно значение должно удовлетворять условию.</span><span class="sxs-lookup"><span data-stu-id="2f488-120">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="2f488-121">Значение по умолчанию: `All` .</span><span class="sxs-lookup"><span data-stu-id="2f488-121">The default is `All`.</span></span>|
|<span data-ttu-id="2f488-122">name</span><span class="sxs-lookup"><span data-stu-id="2f488-122">name</span></span>                        |<span data-ttu-id="2f488-123">String</span><span class="sxs-lookup"><span data-stu-id="2f488-123">String</span></span>                     |<span data-ttu-id="2f488-124">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="2f488-124">Operator name.</span></span> |
|<span data-ttu-id="2f488-125">суппортедаттрибутетипес</span><span class="sxs-lookup"><span data-stu-id="2f488-125">supportedAttributeTypes</span></span>     |<span data-ttu-id="2f488-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2f488-126">String collection</span></span>         |<span data-ttu-id="2f488-127">Типы атрибутов, поддерживаемые оператором.</span><span class="sxs-lookup"><span data-stu-id="2f488-127">Attribute types supported by the operator.</span></span> <span data-ttu-id="2f488-128">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="2f488-128">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f488-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f488-129">JSON representation</span></span>

<span data-ttu-id="2f488-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f488-130">The following is a JSON representation of the resource.</span></span>

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


