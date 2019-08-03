---
title: Тип ресурса Едукатионфидбаккауткоме
description: Объект Едукатионауткоме, который дает отзыв в виде текста.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e61538a62a1bb267b0a13b98b17e9b69a8ceed92
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173253"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="0b8cc-103">Тип ресурса Едукатионфидбаккауткоме</span><span class="sxs-lookup"><span data-stu-id="0b8cc-103">educationFeedbackOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b8cc-104">Представляет обратную связь для объекта [едукатионауткоме](educationoutcome.md) в виде текста.</span><span class="sxs-lookup"><span data-stu-id="0b8cc-104">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="0b8cc-105">Методы</span><span class="sxs-lookup"><span data-stu-id="0b8cc-105">Methods</span></span>

| <span data-ttu-id="0b8cc-106">Метод</span><span class="sxs-lookup"><span data-stu-id="0b8cc-106">Method</span></span>       | <span data-ttu-id="0b8cc-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0b8cc-107">Return Type</span></span> | <span data-ttu-id="0b8cc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0b8cc-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0b8cc-109">Обновление Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="0b8cc-109">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="0b8cc-110">Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="0b8cc-110">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="0b8cc-111">Обновление объекта Едукатионауткоме.</span><span class="sxs-lookup"><span data-stu-id="0b8cc-111">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0b8cc-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b8cc-112">Properties</span></span>

| <span data-ttu-id="0b8cc-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b8cc-113">Property</span></span>     | <span data-ttu-id="0b8cc-114">Тип</span><span class="sxs-lookup"><span data-stu-id="0b8cc-114">Type</span></span>        | <span data-ttu-id="0b8cc-115">Описание</span><span class="sxs-lookup"><span data-stu-id="0b8cc-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b8cc-116">feedback</span><span class="sxs-lookup"><span data-stu-id="0b8cc-116">feedback</span></span>|[<span data-ttu-id="0b8cc-117">Едукатионфидбакк</span><span class="sxs-lookup"><span data-stu-id="0b8cc-117">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="0b8cc-118">Письменный отзыв учащегося.</span><span class="sxs-lookup"><span data-stu-id="0b8cc-118">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="0b8cc-119">Публишедфидбакк</span><span class="sxs-lookup"><span data-stu-id="0b8cc-119">publishedFeedback</span></span>|[<span data-ttu-id="0b8cc-120">Едукатионфидбакк</span><span class="sxs-lookup"><span data-stu-id="0b8cc-120">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="0b8cc-121">Копия свойства обратной связи, выполняемого при отпадении оценки на учащийся.</span><span class="sxs-lookup"><span data-stu-id="0b8cc-121">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b8cc-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="0b8cc-122">Relationships</span></span>

<span data-ttu-id="0b8cc-123">Нет</span><span class="sxs-lookup"><span data-stu-id="0b8cc-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b8cc-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b8cc-124">JSON representation</span></span>

<span data-ttu-id="0b8cc-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b8cc-125">The following is a JSON representation of the resource.</span></span>

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