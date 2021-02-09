---
title: Тип ресурса educationFeedbackOutcome
description: EducationOutcome, который дает отзыв в виде текста.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1c50776f6b8dde27d8f937e8b7ee2028ce1cfca1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153657"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="9e9f9-103">Тип ресурса educationFeedbackOutcome</span><span class="sxs-lookup"><span data-stu-id="9e9f9-103">educationFeedbackOutcome resource type</span></span>

<span data-ttu-id="9e9f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e9f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e9f9-105">Представляет отзыв об [объекте educationOutcome](educationoutcome.md) в виде текста.</span><span class="sxs-lookup"><span data-stu-id="9e9f9-105">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="9e9f9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9e9f9-106">Methods</span></span>

| <span data-ttu-id="9e9f9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9e9f9-107">Method</span></span>       | <span data-ttu-id="9e9f9-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9e9f9-108">Return Type</span></span> | <span data-ttu-id="9e9f9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9e9f9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9e9f9-110">Обновление educationOutcome</span><span class="sxs-lookup"><span data-stu-id="9e9f9-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="9e9f9-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="9e9f9-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="9e9f9-112">Обновление объекта educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="9e9f9-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9e9f9-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e9f9-113">Properties</span></span>

| <span data-ttu-id="9e9f9-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e9f9-114">Property</span></span>     | <span data-ttu-id="9e9f9-115">Тип</span><span class="sxs-lookup"><span data-stu-id="9e9f9-115">Type</span></span>        | <span data-ttu-id="9e9f9-116">Описание</span><span class="sxs-lookup"><span data-stu-id="9e9f9-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e9f9-117">feedback</span><span class="sxs-lookup"><span data-stu-id="9e9f9-117">feedback</span></span>|[<span data-ttu-id="9e9f9-118">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="9e9f9-118">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="9e9f9-119">Письменный отзыв преподавателя для учащегося.</span><span class="sxs-lookup"><span data-stu-id="9e9f9-119">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="9e9f9-120">publishedFeedback</span><span class="sxs-lookup"><span data-stu-id="9e9f9-120">publishedFeedback</span></span>|[<span data-ttu-id="9e9f9-121">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="9e9f9-121">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="9e9f9-122">Копия свойства обратной связи, которая выдана учащемуся после выпуска оценки.</span><span class="sxs-lookup"><span data-stu-id="9e9f9-122">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e9f9-123">Связи</span><span class="sxs-lookup"><span data-stu-id="9e9f9-123">Relationships</span></span>

<span data-ttu-id="9e9f9-124">Нет</span><span class="sxs-lookup"><span data-stu-id="9e9f9-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e9f9-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e9f9-125">JSON representation</span></span>

<span data-ttu-id="9e9f9-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e9f9-126">The following is a JSON representation of the resource.</span></span>

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

