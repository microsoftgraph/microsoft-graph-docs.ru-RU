---
title: тип ресурса educationAssignmentPointsGrade
description: Когда назначение заданной типу класса точек, каждый отправка будет иметь этот объект, связанный с **свойством submission.grade.**
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b624bd0e82336e4e416641240e072c8b4ac6392d
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912810"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="115e5-103">тип ресурса educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="115e5-103">educationAssignmentPointsGrade resource type</span></span>

<span data-ttu-id="115e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="115e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="115e5-105">Когда назначение заданной типу класса точек, каждый отправка будет иметь этот объект, связанный с **свойством submission.grade.**</span><span class="sxs-lookup"><span data-stu-id="115e5-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="115e5-106">Это создает подкласс из [educationAssignmentGrade,](educationassignmentgrade.md)который добавит данные who к этому свойству.</span><span class="sxs-lookup"><span data-stu-id="115e5-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="115e5-107">Максимальные точки хранятся в **свойстве assignments.grading.**</span><span class="sxs-lookup"><span data-stu-id="115e5-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="115e5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="115e5-108">Properties</span></span>
| <span data-ttu-id="115e5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="115e5-109">Property</span></span>     | <span data-ttu-id="115e5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="115e5-110">Type</span></span>   |<span data-ttu-id="115e5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="115e5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="115e5-112">points</span><span class="sxs-lookup"><span data-stu-id="115e5-112">points</span></span>|<span data-ttu-id="115e5-113">Одинарное</span><span class="sxs-lookup"><span data-stu-id="115e5-113">Single</span></span>|<span data-ttu-id="115e5-114">Количество точек, которые учитель дает этому объекту отправки.</span><span class="sxs-lookup"><span data-stu-id="115e5-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="115e5-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="115e5-115">JSON representation</span></span>

<span data-ttu-id="115e5-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="115e5-116">The following is a JSON representation of the resource.</span></span>

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


