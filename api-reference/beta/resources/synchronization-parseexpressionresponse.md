---
title: Тип ресурса Парсикспрессионреспонсе
description: 'Представляет отклик от действия Синчронизатионсчема: Парсикспрессион.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9bd675b079f42856e85f54b7da84a091a0f57f4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988816"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="caaa3-103">Тип ресурса Парсикспрессионреспонсе</span><span class="sxs-lookup"><span data-stu-id="caaa3-103">parseExpressionResponse resource type</span></span>

<span data-ttu-id="caaa3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="caaa3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caaa3-105">Представляет отклик от действия [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) .</span><span class="sxs-lookup"><span data-stu-id="caaa3-105">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="caaa3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="caaa3-106">Properties</span></span>
| <span data-ttu-id="caaa3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="caaa3-107">Property</span></span>     | <span data-ttu-id="caaa3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="caaa3-108">Type</span></span>   |<span data-ttu-id="caaa3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="caaa3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="caaa3-110">error</span><span class="sxs-lookup"><span data-stu-id="caaa3-110">error</span></span>|<span data-ttu-id="caaa3-111">публицеррор</span><span class="sxs-lookup"><span data-stu-id="caaa3-111">publicError</span></span>|<span data-ttu-id="caaa3-112">Сведения об ошибке, если вычисление выражений привело к ошибке.</span><span class="sxs-lookup"><span data-stu-id="caaa3-112">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="caaa3-113">евалуатионресулт</span><span class="sxs-lookup"><span data-stu-id="caaa3-113">evaluationResult</span></span>|<span data-ttu-id="caaa3-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="caaa3-114">String collection</span></span>|<span data-ttu-id="caaa3-115">Коллекция значений, полученных при оценке выражения.</span><span class="sxs-lookup"><span data-stu-id="caaa3-115">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="caaa3-116">евалуатионсукцеедед</span><span class="sxs-lookup"><span data-stu-id="caaa3-116">evaluationSucceeded</span></span>|<span data-ttu-id="caaa3-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="caaa3-117">Boolean</span></span>|<span data-ttu-id="caaa3-118">`true` , если оценка выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="caaa3-118">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="caaa3-119">парседекспрессион</span><span class="sxs-lookup"><span data-stu-id="caaa3-119">parsedExpression</span></span>|[<span data-ttu-id="caaa3-120">аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="caaa3-120">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="caaa3-121">Объект [аттрибутемаппингсаурце](synchronization-attributemappingsource.md) , представляющий проанализированное выражение.</span><span class="sxs-lookup"><span data-stu-id="caaa3-121">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="caaa3-122">парсингсукцеедед</span><span class="sxs-lookup"><span data-stu-id="caaa3-122">parsingSucceeded</span></span>|<span data-ttu-id="caaa3-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="caaa3-123">Boolean</span></span>|<span data-ttu-id="caaa3-124">`true` , если выражение было успешно проанализировано.</span><span class="sxs-lookup"><span data-stu-id="caaa3-124">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="caaa3-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="caaa3-125">JSON representation</span></span>

<span data-ttu-id="caaa3-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="caaa3-126">The following is a JSON representation of the resource.</span></span>

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


