---
title: Тип ресурса attributeMappingFunctionSchema
description: Описываются функции, которая может использоваться в Отображение атрибута для преобразования значения во время синхронизации.
ms.openlocfilehash: 9760669bb29700bfa79c1cd375857b4fd673879b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078710"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="50113-103">Тип ресурса attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="50113-103">attributeMappingFunctionSchema resource type</span></span>

> <span data-ttu-id="50113-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="50113-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50113-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50113-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50113-106">Описываются функции, который может использоваться в [сопоставление атрибутов](synchronization-attributemapping.md) для преобразования значения во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="50113-106">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="50113-107">Методы</span><span class="sxs-lookup"><span data-stu-id="50113-107">Methods</span></span>

| <span data-ttu-id="50113-108">Метод</span><span class="sxs-lookup"><span data-stu-id="50113-108">Method</span></span>           | <span data-ttu-id="50113-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="50113-109">Return Type</span></span>    |<span data-ttu-id="50113-110">Описание</span><span class="sxs-lookup"><span data-stu-id="50113-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50113-111">List</span><span class="sxs-lookup"><span data-stu-id="50113-111">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="50113-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="50113-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="50113-113">Список поддерживаемых атрибут сопоставления функций.</span><span class="sxs-lookup"><span data-stu-id="50113-113">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="50113-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="50113-114">Properties</span></span>

| <span data-ttu-id="50113-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="50113-115">Property</span></span>                   | <span data-ttu-id="50113-116">Тип</span><span class="sxs-lookup"><span data-stu-id="50113-116">Type</span></span>                      | <span data-ttu-id="50113-117">Описание</span><span class="sxs-lookup"><span data-stu-id="50113-117">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="50113-118">name</span><span class="sxs-lookup"><span data-stu-id="50113-118">name</span></span>                        |<span data-ttu-id="50113-119">String</span><span class="sxs-lookup"><span data-stu-id="50113-119">String</span></span>                    |<span data-ttu-id="50113-120">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="50113-120">Operator name.</span></span> |
|<span data-ttu-id="50113-121">parameters</span><span class="sxs-lookup"><span data-stu-id="50113-121">parameters</span></span>                  |<span data-ttu-id="50113-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="50113-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="50113-123">Коллекция параметров функции.</span><span class="sxs-lookup"><span data-stu-id="50113-123">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50113-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50113-124">JSON representation</span></span>

<span data-ttu-id="50113-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50113-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}-->

```json
{
  "name": "String (identifier)",
  "parameters": [{"@odata.type": "microsoft.graph.attributeMappingParameterSchema"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->