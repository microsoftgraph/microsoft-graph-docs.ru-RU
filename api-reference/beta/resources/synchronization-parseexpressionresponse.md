---
title: Тип ресурса parseExpressionResponse
description: 'Представляет ответ от действия synchronizationSchema: parseExpression.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: e564cb2ad7a80c91fec7d6298254fa19bde4537c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133149"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="9f9df-103">Тип ресурса parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="9f9df-103">parseExpressionResponse resource type</span></span>

<span data-ttu-id="9f9df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f9df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f9df-105">Представляет ответ от действия [parseExpression.](../api/synchronization-synchronizationschema-parseexpression.md)</span><span class="sxs-lookup"><span data-stu-id="9f9df-105">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="9f9df-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f9df-106">Properties</span></span>
| <span data-ttu-id="9f9df-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f9df-107">Property</span></span>     | <span data-ttu-id="9f9df-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9f9df-108">Type</span></span>   |<span data-ttu-id="9f9df-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9f9df-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f9df-110">error</span><span class="sxs-lookup"><span data-stu-id="9f9df-110">error</span></span>|<span data-ttu-id="9f9df-111">publicError</span><span class="sxs-lookup"><span data-stu-id="9f9df-111">publicError</span></span>|<span data-ttu-id="9f9df-112">Сведения об ошибке, если оценка выражения приводит к ошибке.</span><span class="sxs-lookup"><span data-stu-id="9f9df-112">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="9f9df-113">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="9f9df-113">evaluationResult</span></span>|<span data-ttu-id="9f9df-114">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="9f9df-114">String collection</span></span>|<span data-ttu-id="9f9df-115">Коллекция значений, производимых при оценке выражения.</span><span class="sxs-lookup"><span data-stu-id="9f9df-115">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="9f9df-116">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="9f9df-116">evaluationSucceeded</span></span>|<span data-ttu-id="9f9df-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f9df-117">Boolean</span></span>|<span data-ttu-id="9f9df-118">`true` если оценка прошла успешно.</span><span class="sxs-lookup"><span data-stu-id="9f9df-118">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="9f9df-119">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="9f9df-119">parsedExpression</span></span>|[<span data-ttu-id="9f9df-120">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="9f9df-120">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="9f9df-121">Объект [attributeMappingSource,](synchronization-attributemappingsource.md) представляющий выражение с разчетом.</span><span class="sxs-lookup"><span data-stu-id="9f9df-121">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="9f9df-122">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="9f9df-122">parsingSucceeded</span></span>|<span data-ttu-id="9f9df-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f9df-123">Boolean</span></span>|<span data-ttu-id="9f9df-124">`true` если выражение было успешно разлино.</span><span class="sxs-lookup"><span data-stu-id="9f9df-124">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f9df-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9f9df-125">JSON representation</span></span>

<span data-ttu-id="9f9df-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f9df-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parseExpressionResponse"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.publicError"},
  "evaluationResult": ["String"],
  "evaluationSucceeded": true,
  "parsedExpression": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "parsingSucceeded": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


