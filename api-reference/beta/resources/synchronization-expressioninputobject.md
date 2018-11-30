---
title: Тип ресурса expressionInputObject
description: 'Представляет объект для использования в качестве входного тестовых данных при [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие выполняется вычисление выражения.'
ms.openlocfilehash: 06b7344f7e6418db0557f2b12dfa7e964b9d5ab7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081666"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="010d3-103">Тип ресурса expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="010d3-103">expressionInputObject resource type</span></span>

> <span data-ttu-id="010d3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="010d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="010d3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="010d3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="010d3-106">Представляет объект для использования в качестве входного тестовых данных при [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие выполняется вычисление выражения.</span><span class="sxs-lookup"><span data-stu-id="010d3-106">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="010d3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="010d3-107">Properties</span></span>
| <span data-ttu-id="010d3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="010d3-108">Property</span></span>     | <span data-ttu-id="010d3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="010d3-109">Type</span></span>   |<span data-ttu-id="010d3-110">Description</span><span class="sxs-lookup"><span data-stu-id="010d3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="010d3-111">definition</span><span class="sxs-lookup"><span data-stu-id="010d3-111">definition</span></span>|[<span data-ttu-id="010d3-112">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="010d3-112">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="010d3-113">Определение объекта теста.</span><span class="sxs-lookup"><span data-stu-id="010d3-113">Definition of the test object.</span></span>|
|<span data-ttu-id="010d3-114">свойства</span><span class="sxs-lookup"><span data-stu-id="010d3-114">properties</span></span>|<span data-ttu-id="010d3-115">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="010d3-115">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="010d3-116">Значения свойств объекта теста.</span><span class="sxs-lookup"><span data-stu-id="010d3-116">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="010d3-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="010d3-117">JSON representation</span></span>

<span data-ttu-id="010d3-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="010d3-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->