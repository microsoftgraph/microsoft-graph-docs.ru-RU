---
title: Тип ресурса Аттрибутемаппингфунктионсчема
description: Описывает функцию, которая может использоваться в сопоставлении атрибутов для преобразования значений во время синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0222a01f2bcea819624d1dcb9f53da7ea0b86b25
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007993"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="b3ef4-103">Тип ресурса Аттрибутемаппингфунктионсчема</span><span class="sxs-lookup"><span data-stu-id="b3ef4-103">attributeMappingFunctionSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3ef4-104">Описывает функцию, которая может использоваться в сопоставлении [атрибутов](synchronization-attributemapping.md) для преобразования значений во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b3ef4-104">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="b3ef4-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b3ef4-105">Methods</span></span>

| <span data-ttu-id="b3ef4-106">Метод</span><span class="sxs-lookup"><span data-stu-id="b3ef4-106">Method</span></span>           | <span data-ttu-id="b3ef4-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b3ef4-107">Return Type</span></span>    |<span data-ttu-id="b3ef4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b3ef4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b3ef4-109">List</span><span class="sxs-lookup"><span data-stu-id="b3ef4-109">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="b3ef4-110">Коллекция [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="b3ef4-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="b3ef4-111">Список поддерживаемых функций сопоставления атрибутов.</span><span class="sxs-lookup"><span data-stu-id="b3ef4-111">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3ef4-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3ef4-112">Properties</span></span>

| <span data-ttu-id="b3ef4-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3ef4-113">Property</span></span>                   | <span data-ttu-id="b3ef4-114">Тип</span><span class="sxs-lookup"><span data-stu-id="b3ef4-114">Type</span></span>                      | <span data-ttu-id="b3ef4-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b3ef4-115">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="b3ef4-116">name</span><span class="sxs-lookup"><span data-stu-id="b3ef4-116">name</span></span>                        |<span data-ttu-id="b3ef4-117">String</span><span class="sxs-lookup"><span data-stu-id="b3ef4-117">String</span></span>                    |<span data-ttu-id="b3ef4-118">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="b3ef4-118">Operator name.</span></span> |
|<span data-ttu-id="b3ef4-119">parameters</span><span class="sxs-lookup"><span data-stu-id="b3ef4-119">parameters</span></span>                  |<span data-ttu-id="b3ef4-120">Коллекция [аттрибутемаппингпараметерсчема](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="b3ef4-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="b3ef4-121">Коллекция параметров функции.</span><span class="sxs-lookup"><span data-stu-id="b3ef4-121">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3ef4-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3ef4-122">JSON representation</span></span>

<span data-ttu-id="b3ef4-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3ef4-123">The following is a JSON representation of the resource.</span></span>

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
