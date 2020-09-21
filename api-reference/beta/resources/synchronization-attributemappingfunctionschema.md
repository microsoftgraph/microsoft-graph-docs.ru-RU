---
title: Тип ресурса Аттрибутемаппингфунктионсчема
description: Описывает функцию, которая может использоваться в сопоставлении атрибутов для преобразования значений во время синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b655d9cfac5835f6887c54c5a6bcbf79887d586
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078082"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="d611d-103">Тип ресурса Аттрибутемаппингфунктионсчема</span><span class="sxs-lookup"><span data-stu-id="d611d-103">attributeMappingFunctionSchema resource type</span></span>

<span data-ttu-id="d611d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d611d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d611d-105">Описывает функцию, которая может использоваться в [сопоставлении атрибутов](synchronization-attributemapping.md) для преобразования значений во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d611d-105">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="d611d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d611d-106">Methods</span></span>

| <span data-ttu-id="d611d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d611d-107">Method</span></span>           | <span data-ttu-id="d611d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d611d-108">Return Type</span></span>    |<span data-ttu-id="d611d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d611d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d611d-110">Список</span><span class="sxs-lookup"><span data-stu-id="d611d-110">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="d611d-111">Коллекция [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="d611d-111">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="d611d-112">Список поддерживаемых функций сопоставления атрибутов.</span><span class="sxs-lookup"><span data-stu-id="d611d-112">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="d611d-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="d611d-113">Properties</span></span>

| <span data-ttu-id="d611d-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="d611d-114">Property</span></span>                   | <span data-ttu-id="d611d-115">Тип</span><span class="sxs-lookup"><span data-stu-id="d611d-115">Type</span></span>                      | <span data-ttu-id="d611d-116">Описание</span><span class="sxs-lookup"><span data-stu-id="d611d-116">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="d611d-117">name</span><span class="sxs-lookup"><span data-stu-id="d611d-117">name</span></span>                        |<span data-ttu-id="d611d-118">String</span><span class="sxs-lookup"><span data-stu-id="d611d-118">String</span></span>                    |<span data-ttu-id="d611d-119">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="d611d-119">Operator name.</span></span> |
|<span data-ttu-id="d611d-120">parameters</span><span class="sxs-lookup"><span data-stu-id="d611d-120">parameters</span></span>                  |<span data-ttu-id="d611d-121">Коллекция [аттрибутемаппингпараметерсчема](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="d611d-121">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="d611d-122">Коллекция параметров функции.</span><span class="sxs-lookup"><span data-stu-id="d611d-122">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d611d-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d611d-123">JSON representation</span></span>

<span data-ttu-id="d611d-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d611d-124">The following is a JSON representation of the resource.</span></span>

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


