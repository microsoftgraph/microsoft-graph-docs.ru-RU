---
title: Тип ресурса Шифтпреференцес
description: Представляет доступность пользователя для назначения смен в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 75084cba71946d8b14ab080ac5872359bf0ceb12
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520613"
---
# <a name="shiftpreferences-resource-type"></a><span data-ttu-id="518fc-103">Тип ресурса Шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="518fc-103">shiftPreferences resource type</span></span>

<span data-ttu-id="518fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="518fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="518fc-105">Представляет доступность пользователя для назначения смен в [расписании](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="518fc-105">Represents a user's availability to be assigned shifts in the [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="518fc-106">Методы</span><span class="sxs-lookup"><span data-stu-id="518fc-106">Methods</span></span>

| <span data-ttu-id="518fc-107">Метод</span><span class="sxs-lookup"><span data-stu-id="518fc-107">Method</span></span>       | <span data-ttu-id="518fc-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="518fc-108">Return Type</span></span> | <span data-ttu-id="518fc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="518fc-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="518fc-110">[получение](../api/shiftpreferences-get.md);</span><span class="sxs-lookup"><span data-stu-id="518fc-110">[Get](../api/shiftpreferences-get.md)</span></span> | [<span data-ttu-id="518fc-111">шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="518fc-111">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="518fc-112">Чтение свойств и связей объекта **шифтпреференцес** .</span><span class="sxs-lookup"><span data-stu-id="518fc-112">Read the properties and relationships of a **shiftPreferences** object.</span></span> |
| <span data-ttu-id="518fc-113">[обновление](../api/shiftpreferences-put.md).</span><span class="sxs-lookup"><span data-stu-id="518fc-113">[Update](../api/shiftpreferences-put.md)</span></span> | [<span data-ttu-id="518fc-114">шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="518fc-114">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="518fc-115">Обновление объекта **шифтпреференцес** .</span><span class="sxs-lookup"><span data-stu-id="518fc-115">Update a **shiftPreferences** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="518fc-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="518fc-116">Properties</span></span>

|<span data-ttu-id="518fc-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="518fc-117">Property</span></span>          |<span data-ttu-id="518fc-118">Тип</span><span class="sxs-lookup"><span data-stu-id="518fc-118">Type</span></span>           |<span data-ttu-id="518fc-119">Описание</span><span class="sxs-lookup"><span data-stu-id="518fc-119">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="518fc-120">id</span><span class="sxs-lookup"><span data-stu-id="518fc-120">id</span></span> | `Edm.String` | <span data-ttu-id="518fc-121">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="518fc-121">The identifier of the entity.</span></span> |
| <span data-ttu-id="518fc-122">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="518fc-122">@odata.etag</span></span> | `Edm.String` | <span data-ttu-id="518fc-123">Ключ изменения для объекта.</span><span class="sxs-lookup"><span data-stu-id="518fc-123">The change key for the entity.</span></span> |
| <span data-ttu-id="518fc-124">availability</span><span class="sxs-lookup"><span data-stu-id="518fc-124">availability</span></span> | <span data-ttu-id="518fc-125">Коллекция [шифтаваилабилити](shiftavailability.md)</span><span class="sxs-lookup"><span data-stu-id="518fc-125">[shiftAvailability](shiftavailability.md) collection</span></span> | <span data-ttu-id="518fc-126">Доступность пользователя для планирования работы и расписания повторения.</span><span class="sxs-lookup"><span data-stu-id="518fc-126">Availability of the user to be scheduled for work and its recurrence pattern.</span></span> |
| <span data-ttu-id="518fc-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="518fc-127">createdDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="518fc-128">Временная метка, соответствующая моменту создания объекта.</span><span class="sxs-lookup"><span data-stu-id="518fc-128">Timestamp corresponding to when the entity was created.</span></span> |
| <span data-ttu-id="518fc-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="518fc-129">lastModifiedDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="518fc-130">Временная метка, соответствующая дате последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="518fc-130">Timestamp corresponding to when the entity was last modified.</span></span> |
| <span data-ttu-id="518fc-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="518fc-131">lastModifiedBy</span></span> | [<span data-ttu-id="518fc-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="518fc-132">identitySet</span></span>](identityset.md) | <span data-ttu-id="518fc-133">Идентификатор пользователя, который последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="518fc-133">Identity of the person who last modified the entity.</span></span> |

## <a name="relationships"></a><span data-ttu-id="518fc-134">Связи</span><span class="sxs-lookup"><span data-stu-id="518fc-134">Relationships</span></span>

<span data-ttu-id="518fc-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="518fc-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="518fc-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="518fc-136">JSON representation</span></span>

<span data-ttu-id="518fc-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="518fc-137">The following is a JSON representation of the resource.</span></span>

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
