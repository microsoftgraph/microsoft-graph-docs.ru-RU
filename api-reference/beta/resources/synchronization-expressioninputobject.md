---
title: Тип ресурса expressionInputObject
description: Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие synchronizationSchema parseExpression выполняет оценку выражения.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 161589d9d8b6e3d06ef6afe31df0fde79bf938bb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132050"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="5e54f-103">Тип ресурса expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="5e54f-103">expressionInputObject resource type</span></span>

<span data-ttu-id="5e54f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e54f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e54f-105">Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) выполняет оценку выражения.</span><span class="sxs-lookup"><span data-stu-id="5e54f-105">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="5e54f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e54f-106">Properties</span></span>
| <span data-ttu-id="5e54f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e54f-107">Property</span></span>     | <span data-ttu-id="5e54f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5e54f-108">Type</span></span>   |<span data-ttu-id="5e54f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5e54f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e54f-110">definition</span><span class="sxs-lookup"><span data-stu-id="5e54f-110">definition</span></span>|[<span data-ttu-id="5e54f-111">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="5e54f-111">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="5e54f-112">Определение тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="5e54f-112">Definition of the test object.</span></span>|
|<span data-ttu-id="5e54f-113">properties</span><span class="sxs-lookup"><span data-stu-id="5e54f-113">properties</span></span>|<span data-ttu-id="5e54f-114">[Коллекция stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5e54f-114">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="5e54f-115">Значения свойств тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="5e54f-115">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e54f-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5e54f-116">JSON representation</span></span>

<span data-ttu-id="5e54f-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e54f-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


