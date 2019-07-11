---
title: Тип ресурса Аттрибутемаппингфунктионсчема
description: Описывает функцию, которая может использоваться в сопоставлении атрибутов для преобразования значений во время синхронизации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2290f2c3140d9c955dc3a3d4bc72f9b953a7775f
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620285"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="92f59-103">Тип ресурса Аттрибутемаппингфунктионсчема</span><span class="sxs-lookup"><span data-stu-id="92f59-103">attributeMappingFunctionSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92f59-104">Описывает функцию, которая может использоваться в сопоставлении [атрибутов](synchronization-attributemapping.md) для преобразования значений во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="92f59-104">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="92f59-105">Методы</span><span class="sxs-lookup"><span data-stu-id="92f59-105">Methods</span></span>

| <span data-ttu-id="92f59-106">Метод</span><span class="sxs-lookup"><span data-stu-id="92f59-106">Method</span></span>           | <span data-ttu-id="92f59-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="92f59-107">Return Type</span></span>    |<span data-ttu-id="92f59-108">Описание</span><span class="sxs-lookup"><span data-stu-id="92f59-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92f59-109">List</span><span class="sxs-lookup"><span data-stu-id="92f59-109">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="92f59-110">Коллекция [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="92f59-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="92f59-111">Список поддерживаемых функций сопоставления атрибутов.</span><span class="sxs-lookup"><span data-stu-id="92f59-111">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="92f59-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="92f59-112">Properties</span></span>

| <span data-ttu-id="92f59-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="92f59-113">Property</span></span>                   | <span data-ttu-id="92f59-114">Тип</span><span class="sxs-lookup"><span data-stu-id="92f59-114">Type</span></span>                      | <span data-ttu-id="92f59-115">Описание</span><span class="sxs-lookup"><span data-stu-id="92f59-115">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="92f59-116">name</span><span class="sxs-lookup"><span data-stu-id="92f59-116">name</span></span>                        |<span data-ttu-id="92f59-117">String</span><span class="sxs-lookup"><span data-stu-id="92f59-117">String</span></span>                    |<span data-ttu-id="92f59-118">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="92f59-118">Operator name.</span></span> |
|<span data-ttu-id="92f59-119">parameters</span><span class="sxs-lookup"><span data-stu-id="92f59-119">parameters</span></span>                  |<span data-ttu-id="92f59-120">Коллекция [аттрибутемаппингпараметерсчема](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="92f59-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="92f59-121">Коллекция параметров функции.</span><span class="sxs-lookup"><span data-stu-id="92f59-121">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92f59-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92f59-122">JSON representation</span></span>

<span data-ttu-id="92f59-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92f59-123">The following is a JSON representation of the resource.</span></span>

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
