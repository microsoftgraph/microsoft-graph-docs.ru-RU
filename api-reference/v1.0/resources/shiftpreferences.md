---
title: Тип ресурса Шифтпреференцес
description: Представляет доступность пользователя для назначения смен в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 91a6093ad66d906fe9917ae7a22d2297ded4b4d7
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154859"
---
# <a name="shiftpreferences-resource-type"></a><span data-ttu-id="c3001-103">Тип ресурса Шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="c3001-103">shiftPreferences resource type</span></span>

<span data-ttu-id="c3001-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3001-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3001-105">Представляет доступность пользователя для назначения смен в [расписании](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="c3001-105">Represents a user's availability to be assigned shifts in the [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c3001-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c3001-106">Methods</span></span>

| <span data-ttu-id="c3001-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c3001-107">Method</span></span>       | <span data-ttu-id="c3001-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c3001-108">Return Type</span></span> | <span data-ttu-id="c3001-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c3001-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c3001-110">[получение](../api/shiftpreferences-get.md);</span><span class="sxs-lookup"><span data-stu-id="c3001-110">[Get](../api/shiftpreferences-get.md)</span></span> | [<span data-ttu-id="c3001-111">шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="c3001-111">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="c3001-112">Чтение свойств и связей объекта **шифтпреференцес** .</span><span class="sxs-lookup"><span data-stu-id="c3001-112">Read the properties and relationships of a **shiftPreferences** object.</span></span> |
| <span data-ttu-id="c3001-113">[обновление](../api/shiftpreferences-put.md).</span><span class="sxs-lookup"><span data-stu-id="c3001-113">[Update](../api/shiftpreferences-put.md)</span></span> | [<span data-ttu-id="c3001-114">шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="c3001-114">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="c3001-115">Обновление объекта **шифтпреференцес** .</span><span class="sxs-lookup"><span data-stu-id="c3001-115">Update a **shiftPreferences** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c3001-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3001-116">Properties</span></span>

|<span data-ttu-id="c3001-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3001-117">Property</span></span>          |<span data-ttu-id="c3001-118">Тип</span><span class="sxs-lookup"><span data-stu-id="c3001-118">Type</span></span>           |<span data-ttu-id="c3001-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c3001-119">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c3001-120">id</span><span class="sxs-lookup"><span data-stu-id="c3001-120">id</span></span> | `Edm.String` | <span data-ttu-id="c3001-121">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="c3001-121">The identifier of the entity.</span></span> |
| <span data-ttu-id="c3001-122">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="c3001-122">@odata.etag</span></span> | `Edm.String` | <span data-ttu-id="c3001-123">Ключ изменения для объекта.</span><span class="sxs-lookup"><span data-stu-id="c3001-123">The change key for the entity.</span></span> |
| <span data-ttu-id="c3001-124">availability</span><span class="sxs-lookup"><span data-stu-id="c3001-124">availability</span></span> | <span data-ttu-id="c3001-125">Коллекция [шифтаваилабилити](shiftavailability.md)</span><span class="sxs-lookup"><span data-stu-id="c3001-125">[shiftAvailability](shiftavailability.md) collection</span></span> | <span data-ttu-id="c3001-126">Доступность пользователя для планирования работы и расписания повторения.</span><span class="sxs-lookup"><span data-stu-id="c3001-126">Availability of the user to be scheduled for work and its recurrence pattern.</span></span> |
| <span data-ttu-id="c3001-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3001-127">createdDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="c3001-128">Временная метка, соответствующая моменту создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c3001-128">Timestamp corresponding to when the entity was created.</span></span> |
| <span data-ttu-id="c3001-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3001-129">lastModifiedDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="c3001-130">Временная метка, соответствующая дате последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c3001-130">Timestamp corresponding to when the entity was last modified.</span></span> |
| <span data-ttu-id="c3001-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c3001-131">lastModifiedBy</span></span> | [<span data-ttu-id="c3001-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="c3001-132">identitySet</span></span>](identityset.md) | <span data-ttu-id="c3001-133">Идентификатор пользователя, который последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="c3001-133">Identity of the person who last modified the entity.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c3001-134">Связи</span><span class="sxs-lookup"><span data-stu-id="c3001-134">Relationships</span></span>

<span data-ttu-id="c3001-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c3001-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3001-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c3001-136">JSON representation</span></span>

<span data-ttu-id="c3001-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3001-137">The following is a JSON representation of the resource.</span></span>

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
