---
title: Тип ресурса parseExpressionResponse
description: 'Представляет ответ от [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие.'
localization_priority: Normal
ms.openlocfilehash: fc37c963e9c9588241d84570edc73a933eec49fc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572880"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="5ec2b-103">Тип ресурса parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="5ec2b-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ec2b-104">Представляет ответ от [synchronizationSchema: parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) действие.</span><span class="sxs-lookup"><span data-stu-id="5ec2b-104">Represents the response from the [synchronizationSchema: parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="5ec2b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ec2b-105">Properties</span></span>
| <span data-ttu-id="5ec2b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ec2b-106">Property</span></span>     | <span data-ttu-id="5ec2b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5ec2b-107">Type</span></span>   |<span data-ttu-id="5ec2b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5ec2b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ec2b-109">error</span><span class="sxs-lookup"><span data-stu-id="5ec2b-109">error</span></span>| <span data-ttu-id="5ec2b-110">publicError</span><span class="sxs-lookup"><span data-stu-id="5ec2b-110">publicError</span></span> |<span data-ttu-id="5ec2b-111">Дополнительные сведения об ошибке, если вычисление выражения возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="5ec2b-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="5ec2b-112">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="5ec2b-112">evaluationResult</span></span>|<span data-ttu-id="5ec2b-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5ec2b-113">String collection</span></span>|<span data-ttu-id="5ec2b-114">Коллекция значений, созданные средством оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="5ec2b-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="5ec2b-115">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="5ec2b-115">evaluationSucceeded</span></span>|<span data-ttu-id="5ec2b-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ec2b-116">Boolean</span></span>|<span data-ttu-id="5ec2b-117">`true`При оценке прошла успешно.</span><span class="sxs-lookup"><span data-stu-id="5ec2b-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="5ec2b-118">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="5ec2b-118">parsedExpression</span></span>|[<span data-ttu-id="5ec2b-119">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="5ec2b-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="5ec2b-120">Объект [attributeMappingSource](synchronization-attributemappingsource.md) , представляющий проанализированного выражения.</span><span class="sxs-lookup"><span data-stu-id="5ec2b-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="5ec2b-121">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="5ec2b-121">parsingSucceeded</span></span>|<span data-ttu-id="5ec2b-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ec2b-122">Boolean</span></span>|<span data-ttu-id="5ec2b-123">`true`Если выражение успешно обработан.</span><span class="sxs-lookup"><span data-stu-id="5ec2b-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ec2b-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ec2b-124">JSON representation</span></span>

<span data-ttu-id="5ec2b-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ec2b-125">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-parseexpressionresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
