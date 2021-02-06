---
title: Тип ресурса attributeMappingFunctionSchema
description: Описывает функцию, которую можно использовать в сопоставлении атрибутов для преобразования значений во время синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a62d2d635504208fc8266e98add66a8503e3e4d2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128745"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="f11db-103">Тип ресурса attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="f11db-103">attributeMappingFunctionSchema resource type</span></span>

<span data-ttu-id="f11db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f11db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f11db-105">Описывает функцию, которую можно использовать в сопоставлении [атрибутов](synchronization-attributemapping.md) для преобразования значений во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f11db-105">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="f11db-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f11db-106">Methods</span></span>

| <span data-ttu-id="f11db-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f11db-107">Method</span></span>           | <span data-ttu-id="f11db-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f11db-108">Return Type</span></span>    |<span data-ttu-id="f11db-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f11db-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f11db-110">Список</span><span class="sxs-lookup"><span data-stu-id="f11db-110">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="f11db-111">[Коллекция attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="f11db-111">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="f11db-112">Список поддерживаемых функций сопоставления атрибутов.</span><span class="sxs-lookup"><span data-stu-id="f11db-112">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="f11db-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="f11db-113">Properties</span></span>

| <span data-ttu-id="f11db-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="f11db-114">Property</span></span>                   | <span data-ttu-id="f11db-115">Тип</span><span class="sxs-lookup"><span data-stu-id="f11db-115">Type</span></span>                      | <span data-ttu-id="f11db-116">Описание</span><span class="sxs-lookup"><span data-stu-id="f11db-116">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="f11db-117">name</span><span class="sxs-lookup"><span data-stu-id="f11db-117">name</span></span>                        |<span data-ttu-id="f11db-118">String</span><span class="sxs-lookup"><span data-stu-id="f11db-118">String</span></span>                    |<span data-ttu-id="f11db-119">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="f11db-119">Operator name.</span></span> |
|<span data-ttu-id="f11db-120">parameters</span><span class="sxs-lookup"><span data-stu-id="f11db-120">parameters</span></span>                  |<span data-ttu-id="f11db-121">[Коллекция attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="f11db-121">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="f11db-122">Коллекция параметров функций.</span><span class="sxs-lookup"><span data-stu-id="f11db-122">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f11db-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f11db-123">JSON representation</span></span>

<span data-ttu-id="f11db-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f11db-124">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


