---
title: Тип ресурса educationAssignmentPointsGradeType
description: Используется совместно со свойством **assignments.grading** . Это подкласс educationAssignmentGradeType.
localization_priority: Normal
ms.openlocfilehash: f00014eab1dbf7bc8eb78a8898c6abba9977e8a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860972"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="80b41-104">Тип ресурса educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="80b41-104">educationAssignmentPointsGradeType resource type</span></span>

> <span data-ttu-id="80b41-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="80b41-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80b41-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80b41-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="80b41-107">Используется совместно со свойством **assignments.grading** .</span><span class="sxs-lookup"><span data-stu-id="80b41-107">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="80b41-108">Это подкласс [educationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="80b41-108">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="80b41-109">Это означает, что назначения выражаемым числом и сохраняет максимальное число пунктов, которые можно достичь каждого студента на этот рабочий элемент.</span><span class="sxs-lookup"><span data-stu-id="80b41-109">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="80b41-110">Если это назначения, каждой отправки будет [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) свойства, связанного с ним для хранения каждого студента точек.</span><span class="sxs-lookup"><span data-stu-id="80b41-110">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="80b41-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="80b41-111">Properties</span></span>
| <span data-ttu-id="80b41-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="80b41-112">Property</span></span>     | <span data-ttu-id="80b41-113">Тип</span><span class="sxs-lookup"><span data-stu-id="80b41-113">Type</span></span>   |<span data-ttu-id="80b41-114">Описание</span><span class="sxs-lookup"><span data-stu-id="80b41-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80b41-115">maxPoints</span><span class="sxs-lookup"><span data-stu-id="80b41-115">maxPoints</span></span>|<span data-ttu-id="80b41-116">Single</span><span class="sxs-lookup"><span data-stu-id="80b41-116">Single</span></span>| <span data-ttu-id="80b41-117">Максимальное число точек можно для данного назначения.</span><span class="sxs-lookup"><span data-stu-id="80b41-117">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="80b41-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80b41-118">JSON representation</span></span>

<span data-ttu-id="80b41-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80b41-119">The following is a JSON representation of the resource.</span></span>

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
