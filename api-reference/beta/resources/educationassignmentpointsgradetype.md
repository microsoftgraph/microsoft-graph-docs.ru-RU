---
title: Тип ресурса educationAssignmentPointsGradeType
description: Используется совместно со свойством **assignments.grading** . Это подкласс educationAssignmentGradeType.
ms.openlocfilehash: 5c170540e99003a78df0550d4d6542c07df8f1ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081821"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="01d3f-104">Тип ресурса educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="01d3f-104">educationAssignmentPointsGradeType resource type</span></span>

> <span data-ttu-id="01d3f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01d3f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01d3f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d3f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01d3f-107">Используется совместно со свойством **assignments.grading** .</span><span class="sxs-lookup"><span data-stu-id="01d3f-107">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="01d3f-108">Это подкласс [educationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="01d3f-108">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="01d3f-109">Это означает, что назначения выражаемым числом и сохраняет максимальное число пунктов, которые можно достичь каждого студента на этот рабочий элемент.</span><span class="sxs-lookup"><span data-stu-id="01d3f-109">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="01d3f-110">Если это назначения, каждой отправки будет [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) свойства, связанного с ним для хранения каждого студента точек.</span><span class="sxs-lookup"><span data-stu-id="01d3f-110">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="01d3f-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="01d3f-111">Properties</span></span>
| <span data-ttu-id="01d3f-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="01d3f-112">Property</span></span>     | <span data-ttu-id="01d3f-113">Тип</span><span class="sxs-lookup"><span data-stu-id="01d3f-113">Type</span></span>   |<span data-ttu-id="01d3f-114">Description</span><span class="sxs-lookup"><span data-stu-id="01d3f-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01d3f-115">maxPoints</span><span class="sxs-lookup"><span data-stu-id="01d3f-115">maxPoints</span></span>|<span data-ttu-id="01d3f-116">Single</span><span class="sxs-lookup"><span data-stu-id="01d3f-116">Single</span></span>| <span data-ttu-id="01d3f-117">Максимальное число точек можно для данного назначения.</span><span class="sxs-lookup"><span data-stu-id="01d3f-117">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="01d3f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01d3f-118">JSON representation</span></span>

<span data-ttu-id="01d3f-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01d3f-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->