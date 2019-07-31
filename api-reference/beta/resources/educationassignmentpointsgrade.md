---
title: Тип ресурса Едукатионассигнментпоинтсграде
description: Если для назначения задан тип уровня баллов, то каждая отправка будет иметь этот объект, связанный с свойством **отправку. Grade** . При этом создается подкласс из Едукатионассигнментграде,
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6e74c6bb74c830cb1ceb80e149903282c4da33ae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972819"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="7a9ba-104">Тип ресурса Едукатионассигнментпоинтсграде</span><span class="sxs-lookup"><span data-stu-id="7a9ba-104">educationAssignmentPointsGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a9ba-105">Если для назначения задан тип уровня баллов, то каждая отправка будет иметь этот объект, связанный с свойством **отправку. Grade** .</span><span class="sxs-lookup"><span data-stu-id="7a9ba-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="7a9ba-106">При этом создается подкласс из [едукатионассигнментграде](educationassignmentgrade.md), который добавляет к этому свойству данные.</span><span class="sxs-lookup"><span data-stu-id="7a9ba-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="7a9ba-107">Максимальные точки хранятся в свойстве **назначений. ступенчато** .</span><span class="sxs-lookup"><span data-stu-id="7a9ba-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="7a9ba-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a9ba-108">Properties</span></span>
| <span data-ttu-id="7a9ba-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a9ba-109">Property</span></span>     | <span data-ttu-id="7a9ba-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7a9ba-110">Type</span></span>   |<span data-ttu-id="7a9ba-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7a9ba-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a9ba-112">points</span><span class="sxs-lookup"><span data-stu-id="7a9ba-112">points</span></span>|<span data-ttu-id="7a9ba-113">Одинарное</span><span class="sxs-lookup"><span data-stu-id="7a9ba-113">Single</span></span>|<span data-ttu-id="7a9ba-114">Количество баллов, на которые преподаватель предоставляет этот объект отправки.</span><span class="sxs-lookup"><span data-stu-id="7a9ba-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a9ba-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a9ba-115">JSON representation</span></span>

<span data-ttu-id="7a9ba-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a9ba-116">The following is a JSON representation of the resource.</span></span>

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
