---
title: Тип ресурса attributeMappingFunctionSchema
description: Описываются функции, которая может использоваться в Отображение атрибута для преобразования значения во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: 7273534d281d8ea5eaf3709b530776295cd9c767
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822164"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="f50bc-103">Тип ресурса attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="f50bc-103">attributeMappingFunctionSchema resource type</span></span>

> <span data-ttu-id="f50bc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f50bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f50bc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f50bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f50bc-106">Описываются функции, который может использоваться в [сопоставление атрибутов](synchronization-attributemapping.md) для преобразования значения во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f50bc-106">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="f50bc-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f50bc-107">Methods</span></span>

| <span data-ttu-id="f50bc-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f50bc-108">Method</span></span>           | <span data-ttu-id="f50bc-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f50bc-109">Return Type</span></span>    |<span data-ttu-id="f50bc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f50bc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f50bc-111">List</span><span class="sxs-lookup"><span data-stu-id="f50bc-111">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="f50bc-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f50bc-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="f50bc-113">Список поддерживаемых атрибут сопоставления функций.</span><span class="sxs-lookup"><span data-stu-id="f50bc-113">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="f50bc-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="f50bc-114">Properties</span></span>

| <span data-ttu-id="f50bc-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="f50bc-115">Property</span></span>                   | <span data-ttu-id="f50bc-116">Тип</span><span class="sxs-lookup"><span data-stu-id="f50bc-116">Type</span></span>                      | <span data-ttu-id="f50bc-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f50bc-117">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="f50bc-118">name</span><span class="sxs-lookup"><span data-stu-id="f50bc-118">name</span></span>                        |<span data-ttu-id="f50bc-119">Строка</span><span class="sxs-lookup"><span data-stu-id="f50bc-119">String</span></span>                    |<span data-ttu-id="f50bc-120">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="f50bc-120">Operator name.</span></span> |
|<span data-ttu-id="f50bc-121">parameters</span><span class="sxs-lookup"><span data-stu-id="f50bc-121">parameters</span></span>                  |<span data-ttu-id="f50bc-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f50bc-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="f50bc-123">Коллекция параметров функции.</span><span class="sxs-lookup"><span data-stu-id="f50bc-123">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f50bc-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f50bc-124">JSON representation</span></span>

<span data-ttu-id="f50bc-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f50bc-125">The following is a JSON representation of the resource.</span></span>

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
