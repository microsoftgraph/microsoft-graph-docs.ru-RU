---
title: Тип ресурса Location
description: Представляет сведения о месте проведения события.
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 9b590d011570981fd926a5e12a8c89e6059b3b41
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522920"
---
# <a name="location-resource-type"></a><span data-ttu-id="68361-103">Тип ресурса Location</span><span class="sxs-lookup"><span data-stu-id="68361-103">Location resource type</span></span>

<span data-ttu-id="68361-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="68361-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68361-105">Представляет сведения о месте проведения [мероприятия](event.md).</span><span class="sxs-lookup"><span data-stu-id="68361-105">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="68361-106">Создавать события в календаре можно несколькими способами, например с помощью REST API [создания события](../api/user-post-events.md) в приложении либо вручную с помощью пользовательского интерфейса Outlook.</span><span class="sxs-lookup"><span data-stu-id="68361-106">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="68361-107">Создавая событие через пользовательский интерфейс, вы можете указать место проведения обычным текстом (например, "Бар «Окунь»") или выбрать его из списка помещений, предоставленного приложением Outlook, [Автозаполнением Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) или [локальным поиском Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="68361-107">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="68361-108">В зависимости от того, как создано событие, Outlook может по-разному задавать доступное только для чтения свойство **locationType**.</span><span class="sxs-lookup"><span data-stu-id="68361-108">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="68361-109">Способ создания события</span><span class="sxs-lookup"><span data-stu-id="68361-109">How event was created</span></span>  | <span data-ttu-id="68361-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="68361-110">Property</span></span>   | <span data-ttu-id="68361-111">Ожидаемое значение</span><span class="sxs-lookup"><span data-stu-id="68361-111">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="68361-112">REST API [создания события](../api/user-post-events.md)</span><span class="sxs-lookup"><span data-stu-id="68361-112">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="68361-113">**locationType**</span><span class="sxs-lookup"><span data-stu-id="68361-113">**locationType**</span></span> | `default` |
| <span data-ttu-id="68361-114">Пользовательский интерфейс Outlook</span><span class="sxs-lookup"><span data-stu-id="68361-114">User interface in Outlook</span></span> | <span data-ttu-id="68361-115">**locationType**</span><span class="sxs-lookup"><span data-stu-id="68361-115">**locationType**</span></span> | <span data-ttu-id="68361-116">Одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="68361-116">One of the following:</span></span> <ul><li><span data-ttu-id="68361-117">`default` для расположения, указанного обычным текстом;</span><span class="sxs-lookup"><span data-stu-id="68361-117">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="68361-118">`conferenceRoom` для помещения из списка в Outlook;</span><span class="sxs-lookup"><span data-stu-id="68361-118">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="68361-119">любое из значений `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness` и `postalAddress` для расположения из Автозаполнения Bing или локального поиска Bing.</span><span class="sxs-lookup"><span data-stu-id="68361-119">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="68361-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="68361-120">Properties</span></span>
| <span data-ttu-id="68361-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="68361-121">Property</span></span>  | <span data-ttu-id="68361-122">Тип</span><span class="sxs-lookup"><span data-stu-id="68361-122">Type</span></span>   | <span data-ttu-id="68361-123">Описание</span><span class="sxs-lookup"><span data-stu-id="68361-123">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="68361-124">address</span><span class="sxs-lookup"><span data-stu-id="68361-124">address</span></span> | [<span data-ttu-id="68361-125">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="68361-125">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="68361-126">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="68361-126">The street address of the location.</span></span> |
| <span data-ttu-id="68361-127">coordinates</span><span class="sxs-lookup"><span data-stu-id="68361-127">coordinates</span></span> | [<span data-ttu-id="68361-128">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="68361-128">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="68361-129">Географические координаты и высота расположения.</span><span class="sxs-lookup"><span data-stu-id="68361-129">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="68361-130">displayName</span><span class="sxs-lookup"><span data-stu-id="68361-130">displayName</span></span>  | <span data-ttu-id="68361-131">String</span><span class="sxs-lookup"><span data-stu-id="68361-131">String</span></span> | <span data-ttu-id="68361-132">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="68361-132">The name associated with the location.</span></span>                       |
| <span data-ttu-id="68361-133">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="68361-133">locationEmailAddress</span></span> | <span data-ttu-id="68361-134">String</span><span class="sxs-lookup"><span data-stu-id="68361-134">String</span></span> | <span data-ttu-id="68361-135">Необязательный электронный адрес для расположения.</span><span class="sxs-lookup"><span data-stu-id="68361-135">Optional email address of the location.</span></span> |
| <span data-ttu-id="68361-136">locationUri</span><span class="sxs-lookup"><span data-stu-id="68361-136">locationUri</span></span> | <span data-ttu-id="68361-137">String</span><span class="sxs-lookup"><span data-stu-id="68361-137">String</span></span> | <span data-ttu-id="68361-138">Необязательный URI, представляющий местоположение.</span><span class="sxs-lookup"><span data-stu-id="68361-138">Optional URI representing the location.</span></span> |
| <span data-ttu-id="68361-139">locationType</span><span class="sxs-lookup"><span data-stu-id="68361-139">locationType</span></span> | <span data-ttu-id="68361-140">locationType</span><span class="sxs-lookup"><span data-stu-id="68361-140">locationType</span></span> | <span data-ttu-id="68361-141">Тип расположения.</span><span class="sxs-lookup"><span data-stu-id="68361-141">The type of location.</span></span> <span data-ttu-id="68361-142">Возможные значения: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="68361-142">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="68361-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68361-143">Read-only.</span></span>|
| <span data-ttu-id="68361-144">uniqueId</span><span class="sxs-lookup"><span data-stu-id="68361-144">uniqueId</span></span> | <span data-ttu-id="68361-145">String</span><span class="sxs-lookup"><span data-stu-id="68361-145">String</span></span> | <span data-ttu-id="68361-146">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="68361-146">For internal use only.</span></span>|
| <span data-ttu-id="68361-147">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="68361-147">uniqueIdType</span></span> | <span data-ttu-id="68361-148">String</span><span class="sxs-lookup"><span data-stu-id="68361-148">String</span></span> | <span data-ttu-id="68361-149">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="68361-149">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="68361-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68361-150">JSON representation</span></span>

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
  "locationType": "string",
  "locationUri": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
