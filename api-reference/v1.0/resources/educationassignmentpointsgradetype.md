---
title: тип ресурсов educationAssignmentPointsGradeType
description: Тип ресурса, используемый с **свойством assignments.grading.** Это подкласс educationAssignmentGradeType.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca5a6ba0dd6674d55b4659fbdb1e2c288a65eb12
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912865"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="86bc2-104">тип ресурсов educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="86bc2-104">educationAssignmentPointsGradeType resource type</span></span>

<span data-ttu-id="86bc2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86bc2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86bc2-106">Тип ресурса, используемый с **свойством assignments.grading.**</span><span class="sxs-lookup"><span data-stu-id="86bc2-106">Resource type that is used with the **assignments.grading** property.</span></span> <span data-ttu-id="86bc2-107">Это подкласс [educationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="86bc2-107">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="86bc2-108">Это указывает на то, что назначение имеет оценку и сохраняет максимальное количество баллов, которые каждый учащийся может достичь в этом элементе работы.</span><span class="sxs-lookup"><span data-stu-id="86bc2-108">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="86bc2-109">При назначении каждая отправка получит свойство [educationAssignmentPointsGrade,](educationassignmentpointsgrade.md) связанное с ним для хранения баллов каждого учащегося.</span><span class="sxs-lookup"><span data-stu-id="86bc2-109">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="86bc2-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="86bc2-110">Properties</span></span>
| <span data-ttu-id="86bc2-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="86bc2-111">Property</span></span>     | <span data-ttu-id="86bc2-112">Тип</span><span class="sxs-lookup"><span data-stu-id="86bc2-112">Type</span></span>   |<span data-ttu-id="86bc2-113">Описание</span><span class="sxs-lookup"><span data-stu-id="86bc2-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86bc2-114">maxPoints</span><span class="sxs-lookup"><span data-stu-id="86bc2-114">maxPoints</span></span>|<span data-ttu-id="86bc2-115">Одинарное</span><span class="sxs-lookup"><span data-stu-id="86bc2-115">Single</span></span>| <span data-ttu-id="86bc2-116">Max указывает возможное для этого назначения.</span><span class="sxs-lookup"><span data-stu-id="86bc2-116">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="86bc2-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86bc2-117">JSON representation</span></span>

<span data-ttu-id="86bc2-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86bc2-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Double"
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
  "suppressions": []
}
-->


