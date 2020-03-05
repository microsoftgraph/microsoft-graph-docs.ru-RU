---
title: Тип ресурса Едукатионфидбаккауткоме
description: Объект Едукатионауткоме, который дает отзыв в виде текста.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3dd9dd01c19306d66ac91578a5430ff26667b0e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502132"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="cae10-103">Тип ресурса Едукатионфидбаккауткоме</span><span class="sxs-lookup"><span data-stu-id="cae10-103">educationFeedbackOutcome resource type</span></span>

<span data-ttu-id="cae10-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cae10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cae10-105">Представляет обратную связь для объекта [едукатионауткоме](educationoutcome.md) в виде текста.</span><span class="sxs-lookup"><span data-stu-id="cae10-105">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="cae10-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cae10-106">Methods</span></span>

| <span data-ttu-id="cae10-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cae10-107">Method</span></span>       | <span data-ttu-id="cae10-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cae10-108">Return Type</span></span> | <span data-ttu-id="cae10-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cae10-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cae10-110">Обновление Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="cae10-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="cae10-111">едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="cae10-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="cae10-112">Обновление объекта Едукатионауткоме.</span><span class="sxs-lookup"><span data-stu-id="cae10-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cae10-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="cae10-113">Properties</span></span>

| <span data-ttu-id="cae10-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="cae10-114">Property</span></span>     | <span data-ttu-id="cae10-115">Тип</span><span class="sxs-lookup"><span data-stu-id="cae10-115">Type</span></span>        | <span data-ttu-id="cae10-116">Описание</span><span class="sxs-lookup"><span data-stu-id="cae10-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cae10-117">feedback</span><span class="sxs-lookup"><span data-stu-id="cae10-117">feedback</span></span>|[<span data-ttu-id="cae10-118">едукатионфидбакк</span><span class="sxs-lookup"><span data-stu-id="cae10-118">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="cae10-119">Письменный отзыв учащегося.</span><span class="sxs-lookup"><span data-stu-id="cae10-119">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="cae10-120">публишедфидбакк</span><span class="sxs-lookup"><span data-stu-id="cae10-120">publishedFeedback</span></span>|[<span data-ttu-id="cae10-121">едукатионфидбакк</span><span class="sxs-lookup"><span data-stu-id="cae10-121">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="cae10-122">Копия свойства обратной связи, выполняемого при отпадении оценки на учащийся.</span><span class="sxs-lookup"><span data-stu-id="cae10-122">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cae10-123">Связи</span><span class="sxs-lookup"><span data-stu-id="cae10-123">Relationships</span></span>

<span data-ttu-id="cae10-124">Нет</span><span class="sxs-lookup"><span data-stu-id="cae10-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cae10-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cae10-125">JSON representation</span></span>

<span data-ttu-id="cae10-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cae10-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackOutcome",
  "baseType": "",
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