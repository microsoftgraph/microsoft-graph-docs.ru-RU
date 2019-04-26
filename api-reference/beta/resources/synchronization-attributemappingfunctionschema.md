---
title: Тип ресурса Аттрибутемаппингфунктионсчема
description: Описывает функцию, которая может использоваться в сопоставлении атрибутов для преобразования значений во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: ca66baf7fbc160cd4c57cba0f865ae07de9d5932
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345643"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="67bc5-103">Тип ресурса Аттрибутемаппингфунктионсчема</span><span class="sxs-lookup"><span data-stu-id="67bc5-103">attributeMappingFunctionSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67bc5-104">Описывает функцию, которая может использоваться в сопоставлении [атрибутов](synchronization-attributemapping.md) для преобразования значений во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="67bc5-104">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="67bc5-105">Методы</span><span class="sxs-lookup"><span data-stu-id="67bc5-105">Methods</span></span>

| <span data-ttu-id="67bc5-106">Метод</span><span class="sxs-lookup"><span data-stu-id="67bc5-106">Method</span></span>           | <span data-ttu-id="67bc5-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="67bc5-107">Return Type</span></span>    |<span data-ttu-id="67bc5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="67bc5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="67bc5-109">Перечисление</span><span class="sxs-lookup"><span data-stu-id="67bc5-109">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="67bc5-110">Коллекция [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="67bc5-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="67bc5-111">Список поддерживаемых функций сопоставления атрибутов.</span><span class="sxs-lookup"><span data-stu-id="67bc5-111">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="67bc5-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="67bc5-112">Properties</span></span>

| <span data-ttu-id="67bc5-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="67bc5-113">Property</span></span>                   | <span data-ttu-id="67bc5-114">Тип</span><span class="sxs-lookup"><span data-stu-id="67bc5-114">Type</span></span>                      | <span data-ttu-id="67bc5-115">Описание</span><span class="sxs-lookup"><span data-stu-id="67bc5-115">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="67bc5-116">name</span><span class="sxs-lookup"><span data-stu-id="67bc5-116">name</span></span>                        |<span data-ttu-id="67bc5-117">String</span><span class="sxs-lookup"><span data-stu-id="67bc5-117">String</span></span>                    |<span data-ttu-id="67bc5-118">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="67bc5-118">Operator name.</span></span> |
|<span data-ttu-id="67bc5-119">parameters</span><span class="sxs-lookup"><span data-stu-id="67bc5-119">parameters</span></span>                  |<span data-ttu-id="67bc5-120">Коллекция [аттрибутемаппингпараметерсчема](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="67bc5-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="67bc5-121">Коллекция параметров функции.</span><span class="sxs-lookup"><span data-stu-id="67bc5-121">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67bc5-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="67bc5-122">JSON representation</span></span>

<span data-ttu-id="67bc5-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67bc5-123">The following is a JSON representation of the resource.</span></span>

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
