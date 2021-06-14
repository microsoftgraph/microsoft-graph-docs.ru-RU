---
title: тип ресурса educationAssignmentGrade
description: Представляет объект Grade в представлении.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ea25bb723249878637d98d91d8c91e14891f8465
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912649"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="0baa7-103">тип ресурса educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="0baa7-103">educationAssignmentGrade resource type</span></span>

<span data-ttu-id="0baa7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0baa7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0baa7-105">Представляет объект **Grade** в представлении.</span><span class="sxs-lookup"><span data-stu-id="0baa7-105">Represents the **Grade** object on a Submission.</span></span> 

<span data-ttu-id="0baa7-106">Это абстрактный тип, который никогда не будет мгновенным; Однако все типы классификации (точки, пропуск/сбой и так далее) являются подклассами этого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="0baa7-106">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="0baa7-107">Этот объект также отслеживает, кто делает классификацию.</span><span class="sxs-lookup"><span data-stu-id="0baa7-107">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="0baa7-108">Это используется в **свойстве submission.grade.**</span><span class="sxs-lookup"><span data-stu-id="0baa7-108">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="0baa7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0baa7-109">Properties</span></span>
| <span data-ttu-id="0baa7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0baa7-110">Property</span></span>     | <span data-ttu-id="0baa7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0baa7-111">Type</span></span>   |<span data-ttu-id="0baa7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0baa7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0baa7-113">gradedBy</span><span class="sxs-lookup"><span data-stu-id="0baa7-113">gradedBy</span></span>|[<span data-ttu-id="0baa7-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="0baa7-114">identitySet</span></span>](identityset.md)| <span data-ttu-id="0baa7-115">Пользователь, который сделал классификацию.</span><span class="sxs-lookup"><span data-stu-id="0baa7-115">User who did the grading.</span></span> |
|<span data-ttu-id="0baa7-116">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="0baa7-116">gradedDateTime</span></span>|<span data-ttu-id="0baa7-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0baa7-117">DateTimeOffset</span></span>| <span data-ttu-id="0baa7-118">Момент времени, когда оценка была применена к этому объекту отправки.</span><span class="sxs-lookup"><span data-stu-id="0baa7-118">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="0baa7-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0baa7-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0baa7-120">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="0baa7-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0baa7-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0baa7-121">JSON representation</span></span>

<span data-ttu-id="0baa7-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0baa7-122">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


