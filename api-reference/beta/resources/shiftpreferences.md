---
title: Тип ресурса Шифтпреференцес
description: Представляет доступность пользователя для назначения смен в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 083b0ad81ffee25d8a03bf5ff38815d2ca0155a8
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952274"
---
# <a name="shiftpreferences-resource-type"></a><span data-ttu-id="4e36b-103">Тип ресурса Шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="4e36b-103">shiftPreferences resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e36b-104">Представляет доступность пользователя для назначения смен в [расписании](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="4e36b-104">Represents a user's availability to be assigned shifts in the [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4e36b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="4e36b-105">Methods</span></span>

| <span data-ttu-id="4e36b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="4e36b-106">Method</span></span>       | <span data-ttu-id="4e36b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e36b-107">Return Type</span></span> | <span data-ttu-id="4e36b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4e36b-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4e36b-109">[получение](../api/shiftpreferences-get.md);</span><span class="sxs-lookup"><span data-stu-id="4e36b-109">[Get](../api/shiftpreferences-get.md)</span></span> | [<span data-ttu-id="4e36b-110">шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="4e36b-110">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="4e36b-111">Чтение свойств и связей объекта **шифтпреференцес** .</span><span class="sxs-lookup"><span data-stu-id="4e36b-111">Read the properties and relationships of a **shiftPreferences** object.</span></span> |
| <span data-ttu-id="4e36b-112">[обновление](../api/shiftpreferences-put.md).</span><span class="sxs-lookup"><span data-stu-id="4e36b-112">[Update](../api/shiftpreferences-put.md)</span></span> | [<span data-ttu-id="4e36b-113">шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="4e36b-113">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="4e36b-114">Обновление объекта **шифтпреференцес** .</span><span class="sxs-lookup"><span data-stu-id="4e36b-114">Update a **shiftPreferences** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4e36b-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e36b-115">Properties</span></span>

|<span data-ttu-id="4e36b-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e36b-116">Property</span></span>          |<span data-ttu-id="4e36b-117">Тип</span><span class="sxs-lookup"><span data-stu-id="4e36b-117">Type</span></span>           |<span data-ttu-id="4e36b-118">Описание</span><span class="sxs-lookup"><span data-stu-id="4e36b-118">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4e36b-119">id</span><span class="sxs-lookup"><span data-stu-id="4e36b-119">id</span></span> | `Edm.String` | <span data-ttu-id="4e36b-120">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="4e36b-120">The identifier of the entity.</span></span> |
| <span data-ttu-id="4e36b-121">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="4e36b-121">@odata.etag</span></span> | `Edm.String` | <span data-ttu-id="4e36b-122">Ключ изменения для объекта.</span><span class="sxs-lookup"><span data-stu-id="4e36b-122">The change key for the entity.</span></span> |
| <span data-ttu-id="4e36b-123">availability</span><span class="sxs-lookup"><span data-stu-id="4e36b-123">availability</span></span> | <span data-ttu-id="4e36b-124">Коллекция [шифтаваилабилити](shiftavailability.md)</span><span class="sxs-lookup"><span data-stu-id="4e36b-124">[shiftAvailability](shiftavailability.md) collection</span></span> | <span data-ttu-id="4e36b-125">Доступность пользователя для планирования работы и расписания повторения.</span><span class="sxs-lookup"><span data-stu-id="4e36b-125">Availability of the user to be scheduled for work and its recurrence pattern.</span></span> |
| <span data-ttu-id="4e36b-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e36b-126">createdDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="4e36b-127">Временная метка, соответствующая моменту создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4e36b-127">Timestamp corresponding to when the entity was created.</span></span> |
| <span data-ttu-id="4e36b-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e36b-128">lastModifiedDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="4e36b-129">Временная метка, соответствующая дате последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4e36b-129">Timestamp corresponding to when the entity was last modified.</span></span> |
| <span data-ttu-id="4e36b-130">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4e36b-130">lastModifiedBy</span></span> | [<span data-ttu-id="4e36b-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="4e36b-131">identitySet</span></span>](identityset.md) | <span data-ttu-id="4e36b-132">Идентификатор пользователя, который последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="4e36b-132">Identity of the person who last modified the entity.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4e36b-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="4e36b-133">Relationships</span></span>

<span data-ttu-id="4e36b-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4e36b-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e36b-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4e36b-135">JSON representation</span></span>

<span data-ttu-id="4e36b-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e36b-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftPreferences",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "availability": [{"@odata.type": "microsoft.graph.shiftAvailability"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftPreferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
