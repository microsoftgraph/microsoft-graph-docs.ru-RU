---
title: Тип ресурса educationOutcome
description: Результат классификации назначения
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 788985e5e63272fea31e579c2da4472ec065dfc5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153633"
---
# <a name="educationoutcome-resource-type"></a><span data-ttu-id="df9d9-103">Тип ресурса educationOutcome</span><span class="sxs-lookup"><span data-stu-id="df9d9-103">educationOutcome resource type</span></span>

<span data-ttu-id="df9d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df9d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df9d9-105">Результат классификации назначения.</span><span class="sxs-lookup"><span data-stu-id="df9d9-105">The result of grading an assignment.</span></span> <span data-ttu-id="df9d9-106">Это базовый класс; производными типами являются [educationFeedbackOutcome,](educationfeedbackoutcome.md) [educationPointsOutcome](educationpointsoutcome.md)и [educationRubricOutcome.](educationrubricoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="df9d9-106">This is a base class; the derived types are [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md), and [educationRubricOutcome](educationrubricoutcome.md).</span></span>

## <a name="methods"></a><span data-ttu-id="df9d9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="df9d9-107">Methods</span></span>

| <span data-ttu-id="df9d9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="df9d9-108">Method</span></span>       | <span data-ttu-id="df9d9-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="df9d9-109">Return Type</span></span> | <span data-ttu-id="df9d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="df9d9-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="df9d9-111">Обновление educationOutcome</span><span class="sxs-lookup"><span data-stu-id="df9d9-111">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="df9d9-112">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="df9d9-112">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="df9d9-113">Обновление объекта educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="df9d9-113">Update educationOutcome object.</span></span> |

## <a name="relationships"></a><span data-ttu-id="df9d9-114">Связи</span><span class="sxs-lookup"><span data-stu-id="df9d9-114">Relationships</span></span>

<span data-ttu-id="df9d9-115">Нет</span><span class="sxs-lookup"><span data-stu-id="df9d9-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df9d9-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df9d9-116">JSON representation</span></span>

<span data-ttu-id="df9d9-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df9d9-117">The following is a JSON representation of the resource.</span></span>

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

