---
title: Тип ресурса Рубриккуалитиселектедколумнмодел
description: Указывает Рубриклевел, выбранный преподавателем при ступенчатом Едукатионрубрик
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6fd6ff5d9def23a6a6fb180c8d12398437e5dce0
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173295"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a><span data-ttu-id="5e2ff-103">Тип ресурса Рубриккуалитиселектедколумнмодел</span><span class="sxs-lookup"><span data-stu-id="5e2ff-103">rubricQualitySelectedColumnModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e2ff-104">Указывает [рубриклевел](rubriclevel.md) , выбранный преподавателем при ступенчатом [едукатионрубрик](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="5e2ff-104">Indicates the [rubricLevel](rubriclevel.md) selected by the teacher when grading an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5e2ff-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e2ff-105">Properties</span></span>

| <span data-ttu-id="5e2ff-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e2ff-106">Property</span></span>     | <span data-ttu-id="5e2ff-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5e2ff-107">Type</span></span>        | <span data-ttu-id="5e2ff-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5e2ff-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5e2ff-109">columnId</span><span class="sxs-lookup"><span data-stu-id="5e2ff-109">columnId</span></span>|<span data-ttu-id="5e2ff-110">String</span><span class="sxs-lookup"><span data-stu-id="5e2ff-110">String</span></span>|<span data-ttu-id="5e2ff-111">Идентификатор выбранного уровня для этого качества.</span><span class="sxs-lookup"><span data-stu-id="5e2ff-111">ID of the selected level for this quality.</span></span>|
|<span data-ttu-id="5e2ff-112">Куалитид</span><span class="sxs-lookup"><span data-stu-id="5e2ff-112">qualityId</span></span>|<span data-ttu-id="5e2ff-113">String</span><span class="sxs-lookup"><span data-stu-id="5e2ff-113">String</span></span>|<span data-ttu-id="5e2ff-114">Идентификатор связанного качества.</span><span class="sxs-lookup"><span data-stu-id="5e2ff-114">ID of the associated quality.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e2ff-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e2ff-115">JSON representation</span></span>

<span data-ttu-id="5e2ff-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e2ff-116">The following is a JSON representation of the resource.</span></span>

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