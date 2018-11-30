---
title: Тип ресурса parseExpressionResponse
description: 'Представляет ответ от [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие.'
ms.openlocfilehash: 625df0ca16135eaa35c5b679c79dea582c4012e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081858"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="ad7ee-103">Тип ресурса parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="ad7ee-103">parseExpressionResponse resource type</span></span>

> <span data-ttu-id="ad7ee-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad7ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad7ee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad7ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad7ee-106">Представляет ответ от [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие.</span><span class="sxs-lookup"><span data-stu-id="ad7ee-106">Represents the response from the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="ad7ee-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad7ee-107">Properties</span></span>
| <span data-ttu-id="ad7ee-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad7ee-108">Property</span></span>     | <span data-ttu-id="ad7ee-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ad7ee-109">Type</span></span>   |<span data-ttu-id="ad7ee-110">Description</span><span class="sxs-lookup"><span data-stu-id="ad7ee-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad7ee-111">error</span><span class="sxs-lookup"><span data-stu-id="ad7ee-111">error</span></span>|<span data-ttu-id="ad7ee-112">OData.Error</span><span class="sxs-lookup"><span data-stu-id="ad7ee-112">odata.error</span></span>|<span data-ttu-id="ad7ee-113">Дополнительные сведения об ошибке, если вычисление выражения возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="ad7ee-113">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="ad7ee-114">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="ad7ee-114">evaluationResult</span></span>|<span data-ttu-id="ad7ee-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ad7ee-115">String collection</span></span>|<span data-ttu-id="ad7ee-116">Коллекция значений, созданные средством оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="ad7ee-116">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="ad7ee-117">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="ad7ee-117">evaluationSucceeded</span></span>|<span data-ttu-id="ad7ee-118">Логический</span><span class="sxs-lookup"><span data-stu-id="ad7ee-118">Boolean</span></span>|<span data-ttu-id="ad7ee-119">`true`При оценке прошла успешно.</span><span class="sxs-lookup"><span data-stu-id="ad7ee-119">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="ad7ee-120">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="ad7ee-120">parsedExpression</span></span>|[<span data-ttu-id="ad7ee-121">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="ad7ee-121">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="ad7ee-122">Объект [attributeMappingSource](synchronization-attributemappingsource.md) , представляющий проанализированного выражения.</span><span class="sxs-lookup"><span data-stu-id="ad7ee-122">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="ad7ee-123">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="ad7ee-123">parsingSucceeded</span></span>|<span data-ttu-id="ad7ee-124">Логический</span><span class="sxs-lookup"><span data-stu-id="ad7ee-124">Boolean</span></span>|<span data-ttu-id="ad7ee-125">`true`Если выражение успешно обработан.</span><span class="sxs-lookup"><span data-stu-id="ad7ee-125">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad7ee-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad7ee-126">JSON representation</span></span>

<span data-ttu-id="ad7ee-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad7ee-127">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->