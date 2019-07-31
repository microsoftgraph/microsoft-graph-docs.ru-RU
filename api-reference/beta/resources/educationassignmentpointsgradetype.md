---
title: Тип ресурса Едукатионассигнментпоинтсградетипе
description: Используется с свойством **назначений. ступенчато** . Это подкласс Едукатионассигнментградетипе.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 18661c6d0eb0269f429fe22203b59b4f6862f21c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972805"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="1adb8-104">Тип ресурса Едукатионассигнментпоинтсградетипе</span><span class="sxs-lookup"><span data-stu-id="1adb8-104">educationAssignmentPointsGradeType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1adb8-105">Используется с свойством **назначений. ступенчато** .</span><span class="sxs-lookup"><span data-stu-id="1adb8-105">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="1adb8-106">Это подкласс [едукатионассигнментградетипе](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="1adb8-106">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="1adb8-107">Это означает, что назначение обладает повышенными уровнями и сохраняет максимальное число баллов, которое каждый учащийся может выполнить для этого рабочего элемента.</span><span class="sxs-lookup"><span data-stu-id="1adb8-107">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="1adb8-108">Если этот параметр задан для назначения, при каждой отправке будет получено свойство [едукатионассигнментпоинтсграде](educationassignmentpointsgrade.md) , связанное с ним для хранения точек каждого учащегося.</span><span class="sxs-lookup"><span data-stu-id="1adb8-108">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="1adb8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1adb8-109">Properties</span></span>
| <span data-ttu-id="1adb8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1adb8-110">Property</span></span>     | <span data-ttu-id="1adb8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1adb8-111">Type</span></span>   |<span data-ttu-id="1adb8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1adb8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1adb8-113">Макспоинтс</span><span class="sxs-lookup"><span data-stu-id="1adb8-113">maxPoints</span></span>|<span data-ttu-id="1adb8-114">Одинарное</span><span class="sxs-lookup"><span data-stu-id="1adb8-114">Single</span></span>| <span data-ttu-id="1adb8-115">Максимальное число баллов, которое можно сделать для этого назначения.</span><span class="sxs-lookup"><span data-stu-id="1adb8-115">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="1adb8-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1adb8-116">JSON representation</span></span>

<span data-ttu-id="1adb8-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1adb8-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
