---
title: Тип ресурса Едукатионассигнментпоинтсграде
description: Если для назначения задан тип уровня баллов, то каждая отправка будет иметь этот объект, связанный с свойством **отправку. Grade** . При этом создается подкласс из Едукатионассигнментграде,
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: bcce2fc6445c465defb2d795f3bfab9545838643
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013721"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="591fa-104">Тип ресурса Едукатионассигнментпоинтсграде</span><span class="sxs-lookup"><span data-stu-id="591fa-104">educationAssignmentPointsGrade resource type</span></span>

<span data-ttu-id="591fa-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="591fa-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="591fa-106">Если для назначения задан тип уровня баллов, то каждая отправка будет иметь этот объект, связанный с свойством **отправку. Grade** .</span><span class="sxs-lookup"><span data-stu-id="591fa-106">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="591fa-107">При этом создается подкласс из [едукатионассигнментграде](educationassignmentgrade.md), который добавляет к этому свойству данные.</span><span class="sxs-lookup"><span data-stu-id="591fa-107">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="591fa-108">Максимальные точки хранятся в свойстве **назначений. ступенчато** .</span><span class="sxs-lookup"><span data-stu-id="591fa-108">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="591fa-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="591fa-109">Properties</span></span>
| <span data-ttu-id="591fa-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="591fa-110">Property</span></span>     | <span data-ttu-id="591fa-111">Тип</span><span class="sxs-lookup"><span data-stu-id="591fa-111">Type</span></span>   |<span data-ttu-id="591fa-112">Описание</span><span class="sxs-lookup"><span data-stu-id="591fa-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="591fa-113">points</span><span class="sxs-lookup"><span data-stu-id="591fa-113">points</span></span>|<span data-ttu-id="591fa-114">Одинарное</span><span class="sxs-lookup"><span data-stu-id="591fa-114">Single</span></span>|<span data-ttu-id="591fa-115">Количество баллов, на которые преподаватель предоставляет этот объект отправки.</span><span class="sxs-lookup"><span data-stu-id="591fa-115">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="591fa-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="591fa-116">JSON representation</span></span>

<span data-ttu-id="591fa-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="591fa-117">The following is a JSON representation of the resource.</span></span>

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


