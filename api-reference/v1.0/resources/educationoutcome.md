---
title: тип ресурсов educationOutcome
description: Результат классификации назначения.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5333b6228b44da1ab0364741fa2b602534fcf9ce
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912804"
---
# <a name="educationoutcome-resource-type"></a><span data-ttu-id="93e8a-103">тип ресурсов educationOutcome</span><span class="sxs-lookup"><span data-stu-id="93e8a-103">educationOutcome resource type</span></span>

<span data-ttu-id="93e8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93e8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93e8a-105">Результат классификации назначения.</span><span class="sxs-lookup"><span data-stu-id="93e8a-105">The result of grading an assignment.</span></span> 

<span data-ttu-id="93e8a-106">Это базовый класс; производными типами являются [educationFeedbackOutcome,](educationfeedbackoutcome.md) [educationPointsOutcome](educationpointsoutcome.md)и [educationRubricOutcome.](educationrubricoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="93e8a-106">This is a base class; the derived types are [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md), and [educationRubricOutcome](educationrubricoutcome.md).</span></span>

## <a name="methods"></a><span data-ttu-id="93e8a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="93e8a-107">Methods</span></span>

| <span data-ttu-id="93e8a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="93e8a-108">Method</span></span>       | <span data-ttu-id="93e8a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="93e8a-109">Return Type</span></span> | <span data-ttu-id="93e8a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="93e8a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="93e8a-111">Обновление educationOutcome</span><span class="sxs-lookup"><span data-stu-id="93e8a-111">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="93e8a-112">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="93e8a-112">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="93e8a-113">Обновление объекта educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="93e8a-113">Update educationOutcome object.</span></span> |

## <a name="relationships"></a><span data-ttu-id="93e8a-114">Связи</span><span class="sxs-lookup"><span data-stu-id="93e8a-114">Relationships</span></span>

<span data-ttu-id="93e8a-115">Нет</span><span class="sxs-lookup"><span data-stu-id="93e8a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93e8a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93e8a-116">JSON representation</span></span>

<span data-ttu-id="93e8a-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93e8a-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOutcome",
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

