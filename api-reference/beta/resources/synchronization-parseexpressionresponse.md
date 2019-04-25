---
title: Тип ресурса Парсикспрессионреспонсе
description: 'Представляет отклик от действия [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) .'
localization_priority: Normal
ms.openlocfilehash: f8ea708468e1e580693b2bd0e6f0e7f3494996f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523436"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="4cb82-103">Тип ресурса Парсикспрессионреспонсе</span><span class="sxs-lookup"><span data-stu-id="4cb82-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cb82-104">Представляет отклик от действия [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) .</span><span class="sxs-lookup"><span data-stu-id="4cb82-104">Represents the response from the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="4cb82-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4cb82-105">Properties</span></span>
| <span data-ttu-id="4cb82-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cb82-106">Property</span></span>     | <span data-ttu-id="4cb82-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4cb82-107">Type</span></span>   |<span data-ttu-id="4cb82-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4cb82-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cb82-109">error</span><span class="sxs-lookup"><span data-stu-id="4cb82-109">error</span></span>|<span data-ttu-id="4cb82-110">OData. Error</span><span class="sxs-lookup"><span data-stu-id="4cb82-110">odata.error</span></span>|<span data-ttu-id="4cb82-111">Сведения об ошибке, если вычисление выражений привело к ошибке.</span><span class="sxs-lookup"><span data-stu-id="4cb82-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="4cb82-112">Евалуатионресулт</span><span class="sxs-lookup"><span data-stu-id="4cb82-112">evaluationResult</span></span>|<span data-ttu-id="4cb82-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4cb82-113">String collection</span></span>|<span data-ttu-id="4cb82-114">Коллекция значений, полученных при оценке выражения.</span><span class="sxs-lookup"><span data-stu-id="4cb82-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="4cb82-115">Евалуатионсукцеедед</span><span class="sxs-lookup"><span data-stu-id="4cb82-115">evaluationSucceeded</span></span>|<span data-ttu-id="4cb82-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cb82-116">Boolean</span></span>|<span data-ttu-id="4cb82-117">`true`, если оценка выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="4cb82-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="4cb82-118">Парседекспрессион</span><span class="sxs-lookup"><span data-stu-id="4cb82-118">parsedExpression</span></span>|[<span data-ttu-id="4cb82-119">Аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="4cb82-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="4cb82-120">Объект [аттрибутемаппингсаурце](synchronization-attributemappingsource.md) , представляющий проанализированное выражение.</span><span class="sxs-lookup"><span data-stu-id="4cb82-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="4cb82-121">Парсингсукцеедед</span><span class="sxs-lookup"><span data-stu-id="4cb82-121">parsingSucceeded</span></span>|<span data-ttu-id="4cb82-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cb82-122">Boolean</span></span>|<span data-ttu-id="4cb82-123">`true`, если выражение было успешно проанализировано.</span><span class="sxs-lookup"><span data-stu-id="4cb82-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4cb82-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4cb82-124">JSON representation</span></span>

<span data-ttu-id="4cb82-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cb82-125">The following is a JSON representation of the resource.</span></span>

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
