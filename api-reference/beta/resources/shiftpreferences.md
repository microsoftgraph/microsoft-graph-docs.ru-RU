---
title: Тип ресурса Шифтпреференцес
description: Представляет доступность пользователя для назначения смен в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d35f77e7d048adb0b0bb49604423bbe2ff53031c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058044"
---
# <a name="shiftpreferences-resource-type"></a><span data-ttu-id="801fa-103">Тип ресурса Шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="801fa-103">shiftPreferences resource type</span></span>

<span data-ttu-id="801fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="801fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="801fa-105">Представляет доступность пользователя для назначения смен в [расписании](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="801fa-105">Represents a user's availability to be assigned shifts in the [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="801fa-106">Методы</span><span class="sxs-lookup"><span data-stu-id="801fa-106">Methods</span></span>

| <span data-ttu-id="801fa-107">Метод</span><span class="sxs-lookup"><span data-stu-id="801fa-107">Method</span></span>       | <span data-ttu-id="801fa-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="801fa-108">Return Type</span></span> | <span data-ttu-id="801fa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="801fa-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="801fa-110">Получение</span><span class="sxs-lookup"><span data-stu-id="801fa-110">Get</span></span>](../api/shiftpreferences-get.md) | [<span data-ttu-id="801fa-111">шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="801fa-111">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="801fa-112">Чтение свойств и связей объекта **шифтпреференцес** .</span><span class="sxs-lookup"><span data-stu-id="801fa-112">Read the properties and relationships of a **shiftPreferences** object.</span></span> |
| [<span data-ttu-id="801fa-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="801fa-113">Update</span></span>](../api/shiftpreferences-put.md) | [<span data-ttu-id="801fa-114">шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="801fa-114">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="801fa-115">Обновление объекта **шифтпреференцес** .</span><span class="sxs-lookup"><span data-stu-id="801fa-115">Update a **shiftPreferences** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="801fa-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="801fa-116">Properties</span></span>

|<span data-ttu-id="801fa-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="801fa-117">Property</span></span>          |<span data-ttu-id="801fa-118">Тип</span><span class="sxs-lookup"><span data-stu-id="801fa-118">Type</span></span>           |<span data-ttu-id="801fa-119">Описание</span><span class="sxs-lookup"><span data-stu-id="801fa-119">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="801fa-120">id</span><span class="sxs-lookup"><span data-stu-id="801fa-120">id</span></span> | `Edm.String` | <span data-ttu-id="801fa-121">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="801fa-121">The identifier of the entity.</span></span> |
| <span data-ttu-id="801fa-122">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="801fa-122">@odata.etag</span></span> | `Edm.String` | <span data-ttu-id="801fa-123">Ключ изменения для объекта.</span><span class="sxs-lookup"><span data-stu-id="801fa-123">The change key for the entity.</span></span> |
| <span data-ttu-id="801fa-124">availability</span><span class="sxs-lookup"><span data-stu-id="801fa-124">availability</span></span> | <span data-ttu-id="801fa-125">Коллекция [шифтаваилабилити](shiftavailability.md)</span><span class="sxs-lookup"><span data-stu-id="801fa-125">[shiftAvailability](shiftavailability.md) collection</span></span> | <span data-ttu-id="801fa-126">Доступность пользователя для планирования работы и расписания повторения.</span><span class="sxs-lookup"><span data-stu-id="801fa-126">Availability of the user to be scheduled for work and its recurrence pattern.</span></span> |
| <span data-ttu-id="801fa-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="801fa-127">createdDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="801fa-128">Временная метка, соответствующая моменту создания объекта.</span><span class="sxs-lookup"><span data-stu-id="801fa-128">Timestamp corresponding to when the entity was created.</span></span> |
| <span data-ttu-id="801fa-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="801fa-129">lastModifiedDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="801fa-130">Временная метка, соответствующая дате последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="801fa-130">Timestamp corresponding to when the entity was last modified.</span></span> |
| <span data-ttu-id="801fa-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="801fa-131">lastModifiedBy</span></span> | [<span data-ttu-id="801fa-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="801fa-132">identitySet</span></span>](identityset.md) | <span data-ttu-id="801fa-133">Идентификатор пользователя, который последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="801fa-133">Identity of the person who last modified the entity.</span></span> |

## <a name="relationships"></a><span data-ttu-id="801fa-134">Связи</span><span class="sxs-lookup"><span data-stu-id="801fa-134">Relationships</span></span>

<span data-ttu-id="801fa-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="801fa-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="801fa-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="801fa-136">JSON representation</span></span>

<span data-ttu-id="801fa-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="801fa-137">The following is a JSON representation of the resource.</span></span>

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


