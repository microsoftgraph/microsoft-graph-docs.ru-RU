---
title: Тип ресурса Рубриккуалитиселектедколумнмодел
description: Указывает Рубриклевел, выбранный преподавателем при ступенчатом Едукатионрубрик
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a381ad878f16dab6197c72bd19d6f5aeee86f4a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016060"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a><span data-ttu-id="a40ac-103">Тип ресурса Рубриккуалитиселектедколумнмодел</span><span class="sxs-lookup"><span data-stu-id="a40ac-103">rubricQualitySelectedColumnModel resource type</span></span>

<span data-ttu-id="a40ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a40ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a40ac-105">Указывает [рубриклевел](rubriclevel.md) , выбранный преподавателем при ступенчатом [едукатионрубрик](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="a40ac-105">Indicates the [rubricLevel](rubriclevel.md) selected by the teacher when grading an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a40ac-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a40ac-106">Properties</span></span>

| <span data-ttu-id="a40ac-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a40ac-107">Property</span></span>     | <span data-ttu-id="a40ac-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a40ac-108">Type</span></span>        | <span data-ttu-id="a40ac-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a40ac-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a40ac-110">columnId</span><span class="sxs-lookup"><span data-stu-id="a40ac-110">columnId</span></span>|<span data-ttu-id="a40ac-111">String</span><span class="sxs-lookup"><span data-stu-id="a40ac-111">String</span></span>|<span data-ttu-id="a40ac-112">Идентификатор выбранного уровня для этого качества.</span><span class="sxs-lookup"><span data-stu-id="a40ac-112">ID of the selected level for this quality.</span></span>|
|<span data-ttu-id="a40ac-113">куалитид</span><span class="sxs-lookup"><span data-stu-id="a40ac-113">qualityId</span></span>|<span data-ttu-id="a40ac-114">String</span><span class="sxs-lookup"><span data-stu-id="a40ac-114">String</span></span>|<span data-ttu-id="a40ac-115">Идентификатор связанного качества.</span><span class="sxs-lookup"><span data-stu-id="a40ac-115">ID of the associated quality.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a40ac-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a40ac-116">JSON representation</span></span>

<span data-ttu-id="a40ac-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a40ac-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel",
  "baseType": null
}-->

```json
{
  "columnId": "String",
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualitySelectedColumnModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

