---
title: Тип ресурса expressionInputObject
description: 'Представляет объект для использования в качестве входного тестовых данных при [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие выполняется вычисление выражения.'
localization_priority: Normal
ms.openlocfilehash: 4f0ba06651fdd8a296b0939d05ecefe996f0089f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570962"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="8cf36-103">Тип ресурса expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="8cf36-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cf36-104">Представляет объект для использования в качестве входного тестовых данных при [synchronizationSchema: parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) действие выполняется вычисление выражения.</span><span class="sxs-lookup"><span data-stu-id="8cf36-104">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="8cf36-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cf36-105">Properties</span></span>
| <span data-ttu-id="8cf36-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cf36-106">Property</span></span>     | <span data-ttu-id="8cf36-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8cf36-107">Type</span></span>   |<span data-ttu-id="8cf36-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8cf36-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cf36-109">definition</span><span class="sxs-lookup"><span data-stu-id="8cf36-109">definition</span></span>|[<span data-ttu-id="8cf36-110">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="8cf36-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="8cf36-111">Определение объекта теста.</span><span class="sxs-lookup"><span data-stu-id="8cf36-111">Definition of the test object.</span></span>|
|<span data-ttu-id="8cf36-112">properties</span><span class="sxs-lookup"><span data-stu-id="8cf36-112">properties</span></span>|<span data-ttu-id="8cf36-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8cf36-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="8cf36-114">Значения свойств объекта теста.</span><span class="sxs-lookup"><span data-stu-id="8cf36-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cf36-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cf36-115">JSON representation</span></span>

<span data-ttu-id="8cf36-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cf36-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-expressioninputobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
