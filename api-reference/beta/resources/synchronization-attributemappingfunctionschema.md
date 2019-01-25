---
title: Тип ресурса attributeMappingFunctionSchema
description: Описываются функции, которая может использоваться в Отображение атрибута для преобразования значения во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: e2c0139f7c797c3f519cc638561b09f611018b28
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511984"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="15fcd-103">Тип ресурса attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="15fcd-103">attributeMappingFunctionSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15fcd-104">Описываются функции, который может использоваться в [сопоставление атрибутов](synchronization-attributemapping.md) для преобразования значения во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="15fcd-104">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="15fcd-105">Методы</span><span class="sxs-lookup"><span data-stu-id="15fcd-105">Methods</span></span>

| <span data-ttu-id="15fcd-106">Метод</span><span class="sxs-lookup"><span data-stu-id="15fcd-106">Method</span></span>           | <span data-ttu-id="15fcd-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="15fcd-107">Return Type</span></span>    |<span data-ttu-id="15fcd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="15fcd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="15fcd-109">List</span><span class="sxs-lookup"><span data-stu-id="15fcd-109">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="15fcd-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="15fcd-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="15fcd-111">Список поддерживаемых атрибут сопоставления функций.</span><span class="sxs-lookup"><span data-stu-id="15fcd-111">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="15fcd-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="15fcd-112">Properties</span></span>

| <span data-ttu-id="15fcd-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="15fcd-113">Property</span></span>                   | <span data-ttu-id="15fcd-114">Тип</span><span class="sxs-lookup"><span data-stu-id="15fcd-114">Type</span></span>                      | <span data-ttu-id="15fcd-115">Описание</span><span class="sxs-lookup"><span data-stu-id="15fcd-115">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="15fcd-116">name</span><span class="sxs-lookup"><span data-stu-id="15fcd-116">name</span></span>                        |<span data-ttu-id="15fcd-117">String</span><span class="sxs-lookup"><span data-stu-id="15fcd-117">String</span></span>                    |<span data-ttu-id="15fcd-118">Имя оператора.</span><span class="sxs-lookup"><span data-stu-id="15fcd-118">Operator name.</span></span> |
|<span data-ttu-id="15fcd-119">parameters</span><span class="sxs-lookup"><span data-stu-id="15fcd-119">parameters</span></span>                  |<span data-ttu-id="15fcd-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="15fcd-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="15fcd-121">Коллекция параметров функции.</span><span class="sxs-lookup"><span data-stu-id="15fcd-121">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15fcd-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15fcd-122">JSON representation</span></span>

<span data-ttu-id="15fcd-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15fcd-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingfunctionschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
