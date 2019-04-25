---
title: Тип ресурса Едукатионассигнментпоинтсградетипе
description: Используется с свойством **назначений. ступенчато** . Это подкласс Едукатионассигнментградетипе.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 567bff38f8a20456dffffdd91775a1e32852fe20
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543121"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="4599a-104">Тип ресурса Едукатионассигнментпоинтсградетипе</span><span class="sxs-lookup"><span data-stu-id="4599a-104">educationAssignmentPointsGradeType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4599a-105">Используется с свойством **назначений. ступенчато** .</span><span class="sxs-lookup"><span data-stu-id="4599a-105">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="4599a-106">Это подкласс [едукатионассигнментградетипе](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="4599a-106">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="4599a-107">Это означает, что назначение обладает повышенными уровнями и сохраняет максимальное число баллов, которое каждый учащийся может выполнить для этого рабочего элемента.</span><span class="sxs-lookup"><span data-stu-id="4599a-107">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="4599a-108">Если этот параметр задан для назначения, при каждой отправке будет получено свойство [едукатионассигнментпоинтсграде](educationassignmentpointsgrade.md) , связанное с ним для хранения точек каждого учащегося.</span><span class="sxs-lookup"><span data-stu-id="4599a-108">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="4599a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4599a-109">Properties</span></span>
| <span data-ttu-id="4599a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4599a-110">Property</span></span>     | <span data-ttu-id="4599a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4599a-111">Type</span></span>   |<span data-ttu-id="4599a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4599a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4599a-113">Макспоинтс</span><span class="sxs-lookup"><span data-stu-id="4599a-113">maxPoints</span></span>|<span data-ttu-id="4599a-114">Одинарное</span><span class="sxs-lookup"><span data-stu-id="4599a-114">Single</span></span>| <span data-ttu-id="4599a-115">Максимальное число баллов, которое можно сделать для этого назначения.</span><span class="sxs-lookup"><span data-stu-id="4599a-115">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="4599a-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4599a-116">JSON representation</span></span>

<span data-ttu-id="4599a-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4599a-117">The following is a JSON representation of the resource.</span></span>

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
