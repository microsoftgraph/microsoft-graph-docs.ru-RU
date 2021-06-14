---
title: rubricQualitySelectedColumnModel type
description: Указывает rubricLevel, выбранный преподавателем при классификации educationRubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9e69fa26d97684db4964ffba3d268ee1d1c11b44
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911516"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a><span data-ttu-id="1b532-103">rubricQualitySelectedColumnModel type</span><span class="sxs-lookup"><span data-stu-id="1b532-103">rubricQualitySelectedColumnModel resource type</span></span>

<span data-ttu-id="1b532-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b532-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b532-105">Указывает [rubricLevel,](rubriclevel.md) выбранный преподавателем при классификации [educationRubric](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="1b532-105">Indicates the [rubricLevel](rubriclevel.md) selected by the teacher when grading an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1b532-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b532-106">Properties</span></span>

| <span data-ttu-id="1b532-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b532-107">Property</span></span>     | <span data-ttu-id="1b532-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1b532-108">Type</span></span>        | <span data-ttu-id="1b532-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1b532-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b532-110">columnId</span><span class="sxs-lookup"><span data-stu-id="1b532-110">columnId</span></span>|<span data-ttu-id="1b532-111">String</span><span class="sxs-lookup"><span data-stu-id="1b532-111">String</span></span>|<span data-ttu-id="1b532-112">ID выбранного уровня для этого качества.</span><span class="sxs-lookup"><span data-stu-id="1b532-112">ID of the selected level for this quality.</span></span>|
|<span data-ttu-id="1b532-113">qualityId</span><span class="sxs-lookup"><span data-stu-id="1b532-113">qualityId</span></span>|<span data-ttu-id="1b532-114">String</span><span class="sxs-lookup"><span data-stu-id="1b532-114">String</span></span>|<span data-ttu-id="1b532-115">ID связанного качества.</span><span class="sxs-lookup"><span data-stu-id="1b532-115">ID of the associated quality.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b532-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b532-116">JSON representation</span></span>

<span data-ttu-id="1b532-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b532-117">The following is a JSON representation of the resource.</span></span>

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

