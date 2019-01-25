---
title: Тип ресурса educationAssignmentPointsGradeType
description: Используется совместно со свойством **assignments.grading** . Это подкласс educationAssignmentGradeType.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 567bff38f8a20456dffffdd91775a1e32852fe20
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508897"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="0cc88-104">Тип ресурса educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="0cc88-104">educationAssignmentPointsGradeType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cc88-105">Используется совместно со свойством **assignments.grading** .</span><span class="sxs-lookup"><span data-stu-id="0cc88-105">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="0cc88-106">Это подкласс [educationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="0cc88-106">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="0cc88-107">Это означает, что назначения выражаемым числом и сохраняет максимальное число пунктов, которые можно достичь каждого студента на этот рабочий элемент.</span><span class="sxs-lookup"><span data-stu-id="0cc88-107">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="0cc88-108">Если это назначения, каждой отправки будет [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) свойства, связанного с ним для хранения каждого студента точек.</span><span class="sxs-lookup"><span data-stu-id="0cc88-108">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="0cc88-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cc88-109">Properties</span></span>
| <span data-ttu-id="0cc88-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cc88-110">Property</span></span>     | <span data-ttu-id="0cc88-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0cc88-111">Type</span></span>   |<span data-ttu-id="0cc88-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0cc88-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cc88-113">maxPoints</span><span class="sxs-lookup"><span data-stu-id="0cc88-113">maxPoints</span></span>|<span data-ttu-id="0cc88-114">Single</span><span class="sxs-lookup"><span data-stu-id="0cc88-114">Single</span></span>| <span data-ttu-id="0cc88-115">Максимальное число точек можно для данного назначения.</span><span class="sxs-lookup"><span data-stu-id="0cc88-115">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="0cc88-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cc88-116">JSON representation</span></span>

<span data-ttu-id="0cc88-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cc88-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgradetype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
