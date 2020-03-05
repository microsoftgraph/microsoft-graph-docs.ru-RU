---
title: Тип ресурса Парсикспрессионреспонсе
description: 'Представляет отклик от действия [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) .'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c752d5c021418dd4a3154a539a61c6ab3bae8a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520137"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="f6a44-103">Тип ресурса Парсикспрессионреспонсе</span><span class="sxs-lookup"><span data-stu-id="f6a44-103">parseExpressionResponse resource type</span></span>

<span data-ttu-id="f6a44-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f6a44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6a44-105">Представляет отклик от действия [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) .</span><span class="sxs-lookup"><span data-stu-id="f6a44-105">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="f6a44-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6a44-106">Properties</span></span>
| <span data-ttu-id="f6a44-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6a44-107">Property</span></span>     | <span data-ttu-id="f6a44-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f6a44-108">Type</span></span>   |<span data-ttu-id="f6a44-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f6a44-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6a44-110">error</span><span class="sxs-lookup"><span data-stu-id="f6a44-110">error</span></span>|<span data-ttu-id="f6a44-111">публицеррор</span><span class="sxs-lookup"><span data-stu-id="f6a44-111">publicError</span></span>|<span data-ttu-id="f6a44-112">Сведения об ошибке, если вычисление выражений привело к ошибке.</span><span class="sxs-lookup"><span data-stu-id="f6a44-112">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="f6a44-113">евалуатионресулт</span><span class="sxs-lookup"><span data-stu-id="f6a44-113">evaluationResult</span></span>|<span data-ttu-id="f6a44-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f6a44-114">String collection</span></span>|<span data-ttu-id="f6a44-115">Коллекция значений, полученных при оценке выражения.</span><span class="sxs-lookup"><span data-stu-id="f6a44-115">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="f6a44-116">евалуатионсукцеедед</span><span class="sxs-lookup"><span data-stu-id="f6a44-116">evaluationSucceeded</span></span>|<span data-ttu-id="f6a44-117">Логический</span><span class="sxs-lookup"><span data-stu-id="f6a44-117">Boolean</span></span>|<span data-ttu-id="f6a44-118">`true`, если оценка выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="f6a44-118">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="f6a44-119">парседекспрессион</span><span class="sxs-lookup"><span data-stu-id="f6a44-119">parsedExpression</span></span>|[<span data-ttu-id="f6a44-120">аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="f6a44-120">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="f6a44-121">Объект [аттрибутемаппингсаурце](synchronization-attributemappingsource.md) , представляющий проанализированное выражение.</span><span class="sxs-lookup"><span data-stu-id="f6a44-121">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="f6a44-122">парсингсукцеедед</span><span class="sxs-lookup"><span data-stu-id="f6a44-122">parsingSucceeded</span></span>|<span data-ttu-id="f6a44-123">Логический</span><span class="sxs-lookup"><span data-stu-id="f6a44-123">Boolean</span></span>|<span data-ttu-id="f6a44-124">`true`, если выражение было успешно проанализировано.</span><span class="sxs-lookup"><span data-stu-id="f6a44-124">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6a44-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6a44-125">JSON representation</span></span>

<span data-ttu-id="f6a44-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6a44-126">The following is a JSON representation of the resource.</span></span>

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
