---
title: Тип ресурса Парсикспрессионреспонсе
description: 'Представляет отклик от действия [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) .'
localization_priority: Normal
ms.openlocfilehash: 14fcce13d2e78b99a8712c51768e6a94928fa07f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345560"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="6af54-103">Тип ресурса Парсикспрессионреспонсе</span><span class="sxs-lookup"><span data-stu-id="6af54-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6af54-104">Представляет отклик от действия [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) .</span><span class="sxs-lookup"><span data-stu-id="6af54-104">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="6af54-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6af54-105">Properties</span></span>
| <span data-ttu-id="6af54-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6af54-106">Property</span></span>     | <span data-ttu-id="6af54-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6af54-107">Type</span></span>   |<span data-ttu-id="6af54-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6af54-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6af54-109">error</span><span class="sxs-lookup"><span data-stu-id="6af54-109">error</span></span>|<span data-ttu-id="6af54-110">Публицеррор</span><span class="sxs-lookup"><span data-stu-id="6af54-110">publicError</span></span>|<span data-ttu-id="6af54-111">Сведения об ошибке, если вычисление выражений привело к ошибке.</span><span class="sxs-lookup"><span data-stu-id="6af54-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="6af54-112">Евалуатионресулт</span><span class="sxs-lookup"><span data-stu-id="6af54-112">evaluationResult</span></span>|<span data-ttu-id="6af54-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6af54-113">String collection</span></span>|<span data-ttu-id="6af54-114">Коллекция значений, полученных при оценке выражения.</span><span class="sxs-lookup"><span data-stu-id="6af54-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="6af54-115">Евалуатионсукцеедед</span><span class="sxs-lookup"><span data-stu-id="6af54-115">evaluationSucceeded</span></span>|<span data-ttu-id="6af54-116">Логический</span><span class="sxs-lookup"><span data-stu-id="6af54-116">Boolean</span></span>|<span data-ttu-id="6af54-117">`true`, если оценка выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="6af54-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="6af54-118">Парседекспрессион</span><span class="sxs-lookup"><span data-stu-id="6af54-118">parsedExpression</span></span>|[<span data-ttu-id="6af54-119">Аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="6af54-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="6af54-120">Объект [аттрибутемаппингсаурце](synchronization-attributemappingsource.md) , представляющий проанализированное выражение.</span><span class="sxs-lookup"><span data-stu-id="6af54-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="6af54-121">Парсингсукцеедед</span><span class="sxs-lookup"><span data-stu-id="6af54-121">parsingSucceeded</span></span>|<span data-ttu-id="6af54-122">Логический</span><span class="sxs-lookup"><span data-stu-id="6af54-122">Boolean</span></span>|<span data-ttu-id="6af54-123">`true`, если выражение было успешно проанализировано.</span><span class="sxs-lookup"><span data-stu-id="6af54-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6af54-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6af54-124">JSON representation</span></span>

<span data-ttu-id="6af54-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6af54-125">The following is a JSON representation of the resource.</span></span>

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
