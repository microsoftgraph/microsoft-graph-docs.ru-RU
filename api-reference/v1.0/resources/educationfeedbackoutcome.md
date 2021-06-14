---
title: тип ресурса educationFeedbackOutcome
description: EducationOutcome, который дает обратную связь в виде текста.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d29a09ccca331e466812c44e8f397696d1eb3539
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912632"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="76f64-103">тип ресурса educationFeedbackOutcome</span><span class="sxs-lookup"><span data-stu-id="76f64-103">educationFeedbackOutcome resource type</span></span>

<span data-ttu-id="76f64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76f64-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76f64-105">Представляет обратную связь по [объекту educationOutcome](educationoutcome.md) в виде текста.</span><span class="sxs-lookup"><span data-stu-id="76f64-105">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="76f64-106">Методы</span><span class="sxs-lookup"><span data-stu-id="76f64-106">Methods</span></span>

| <span data-ttu-id="76f64-107">Метод</span><span class="sxs-lookup"><span data-stu-id="76f64-107">Method</span></span>       | <span data-ttu-id="76f64-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="76f64-108">Return Type</span></span> | <span data-ttu-id="76f64-109">Описание</span><span class="sxs-lookup"><span data-stu-id="76f64-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="76f64-110">Обновление educationOutcome</span><span class="sxs-lookup"><span data-stu-id="76f64-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="76f64-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="76f64-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="76f64-112">Обновление объекта educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="76f64-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="76f64-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="76f64-113">Properties</span></span>

| <span data-ttu-id="76f64-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="76f64-114">Property</span></span>     | <span data-ttu-id="76f64-115">Тип</span><span class="sxs-lookup"><span data-stu-id="76f64-115">Type</span></span>        | <span data-ttu-id="76f64-116">Описание</span><span class="sxs-lookup"><span data-stu-id="76f64-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="76f64-117">feedback</span><span class="sxs-lookup"><span data-stu-id="76f64-117">feedback</span></span>|[<span data-ttu-id="76f64-118">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="76f64-118">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="76f64-119">Письменные отзывы преподавателя для учащегося.</span><span class="sxs-lookup"><span data-stu-id="76f64-119">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="76f64-120">publishedFeedback</span><span class="sxs-lookup"><span data-stu-id="76f64-120">publishedFeedback</span></span>|[<span data-ttu-id="76f64-121">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="76f64-121">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="76f64-122">Копия свойства обратной связи, которая сделана при отсвойке класса учащемуся.</span><span class="sxs-lookup"><span data-stu-id="76f64-122">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76f64-123">Связи</span><span class="sxs-lookup"><span data-stu-id="76f64-123">Relationships</span></span>

<span data-ttu-id="76f64-124">Нет</span><span class="sxs-lookup"><span data-stu-id="76f64-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76f64-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76f64-125">JSON representation</span></span>

<span data-ttu-id="76f64-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76f64-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackOutcome",
  "keyProperty": "id"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "publishedFeedback": {"@odata.type": "microsoft.graph.educationFeedback"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedbackOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

