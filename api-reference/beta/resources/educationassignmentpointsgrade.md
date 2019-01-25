---
title: Тип ресурса educationAssignmentPointsGrade
description: Если тип марки точек назначения, каждой отправки будут иметь этот объект, связанный со свойством **submission.grade** . Это создаст подкласс из educationAssignmentGrade,
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5d2a5cf6f6f886185179c6f1a61c1bb1d9d1ecfc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523738"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="143c1-104">Тип ресурса educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="143c1-104">educationAssignmentPointsGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="143c1-105">Если тип марки точек назначения, каждой отправки будут иметь этот объект, связанный со свойством **submission.grade** .</span><span class="sxs-lookup"><span data-stu-id="143c1-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="143c1-106">Это создаст подкласс из [educationAssignmentGrade](educationassignmentgrade.md), который добавит who данных этого свойства.</span><span class="sxs-lookup"><span data-stu-id="143c1-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="143c1-107">Max точек хранится в свойстве **assignments.grading** .</span><span class="sxs-lookup"><span data-stu-id="143c1-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="143c1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="143c1-108">Properties</span></span>
| <span data-ttu-id="143c1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="143c1-109">Property</span></span>     | <span data-ttu-id="143c1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="143c1-110">Type</span></span>   |<span data-ttu-id="143c1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="143c1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="143c1-112">points</span><span class="sxs-lookup"><span data-stu-id="143c1-112">points</span></span>|<span data-ttu-id="143c1-113">Single</span><span class="sxs-lookup"><span data-stu-id="143c1-113">Single</span></span>|<span data-ttu-id="143c1-114">Число точек a учитель передается объект отправки.</span><span class="sxs-lookup"><span data-stu-id="143c1-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="143c1-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="143c1-115">JSON representation</span></span>

<span data-ttu-id="143c1-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="143c1-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
