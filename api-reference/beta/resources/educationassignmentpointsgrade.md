---
title: Тип ресурса Едукатионассигнментпоинтсграде
description: Если для назначения задан тип уровня баллов, то каждая отправка будет иметь этот объект, связанный с свойством **отправку. Grade** . При этом создается подкласс из Едукатионассигнментграде,
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c2ef014c3e9e2954dba5fb759fcf3f86b3681b68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502510"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="304f3-104">Тип ресурса Едукатионассигнментпоинтсграде</span><span class="sxs-lookup"><span data-stu-id="304f3-104">educationAssignmentPointsGrade resource type</span></span>

<span data-ttu-id="304f3-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="304f3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="304f3-106">Если для назначения задан тип уровня баллов, то каждая отправка будет иметь этот объект, связанный с свойством **отправку. Grade** .</span><span class="sxs-lookup"><span data-stu-id="304f3-106">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="304f3-107">При этом создается подкласс из [едукатионассигнментграде](educationassignmentgrade.md), который добавляет к этому свойству данные.</span><span class="sxs-lookup"><span data-stu-id="304f3-107">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="304f3-108">Максимальные точки хранятся в свойстве **назначений. ступенчато** .</span><span class="sxs-lookup"><span data-stu-id="304f3-108">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="304f3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="304f3-109">Properties</span></span>
| <span data-ttu-id="304f3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="304f3-110">Property</span></span>     | <span data-ttu-id="304f3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="304f3-111">Type</span></span>   |<span data-ttu-id="304f3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="304f3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="304f3-113">points</span><span class="sxs-lookup"><span data-stu-id="304f3-113">points</span></span>|<span data-ttu-id="304f3-114">Одинарное</span><span class="sxs-lookup"><span data-stu-id="304f3-114">Single</span></span>|<span data-ttu-id="304f3-115">Количество баллов, на которые преподаватель предоставляет этот объект отправки.</span><span class="sxs-lookup"><span data-stu-id="304f3-115">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="304f3-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="304f3-116">JSON representation</span></span>

<span data-ttu-id="304f3-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="304f3-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Double"
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
