---
title: Тип ресурса Едукатионассигнментпоинтсградетипе
description: Используется с свойством **назначений. ступенчато** . Это подкласс Едукатионассигнментградетипе.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b11ba94bba2147e2ef1d084a66cd7628371a57fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998890"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="f723b-104">Тип ресурса Едукатионассигнментпоинтсградетипе</span><span class="sxs-lookup"><span data-stu-id="f723b-104">educationAssignmentPointsGradeType resource type</span></span>

<span data-ttu-id="f723b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f723b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f723b-106">Используется с свойством **назначений. ступенчато** .</span><span class="sxs-lookup"><span data-stu-id="f723b-106">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="f723b-107">Это подкласс [едукатионассигнментградетипе](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="f723b-107">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="f723b-108">Это означает, что назначение обладает повышенными уровнями и сохраняет максимальное число баллов, которое каждый учащийся может выполнить для этого рабочего элемента.</span><span class="sxs-lookup"><span data-stu-id="f723b-108">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="f723b-109">Если этот параметр задан для назначения, при каждой отправке будет получено свойство [едукатионассигнментпоинтсграде](educationassignmentpointsgrade.md) , связанное с ним для хранения точек каждого учащегося.</span><span class="sxs-lookup"><span data-stu-id="f723b-109">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="f723b-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="f723b-110">Properties</span></span>
| <span data-ttu-id="f723b-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="f723b-111">Property</span></span>     | <span data-ttu-id="f723b-112">Тип</span><span class="sxs-lookup"><span data-stu-id="f723b-112">Type</span></span>   |<span data-ttu-id="f723b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f723b-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f723b-114">макспоинтс</span><span class="sxs-lookup"><span data-stu-id="f723b-114">maxPoints</span></span>|<span data-ttu-id="f723b-115">Одинарное</span><span class="sxs-lookup"><span data-stu-id="f723b-115">Single</span></span>| <span data-ttu-id="f723b-116">Максимальное число баллов, которое можно сделать для этого назначения.</span><span class="sxs-lookup"><span data-stu-id="f723b-116">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f723b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f723b-117">JSON representation</span></span>

<span data-ttu-id="f723b-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f723b-118">The following is a JSON representation of the resource.</span></span>

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


