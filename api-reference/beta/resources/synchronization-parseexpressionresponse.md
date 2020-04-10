---
title: Тип ресурса Парсикспрессионреспонсе
description: 'Представляет отклик от действия Синчронизатионсчема: Парсикспрессион.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ef96bda8e9e28c655c4bbcf0153ea83ef5b0c8e
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217607"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="ae117-103">Тип ресурса Парсикспрессионреспонсе</span><span class="sxs-lookup"><span data-stu-id="ae117-103">parseExpressionResponse resource type</span></span>

<span data-ttu-id="ae117-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae117-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae117-105">Представляет отклик от действия [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) .</span><span class="sxs-lookup"><span data-stu-id="ae117-105">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="ae117-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae117-106">Properties</span></span>
| <span data-ttu-id="ae117-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae117-107">Property</span></span>     | <span data-ttu-id="ae117-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ae117-108">Type</span></span>   |<span data-ttu-id="ae117-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ae117-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae117-110">error</span><span class="sxs-lookup"><span data-stu-id="ae117-110">error</span></span>|<span data-ttu-id="ae117-111">публицеррор</span><span class="sxs-lookup"><span data-stu-id="ae117-111">publicError</span></span>|<span data-ttu-id="ae117-112">Сведения об ошибке, если вычисление выражений привело к ошибке.</span><span class="sxs-lookup"><span data-stu-id="ae117-112">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="ae117-113">евалуатионресулт</span><span class="sxs-lookup"><span data-stu-id="ae117-113">evaluationResult</span></span>|<span data-ttu-id="ae117-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ae117-114">String collection</span></span>|<span data-ttu-id="ae117-115">Коллекция значений, полученных при оценке выражения.</span><span class="sxs-lookup"><span data-stu-id="ae117-115">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="ae117-116">евалуатионсукцеедед</span><span class="sxs-lookup"><span data-stu-id="ae117-116">evaluationSucceeded</span></span>|<span data-ttu-id="ae117-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae117-117">Boolean</span></span>|<span data-ttu-id="ae117-118">`true`, если оценка выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="ae117-118">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="ae117-119">парседекспрессион</span><span class="sxs-lookup"><span data-stu-id="ae117-119">parsedExpression</span></span>|[<span data-ttu-id="ae117-120">аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="ae117-120">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="ae117-121">Объект [аттрибутемаппингсаурце](synchronization-attributemappingsource.md) , представляющий проанализированное выражение.</span><span class="sxs-lookup"><span data-stu-id="ae117-121">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="ae117-122">парсингсукцеедед</span><span class="sxs-lookup"><span data-stu-id="ae117-122">parsingSucceeded</span></span>|<span data-ttu-id="ae117-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae117-123">Boolean</span></span>|<span data-ttu-id="ae117-124">`true`, если выражение было успешно проанализировано.</span><span class="sxs-lookup"><span data-stu-id="ae117-124">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae117-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae117-125">JSON representation</span></span>

<span data-ttu-id="ae117-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae117-126">The following is a JSON representation of the resource.</span></span>

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
