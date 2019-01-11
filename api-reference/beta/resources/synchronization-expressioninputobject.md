---
title: Тип ресурса expressionInputObject
description: 'Представляет объект для использования в качестве входного тестовых данных при [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие выполняется вычисление выражения.'
localization_priority: Normal
ms.openlocfilehash: acf0fa5125d863224de6df76d46109b9888f8ddf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820113"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="6100f-103">Тип ресурса expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="6100f-103">expressionInputObject resource type</span></span>

> <span data-ttu-id="6100f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6100f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6100f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6100f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6100f-106">Представляет объект для использования в качестве входного тестовых данных при [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие выполняется вычисление выражения.</span><span class="sxs-lookup"><span data-stu-id="6100f-106">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="6100f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6100f-107">Properties</span></span>
| <span data-ttu-id="6100f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6100f-108">Property</span></span>     | <span data-ttu-id="6100f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6100f-109">Type</span></span>   |<span data-ttu-id="6100f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6100f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6100f-111">definition</span><span class="sxs-lookup"><span data-stu-id="6100f-111">definition</span></span>|[<span data-ttu-id="6100f-112">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="6100f-112">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="6100f-113">Определение объекта теста.</span><span class="sxs-lookup"><span data-stu-id="6100f-113">Definition of the test object.</span></span>|
|<span data-ttu-id="6100f-114">свойства</span><span class="sxs-lookup"><span data-stu-id="6100f-114">properties</span></span>|<span data-ttu-id="6100f-115">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6100f-115">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="6100f-116">Значения свойств объекта теста.</span><span class="sxs-lookup"><span data-stu-id="6100f-116">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6100f-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6100f-117">JSON representation</span></span>

<span data-ttu-id="6100f-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6100f-118">The following is a JSON representation of the resource.</span></span>

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
