---
title: Тип ресурса Планнерпланконтекстколлектион
description: Ресурс **планнерпланконтекстколлектион** представляет коллекцию внешних контекстов, с которыми связан план. Этот ресурс является открытым типом и является частью объекта plannerPlan. Значение в параметре "свойство-значение" является объектом Планнерпланконтекст.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 7cd887838cf51a46f1475a39566c65c8b8b922ea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521701"
---
# <a name="plannerplancontextcollection-resource-type"></a><span data-ttu-id="b3b38-105">Тип ресурса Планнерпланконтекстколлектион</span><span class="sxs-lookup"><span data-stu-id="b3b38-105">plannerPlanContextCollection resource type</span></span>

<span data-ttu-id="b3b38-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3b38-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="b3b38-107">Ресурс **планнерпланконтекстколлектион** представляет коллекцию внешних контекстов, с которыми связан план.</span><span class="sxs-lookup"><span data-stu-id="b3b38-107">The **plannerPlanContextCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="b3b38-108">Этот ресурс является открытым типом и является частью объекта [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="b3b38-108">This resource is an open type and is part of the [plannerPlan](plannerplan.md) object.</span></span> <span data-ttu-id="b3b38-109">Значение в параметре "свойство-значение" является объектом [планнерпланконтекст](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="b3b38-109">The value in the property-value pair is the [plannerPlanContext](plannerplancontext.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="b3b38-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3b38-110">Properties</span></span>
<span data-ttu-id="b3b38-111">Вы можете определить свойства этого открытого типа.</span><span class="sxs-lookup"><span data-stu-id="b3b38-111">You can define the properties of this open type.</span></span> <span data-ttu-id="b3b38-112">Значения свойств должны представлять собой отличительный идентификатор, представляющий внешний контекст в качестве имени свойства.</span><span class="sxs-lookup"><span data-stu-id="b3b38-112">The property values should be distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="b3b38-113">Значения свойств должны быть [планнерпланконтекст](plannerplancontext.md) объектами.</span><span class="sxs-lookup"><span data-stu-id="b3b38-113">The property values must be [plannerPlanContext](plannerplancontext.md) objects.</span></span> <span data-ttu-id="b3b38-114">В зависимости от требований OData имена свойств в открытых типах не могут содержать следующие символы: `.`, `:`, `%`, `@`.</span><span class="sxs-lookup"><span data-stu-id="b3b38-114">Based on OData requirements, property names in open types cannot contain the following characters: `.`, `:`, `%`, `@`.</span></span> <span data-ttu-id="b3b38-115">Эти символы необходимо закодировать с помощью URL-кодировки.</span><span class="sxs-lookup"><span data-stu-id="b3b38-115">These characters need to be encoded using URL encoding.</span></span> <span data-ttu-id="b3b38-116">Чтобы удалить элемент из списка "Избранное", присвойте свойству значение `null`.</span><span class="sxs-lookup"><span data-stu-id="b3b38-116">To remove an item in the favorites list, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3b38-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3b38-117">JSON representation</span></span>

<span data-ttu-id="b3b38-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3b38-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextCollection"
}-->

```json
{
  "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
    "@odata.type": "#microsoft.graph.plannerPlanContext",
    "associationType": "Board",
    "createdDateTime": "2015-10-14T00:57:28.4698344Z",
    "displayNameSegments": [
        "Finance Team",
        "Budget Plans"
    ],
    "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
