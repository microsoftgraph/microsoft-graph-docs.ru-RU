---
title: Тип ресурса Аттрибутемаппингфунктионсчема
description: Описывает функцию, которая может использоваться в сопоставлении атрибутов для преобразования значений во время синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 16dae5dca65b3d238c2d12fddc2b474e7e03ac0d
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219181"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="16593-103">Тип ресурса Аттрибутемаппингфунктионсчема</span><span class="sxs-lookup"><span data-stu-id="16593-103">attributeMappingFunctionSchema resource type</span></span>

<span data-ttu-id="16593-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16593-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16593-105">Описывает функцию, которая может использоваться в [сопоставлении атрибутов](synchronization-attributemapping.md) для преобразования значений во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="16593-105">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="16593-106">Методы</span><span class="sxs-lookup"><span data-stu-id="16593-106">Methods</span></span>

| <span data-ttu-id="16593-107">Метод</span><span class="sxs-lookup"><span data-stu-id="16593-107">Method</span></span>           | <span data-ttu-id="16593-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="16593-108">Return Type</span></span>    |<span data-ttu-id="16593-109">Описание</span><span class="sxs-lookup"><span data-stu-id="16593-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16593-110">List</span><span class="sxs-lookup"><span data-stu-id="16593-110">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="16593-111">Коллекция [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="16593-111">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="16593-112">Список поддерживаемых функций сопоставления атрибутов.</span><span class="sxs-lookup"><span data-stu-id="16593-112">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="16593-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="16593-113">Properties</span></span>

| <span data-ttu-id="16593-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="16593-114">Property</span></span>                   | <span data-ttu-id="16593-115">Тип</span><span class="sxs-lookup"><span data-stu-id="16593-115">Type</span></span>                      | <span data-ttu-id="16593-116">Описание</span><span class="sxs-lookup"><span data-stu-id="16593-116">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="16593-117">name</span><span class="sxs-lookup"><span data-stu-id="16593-117">name</span></span>                        |<span data-ttu-id="16593-118">String</span><span class="sxs-lookup"><span data-stu-id="16593-118">String</span></span>                    |<span data-ttu-id="16593-119">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="16593-119">Operator name.</span></span> |
|<span data-ttu-id="16593-120">parameters</span><span class="sxs-lookup"><span data-stu-id="16593-120">parameters</span></span>                  |<span data-ttu-id="16593-121">Коллекция [аттрибутемаппингпараметерсчема](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="16593-121">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="16593-122">Коллекция параметров функции.</span><span class="sxs-lookup"><span data-stu-id="16593-122">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16593-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16593-123">JSON representation</span></span>

<span data-ttu-id="16593-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16593-124">The following is a JSON representation of the resource.</span></span>

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
