---
title: Тип ресурса plannerPlanContextCollection
description: Ресурс **plannerPlanContextCollection** представляет коллекцию внешних контекстах, с которыми связан плана. Этот ресурс является открытым и является частью объекта plannerPlan. Значение в паре значение свойства — это объект plannerPlanContext.
localization_priority: Normal
ms.openlocfilehash: 51a09353993a61324f31a03c8ffadd5462cac692
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805455"
---
# <a name="plannerplancontextcollection-resource-type"></a><span data-ttu-id="01176-105">Тип ресурса plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="01176-105">plannerPlanContextCollection resource type</span></span>

> <span data-ttu-id="01176-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01176-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01176-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01176-107">Use of these APIs in production applications is not supported.</span></span>


<span data-ttu-id="01176-108">Ресурс **plannerPlanContextCollection** представляет коллекцию внешних контекстах, с которыми связан плана.</span><span class="sxs-lookup"><span data-stu-id="01176-108">The **plannerPlanContextCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="01176-109">Этот ресурс является открытым и является частью объекта [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="01176-109">This resource is an open type and is part of the [plannerPlan](plannerplan.md) object.</span></span> <span data-ttu-id="01176-110">Значение в паре значение свойства — это объект [plannerPlanContext](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="01176-110">The value in the property-value pair is the [plannerPlanContext](plannerplancontext.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="01176-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="01176-111">Properties</span></span>
<span data-ttu-id="01176-112">Можно определить свойства этого типа open.</span><span class="sxs-lookup"><span data-stu-id="01176-112">You can define the properties of this open type.</span></span> <span data-ttu-id="01176-113">Значения свойства должны быть особый идентификатор, представляющий внешнего контекста как имя свойства.</span><span class="sxs-lookup"><span data-stu-id="01176-113">The property values should be distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="01176-114">Значения свойства должны быть [plannerPlanContext](plannerplancontext.md) объектов.</span><span class="sxs-lookup"><span data-stu-id="01176-114">The property values must be [plannerPlanContext](plannerplancontext.md) objects.</span></span> <span data-ttu-id="01176-115">На основании требований к OData, имена свойств в открытые типы не может содержать следующие символы: `.`, `:`, `%`, `@`.</span><span class="sxs-lookup"><span data-stu-id="01176-115">Based on OData requirements, property names in open types cannot contain the following characters: `.`, `:`, `%`, `@`.</span></span> <span data-ttu-id="01176-116">Эти символы должны быть закодированы с помощью Кодировка URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="01176-116">These characters need to be encoded using URL encoding.</span></span> <span data-ttu-id="01176-117">Чтобы удалить элемент в списке "Избранное", задайте значение свойства, которое должно `null`.</span><span class="sxs-lookup"><span data-stu-id="01176-117">To remove an item in the favorites list, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="01176-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01176-118">JSON representation</span></span>

<span data-ttu-id="01176-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01176-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
