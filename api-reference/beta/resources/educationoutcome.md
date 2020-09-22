---
title: Тип ресурса Едукатионауткоме
description: Результат ступенчатого задания
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 129e48b5d1101aaf9ab6ab7eb8c89a92b41a6ac7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081715"
---
# <a name="educationoutcome-resource-type"></a><span data-ttu-id="bb6e7-103">Тип ресурса Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="bb6e7-103">educationOutcome resource type</span></span>

<span data-ttu-id="bb6e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb6e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb6e7-105">Результат ступенчатого присваивания.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-105">The result of grading an assignment.</span></span> <span data-ttu-id="bb6e7-106">Это базовый класс; производные типы: [едукатионфидбаккауткоме](educationfeedbackoutcome.md), [едукатионпоинтсауткоме](educationpointsoutcome.md)и [едукатионрубрикауткоме](educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="bb6e7-106">This is a base class; the derived types are [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md), and [educationRubricOutcome](educationrubricoutcome.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bb6e7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bb6e7-107">Methods</span></span>

| <span data-ttu-id="bb6e7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="bb6e7-108">Method</span></span>       | <span data-ttu-id="bb6e7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bb6e7-109">Return Type</span></span> | <span data-ttu-id="bb6e7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bb6e7-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bb6e7-111">Обновление Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="bb6e7-111">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="bb6e7-112">едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="bb6e7-112">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="bb6e7-113">Обновление объекта Едукатионауткоме.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-113">Update educationOutcome object.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bb6e7-114">Связи</span><span class="sxs-lookup"><span data-stu-id="bb6e7-114">Relationships</span></span>

<span data-ttu-id="bb6e7-115">Нет</span><span class="sxs-lookup"><span data-stu-id="bb6e7-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb6e7-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb6e7-116">JSON representation</span></span>

<span data-ttu-id="bb6e7-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-117">The following is a JSON representation of the resource.</span></span>

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

