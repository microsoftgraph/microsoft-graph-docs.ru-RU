---
title: Тип ресурса educationAssignmentGrade
description: " Тем не менее являются подклассов это всех типов участников (точек, работоспособность и т.д.)"
localization_priority: Normal
ms.openlocfilehash: 371346c6ff23623a118b9ee169e563e75e2429f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889014"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="01cd3-103">Тип ресурса educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="01cd3-103">educationAssignmentGrade resource type</span></span>

> <span data-ttu-id="01cd3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01cd3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01cd3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01cd3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01cd3-106">Представляет объект **марки** на отправку.</span><span class="sxs-lookup"><span data-stu-id="01cd3-106">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="01cd3-107">Это абстрактный тип, никогда не будет создаваться; Тем не менее все типы участников (точек, работоспособность и т.д.), подклассов этого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="01cd3-107">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="01cd3-108">Этот объект также отслеживает, который делает участников.</span><span class="sxs-lookup"><span data-stu-id="01cd3-108">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="01cd3-109">Используется в свойстве **submission.grade** .</span><span class="sxs-lookup"><span data-stu-id="01cd3-109">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="01cd3-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="01cd3-110">Properties</span></span>
| <span data-ttu-id="01cd3-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="01cd3-111">Property</span></span>     | <span data-ttu-id="01cd3-112">Тип</span><span class="sxs-lookup"><span data-stu-id="01cd3-112">Type</span></span>   |<span data-ttu-id="01cd3-113">Описание</span><span class="sxs-lookup"><span data-stu-id="01cd3-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01cd3-114">gradedBy</span><span class="sxs-lookup"><span data-stu-id="01cd3-114">gradedBy</span></span>|[<span data-ttu-id="01cd3-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="01cd3-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="01cd3-116">Пользователь, который был участников.</span><span class="sxs-lookup"><span data-stu-id="01cd3-116">User who did the grading.</span></span> |
|<span data-ttu-id="01cd3-117">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="01cd3-117">gradedDateTime</span></span>|<span data-ttu-id="01cd3-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01cd3-118">DateTimeOffset</span></span>| <span data-ttu-id="01cd3-119">Момент времени, когда марки была применена этот объект отправки.</span><span class="sxs-lookup"><span data-stu-id="01cd3-119">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="01cd3-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="01cd3-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="01cd3-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="01cd3-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01cd3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01cd3-122">JSON representation</span></span>

<span data-ttu-id="01cd3-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01cd3-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
