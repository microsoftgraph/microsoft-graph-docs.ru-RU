---
title: Тип ресурса Location
description: Представляет сведения о месте проведения события.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bb975753e838d273c8d516472f1963d92413a367
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036431"
---
# <a name="location-resource-type"></a><span data-ttu-id="d21ca-103">Тип ресурса Location</span><span class="sxs-lookup"><span data-stu-id="d21ca-103">Location resource type</span></span>

<span data-ttu-id="d21ca-104">Представляет сведения о месте проведения [мероприятия](event.md).</span><span class="sxs-lookup"><span data-stu-id="d21ca-104">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="d21ca-105">Создавать события в календаре можно несколькими способами, например с помощью REST API [создания события](../api/user-post-events.md) в приложении либо вручную с помощью пользовательского интерфейса Outlook.</span><span class="sxs-lookup"><span data-stu-id="d21ca-105">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="d21ca-106">Создавая событие через пользовательский интерфейс, вы можете указать место проведения обычным текстом (например, "Бар «Окунь»") или выбрать его из списка помещений, предоставленного приложением Outlook, [Автозаполнением Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) или [локальным поиском Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="d21ca-106">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="d21ca-107">В зависимости от того, как создано событие, Outlook может по-разному задавать доступное только для чтения свойство **locationType**.</span><span class="sxs-lookup"><span data-stu-id="d21ca-107">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="d21ca-108">Способ создания события</span><span class="sxs-lookup"><span data-stu-id="d21ca-108">How event was created</span></span>  | <span data-ttu-id="d21ca-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d21ca-109">Property</span></span>   | <span data-ttu-id="d21ca-110">Ожидаемое значение</span><span class="sxs-lookup"><span data-stu-id="d21ca-110">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="d21ca-111">REST API [создания события](../api/user-post-events.md)</span><span class="sxs-lookup"><span data-stu-id="d21ca-111">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="d21ca-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="d21ca-112">**locationType**</span></span> | `default` |
| <span data-ttu-id="d21ca-113">Пользовательский интерфейс Outlook</span><span class="sxs-lookup"><span data-stu-id="d21ca-113">User interface in Outlook</span></span> | <span data-ttu-id="d21ca-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="d21ca-114">**locationType**</span></span> | <span data-ttu-id="d21ca-115">Одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="d21ca-115">One of the following:</span></span> <ul><li><span data-ttu-id="d21ca-116">`default` для расположения, указанного обычным текстом;</span><span class="sxs-lookup"><span data-stu-id="d21ca-116">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="d21ca-117">`conferenceRoom` для помещения из списка в Outlook;</span><span class="sxs-lookup"><span data-stu-id="d21ca-117">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="d21ca-118">любое из значений `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness` и `postalAddress` для расположения из Автозаполнения Bing или локального поиска Bing.</span><span class="sxs-lookup"><span data-stu-id="d21ca-118">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |

## <a name="properties"></a><span data-ttu-id="d21ca-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="d21ca-119">Properties</span></span>
| <span data-ttu-id="d21ca-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="d21ca-120">Property</span></span>  | <span data-ttu-id="d21ca-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d21ca-121">Type</span></span>   | <span data-ttu-id="d21ca-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d21ca-122">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="d21ca-123">address</span><span class="sxs-lookup"><span data-stu-id="d21ca-123">address</span></span> | [<span data-ttu-id="d21ca-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="d21ca-124">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="d21ca-125">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="d21ca-125">The street address of the location.</span></span> |
| <span data-ttu-id="d21ca-126">coordinates</span><span class="sxs-lookup"><span data-stu-id="d21ca-126">coordinates</span></span> | [<span data-ttu-id="d21ca-127">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="d21ca-127">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="d21ca-128">Географические координаты и высота расположения.</span><span class="sxs-lookup"><span data-stu-id="d21ca-128">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="d21ca-129">displayName</span><span class="sxs-lookup"><span data-stu-id="d21ca-129">displayName</span></span>  | <span data-ttu-id="d21ca-130">String</span><span class="sxs-lookup"><span data-stu-id="d21ca-130">String</span></span> | <span data-ttu-id="d21ca-131">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="d21ca-131">The name associated with the location.</span></span>                       |
| <span data-ttu-id="d21ca-132">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d21ca-132">locationEmailAddress</span></span> | <span data-ttu-id="d21ca-133">String</span><span class="sxs-lookup"><span data-stu-id="d21ca-133">String</span></span> | <span data-ttu-id="d21ca-134">Необязательный электронный адрес для расположения.</span><span class="sxs-lookup"><span data-stu-id="d21ca-134">Optional email address of the location.</span></span>              |
| <span data-ttu-id="d21ca-135">locationUri</span><span class="sxs-lookup"><span data-stu-id="d21ca-135">locationUri</span></span> | <span data-ttu-id="d21ca-136">String</span><span class="sxs-lookup"><span data-stu-id="d21ca-136">String</span></span> | <span data-ttu-id="d21ca-137">Необязательный URI, представляющий местоположение.</span><span class="sxs-lookup"><span data-stu-id="d21ca-137">Optional URI representing the location.</span></span> |
| <span data-ttu-id="d21ca-138">locationType</span><span class="sxs-lookup"><span data-stu-id="d21ca-138">locationType</span></span> | <span data-ttu-id="d21ca-139">locationType</span><span class="sxs-lookup"><span data-stu-id="d21ca-139">locationType</span></span> | <span data-ttu-id="d21ca-140">Тип расположения.</span><span class="sxs-lookup"><span data-stu-id="d21ca-140">The type of location.</span></span> <span data-ttu-id="d21ca-141">Возможные `default`значения:, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`,. `postalAddress`</span><span class="sxs-lookup"><span data-stu-id="d21ca-141">The possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="d21ca-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d21ca-142">Read-only.</span></span>|
| <span data-ttu-id="d21ca-143">uniqueId</span><span class="sxs-lookup"><span data-stu-id="d21ca-143">uniqueId</span></span> | <span data-ttu-id="d21ca-144">String</span><span class="sxs-lookup"><span data-stu-id="d21ca-144">String</span></span> | <span data-ttu-id="d21ca-145">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="d21ca-145">For internal use only.</span></span>|
| <span data-ttu-id="d21ca-146">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="d21ca-146">uniqueIdType</span></span> | <span data-ttu-id="d21ca-147">Локатионуникуеидтипе</span><span class="sxs-lookup"><span data-stu-id="d21ca-147">locationUniqueIdType</span></span> | <span data-ttu-id="d21ca-148">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="d21ca-148">For internal use only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d21ca-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d21ca-149">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string",
  "locationType": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
