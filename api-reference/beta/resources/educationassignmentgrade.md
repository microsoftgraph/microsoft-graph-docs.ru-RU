---
title: Тип ресурса educationAssignmentGrade
description: " Тем не менее являются подклассов это всех типов участников (точек, работоспособность и т.д.)"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: ecdd92c84399ee17d2808301d997830725fb5642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982360"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="efc3e-103">Тип ресурса educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="efc3e-103">educationAssignmentGrade resource type</span></span>

> <span data-ttu-id="efc3e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="efc3e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efc3e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efc3e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="efc3e-106">Представляет объект **марки** на отправку.</span><span class="sxs-lookup"><span data-stu-id="efc3e-106">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="efc3e-107">Это абстрактный тип, никогда не будет создаваться; Тем не менее все типы участников (точек, работоспособность и т.д.), подклассов этого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="efc3e-107">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="efc3e-108">Этот объект также отслеживает, который делает участников.</span><span class="sxs-lookup"><span data-stu-id="efc3e-108">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="efc3e-109">Используется в свойстве **submission.grade** .</span><span class="sxs-lookup"><span data-stu-id="efc3e-109">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="efc3e-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="efc3e-110">Properties</span></span>
| <span data-ttu-id="efc3e-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="efc3e-111">Property</span></span>     | <span data-ttu-id="efc3e-112">Тип</span><span class="sxs-lookup"><span data-stu-id="efc3e-112">Type</span></span>   |<span data-ttu-id="efc3e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="efc3e-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efc3e-114">gradedBy</span><span class="sxs-lookup"><span data-stu-id="efc3e-114">gradedBy</span></span>|[<span data-ttu-id="efc3e-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="efc3e-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="efc3e-116">Пользователь, который был участников.</span><span class="sxs-lookup"><span data-stu-id="efc3e-116">User who did the grading.</span></span> |
|<span data-ttu-id="efc3e-117">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="efc3e-117">gradedDateTime</span></span>|<span data-ttu-id="efc3e-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efc3e-118">DateTimeOffset</span></span>| <span data-ttu-id="efc3e-119">Момент времени, когда марки была применена этот объект отправки.</span><span class="sxs-lookup"><span data-stu-id="efc3e-119">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="efc3e-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="efc3e-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="efc3e-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="efc3e-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efc3e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efc3e-122">JSON representation</span></span>

<span data-ttu-id="efc3e-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efc3e-123">The following is a JSON representation of the resource.</span></span>

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
