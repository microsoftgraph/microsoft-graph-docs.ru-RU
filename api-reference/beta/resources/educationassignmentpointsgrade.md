---
title: Тип ресурса Едукатионассигнментпоинтсграде
description: Если для назначения задан тип уровня баллов, то каждая отправка будет иметь этот объект, связанный с свойством **отправку. Grade** . При этом создается подкласс из Едукатионассигнментграде,
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 166f6b5ce377441641cf12232c2194dff1184765
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340590"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="e1d1f-104">Тип ресурса Едукатионассигнментпоинтсграде</span><span class="sxs-lookup"><span data-stu-id="e1d1f-104">educationAssignmentPointsGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1d1f-105">Если для назначения задан тип уровня баллов, то каждая отправка будет иметь этот объект, связанный с свойством **отправку. Grade** .</span><span class="sxs-lookup"><span data-stu-id="e1d1f-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="e1d1f-106">При этом создается подкласс из [едукатионассигнментграде](educationassignmentgrade.md), который добавляет к этому свойству данные.</span><span class="sxs-lookup"><span data-stu-id="e1d1f-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="e1d1f-107">Максимальные точки хранятся в свойстве **назначений. ступенчато** .</span><span class="sxs-lookup"><span data-stu-id="e1d1f-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="e1d1f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1d1f-108">Properties</span></span>
| <span data-ttu-id="e1d1f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1d1f-109">Property</span></span>     | <span data-ttu-id="e1d1f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e1d1f-110">Type</span></span>   |<span data-ttu-id="e1d1f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e1d1f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1d1f-112">points</span><span class="sxs-lookup"><span data-stu-id="e1d1f-112">points</span></span>|<span data-ttu-id="e1d1f-113">Одинарное</span><span class="sxs-lookup"><span data-stu-id="e1d1f-113">Single</span></span>|<span data-ttu-id="e1d1f-114">Количество баллов, на которые преподаватель предоставляет этот объект отправки.</span><span class="sxs-lookup"><span data-stu-id="e1d1f-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1d1f-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1d1f-115">JSON representation</span></span>

<span data-ttu-id="e1d1f-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1d1f-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
