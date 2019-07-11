---
title: Тип ресурса Парсикспрессионреспонсе
description: 'Представляет отклик от действия [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) .'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d63a8834640d357e41051750f7f2cd50b8724fee
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620488"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="d4c65-103">Тип ресурса Парсикспрессионреспонсе</span><span class="sxs-lookup"><span data-stu-id="d4c65-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4c65-104">Представляет отклик от действия [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) .</span><span class="sxs-lookup"><span data-stu-id="d4c65-104">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="d4c65-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4c65-105">Properties</span></span>
| <span data-ttu-id="d4c65-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4c65-106">Property</span></span>     | <span data-ttu-id="d4c65-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d4c65-107">Type</span></span>   |<span data-ttu-id="d4c65-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d4c65-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4c65-109">error</span><span class="sxs-lookup"><span data-stu-id="d4c65-109">error</span></span>|<span data-ttu-id="d4c65-110">Публицеррор</span><span class="sxs-lookup"><span data-stu-id="d4c65-110">publicError</span></span>|<span data-ttu-id="d4c65-111">Сведения об ошибке, если вычисление выражений привело к ошибке.</span><span class="sxs-lookup"><span data-stu-id="d4c65-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="d4c65-112">Евалуатионресулт</span><span class="sxs-lookup"><span data-stu-id="d4c65-112">evaluationResult</span></span>|<span data-ttu-id="d4c65-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d4c65-113">String collection</span></span>|<span data-ttu-id="d4c65-114">Коллекция значений, полученных при оценке выражения.</span><span class="sxs-lookup"><span data-stu-id="d4c65-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="d4c65-115">Евалуатионсукцеедед</span><span class="sxs-lookup"><span data-stu-id="d4c65-115">evaluationSucceeded</span></span>|<span data-ttu-id="d4c65-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4c65-116">Boolean</span></span>|<span data-ttu-id="d4c65-117">`true`, если оценка выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="d4c65-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="d4c65-118">Парседекспрессион</span><span class="sxs-lookup"><span data-stu-id="d4c65-118">parsedExpression</span></span>|[<span data-ttu-id="d4c65-119">Аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="d4c65-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="d4c65-120">Объект [аттрибутемаппингсаурце](synchronization-attributemappingsource.md) , представляющий проанализированное выражение.</span><span class="sxs-lookup"><span data-stu-id="d4c65-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="d4c65-121">Парсингсукцеедед</span><span class="sxs-lookup"><span data-stu-id="d4c65-121">parsingSucceeded</span></span>|<span data-ttu-id="d4c65-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4c65-122">Boolean</span></span>|<span data-ttu-id="d4c65-123">`true`, если выражение было успешно проанализировано.</span><span class="sxs-lookup"><span data-stu-id="d4c65-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4c65-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4c65-124">JSON representation</span></span>

<span data-ttu-id="d4c65-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4c65-125">The following is a JSON representation of the resource.</span></span>

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
