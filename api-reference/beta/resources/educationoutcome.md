---
title: Тип ресурса Едукатионауткоме
description: Результат ступенчатого задания
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a0a49b9a383f1e787fd2698c6d2011e11b3abedb
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173365"
---
# <a name="educationoutcome-resource-type"></a><span data-ttu-id="8fb4a-103">Тип ресурса Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="8fb4a-103">educationOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fb4a-104">Результат ступенчатого присваивания.</span><span class="sxs-lookup"><span data-stu-id="8fb4a-104">The result of grading an assignment.</span></span> <span data-ttu-id="8fb4a-105">Это базовый класс; производные типы: [едукатионфидбаккауткоме](educationfeedbackoutcome.md), [едукатионпоинтсауткоме](educationpointsoutcome.md)и [едукатионрубрикауткоме](educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="8fb4a-105">This is a base class; the derived types are [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md), and [educationRubricOutcome](educationrubricoutcome.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8fb4a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8fb4a-106">Methods</span></span>

| <span data-ttu-id="8fb4a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8fb4a-107">Method</span></span>       | <span data-ttu-id="8fb4a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8fb4a-108">Return Type</span></span> | <span data-ttu-id="8fb4a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8fb4a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8fb4a-110">Обновление Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="8fb4a-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="8fb4a-111">Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="8fb4a-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="8fb4a-112">Обновление объекта Едукатионауткоме.</span><span class="sxs-lookup"><span data-stu-id="8fb4a-112">Update educationOutcome object.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8fb4a-113">Отношения</span><span class="sxs-lookup"><span data-stu-id="8fb4a-113">Relationships</span></span>

<span data-ttu-id="8fb4a-114">Нет</span><span class="sxs-lookup"><span data-stu-id="8fb4a-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fb4a-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8fb4a-115">JSON representation</span></span>

<span data-ttu-id="8fb4a-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fb4a-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->