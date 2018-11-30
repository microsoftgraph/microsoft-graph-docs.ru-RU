---
title: Тип ресурса educationAssignmentPointsGrade
description: Если тип марки точек назначения, каждой отправки будут иметь этот объект, связанный со свойством **submission.grade** . Это создаст подкласс из educationAssignmentGrade,
ms.openlocfilehash: 2439ac8946fea588bd7bc1afe7f1ff1042b9179a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076837"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="21c01-104">Тип ресурса educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="21c01-104">educationAssignmentPointsGrade resource type</span></span>

> <span data-ttu-id="21c01-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="21c01-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21c01-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21c01-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21c01-107">Если тип марки точек назначения, каждой отправки будут иметь этот объект, связанный со свойством **submission.grade** .</span><span class="sxs-lookup"><span data-stu-id="21c01-107">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="21c01-108">Это создаст подкласс из [educationAssignmentGrade](educationassignmentgrade.md), который добавит who данных этого свойства.</span><span class="sxs-lookup"><span data-stu-id="21c01-108">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="21c01-109">Max точек хранится в свойстве **assignments.grading** .</span><span class="sxs-lookup"><span data-stu-id="21c01-109">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="21c01-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="21c01-110">Properties</span></span>
| <span data-ttu-id="21c01-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="21c01-111">Property</span></span>     | <span data-ttu-id="21c01-112">Тип</span><span class="sxs-lookup"><span data-stu-id="21c01-112">Type</span></span>   |<span data-ttu-id="21c01-113">Description</span><span class="sxs-lookup"><span data-stu-id="21c01-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21c01-114">points</span><span class="sxs-lookup"><span data-stu-id="21c01-114">points</span></span>|<span data-ttu-id="21c01-115">Single</span><span class="sxs-lookup"><span data-stu-id="21c01-115">Single</span></span>|<span data-ttu-id="21c01-116">Число точек a учитель передается объект отправки.</span><span class="sxs-lookup"><span data-stu-id="21c01-116">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21c01-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21c01-117">JSON representation</span></span>

<span data-ttu-id="21c01-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21c01-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->