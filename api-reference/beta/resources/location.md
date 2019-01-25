---
title: Тип ресурса Location
description: Представляет сведения о месте проведения события.
localization_priority: Normal
ms.openlocfilehash: 6e3c61bcf8f22a20bf41053c2310dc51f5b800a7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508610"
---
# <a name="location-resource-type"></a><span data-ttu-id="c82c4-103">Тип ресурса Location</span><span class="sxs-lookup"><span data-stu-id="c82c4-103">Location resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c82c4-104">Представляет сведения о месте проведения [мероприятия](event.md).</span><span class="sxs-lookup"><span data-stu-id="c82c4-104">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="c82c4-105">Создавать события в календаре можно несколькими способами, например с помощью REST API [создания события](../api/user-post-events.md) в приложении либо вручную с помощью пользовательского интерфейса Outlook.</span><span class="sxs-lookup"><span data-stu-id="c82c4-105">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="c82c4-106">Создавая событие через пользовательский интерфейс, вы можете указать место проведения обычным текстом (например, "Бар «Окунь»") или выбрать его из списка помещений, предоставленного приложением Outlook, [Автозаполнением Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) или [локальным поиском Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="c82c4-106">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="c82c4-107">В зависимости от того, как создано событие, Outlook может по-разному задавать доступное только для чтения свойство **locationType**.</span><span class="sxs-lookup"><span data-stu-id="c82c4-107">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="c82c4-108">Способ создания события</span><span class="sxs-lookup"><span data-stu-id="c82c4-108">How event was created</span></span>  | <span data-ttu-id="c82c4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c82c4-109">Property</span></span>   | <span data-ttu-id="c82c4-110">Ожидаемое значение</span><span class="sxs-lookup"><span data-stu-id="c82c4-110">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="c82c4-111">REST API [создания события](../api/user-post-events.md)</span><span class="sxs-lookup"><span data-stu-id="c82c4-111">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="c82c4-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="c82c4-112">**locationType**</span></span> | `default` |
| <span data-ttu-id="c82c4-113">Пользовательский интерфейс Outlook</span><span class="sxs-lookup"><span data-stu-id="c82c4-113">User interface in Outlook</span></span> | <span data-ttu-id="c82c4-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="c82c4-114">**locationType**</span></span> | <span data-ttu-id="c82c4-115">Одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="c82c4-115">One of the following:</span></span> <ul><li><span data-ttu-id="c82c4-116">`default` для расположения, указанного обычным текстом;</span><span class="sxs-lookup"><span data-stu-id="c82c4-116">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="c82c4-117">`conferenceRoom` для помещения из списка в Outlook;</span><span class="sxs-lookup"><span data-stu-id="c82c4-117">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="c82c4-118">любое из значений `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness` и `postalAddress` для расположения из Автозаполнения Bing или локального поиска Bing.</span><span class="sxs-lookup"><span data-stu-id="c82c4-118">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="c82c4-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="c82c4-119">Properties</span></span>
| <span data-ttu-id="c82c4-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="c82c4-120">Property</span></span>  | <span data-ttu-id="c82c4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c82c4-121">Type</span></span>   | <span data-ttu-id="c82c4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c82c4-122">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="c82c4-123">address</span><span class="sxs-lookup"><span data-stu-id="c82c4-123">address</span></span> | [<span data-ttu-id="c82c4-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c82c4-124">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="c82c4-125">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="c82c4-125">The street address of the location.</span></span> |
| <span data-ttu-id="c82c4-126">coordinates</span><span class="sxs-lookup"><span data-stu-id="c82c4-126">coordinates</span></span> | [<span data-ttu-id="c82c4-127">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="c82c4-127">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="c82c4-128">Географические координаты и высота расположения.</span><span class="sxs-lookup"><span data-stu-id="c82c4-128">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="c82c4-129">displayName</span><span class="sxs-lookup"><span data-stu-id="c82c4-129">displayName</span></span>  | <span data-ttu-id="c82c4-130">String</span><span class="sxs-lookup"><span data-stu-id="c82c4-130">String</span></span> | <span data-ttu-id="c82c4-131">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="c82c4-131">The name associated with the location.</span></span>                       |
| <span data-ttu-id="c82c4-132">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c82c4-132">locationEmailAddress</span></span> | <span data-ttu-id="c82c4-133">String</span><span class="sxs-lookup"><span data-stu-id="c82c4-133">String</span></span> | <span data-ttu-id="c82c4-134">Необязательный электронный адрес для расположения.</span><span class="sxs-lookup"><span data-stu-id="c82c4-134">Optional email address of the location.</span></span> |
| <span data-ttu-id="c82c4-135">locationUri</span><span class="sxs-lookup"><span data-stu-id="c82c4-135">locationUri</span></span> | <span data-ttu-id="c82c4-136">String</span><span class="sxs-lookup"><span data-stu-id="c82c4-136">String</span></span> | <span data-ttu-id="c82c4-137">Необязательный URI, представляющий местоположение.</span><span class="sxs-lookup"><span data-stu-id="c82c4-137">Optional URI representing the location.</span></span> |
| <span data-ttu-id="c82c4-138">locationType</span><span class="sxs-lookup"><span data-stu-id="c82c4-138">locationType</span></span> | <span data-ttu-id="c82c4-139">String</span><span class="sxs-lookup"><span data-stu-id="c82c4-139">String</span></span> | <span data-ttu-id="c82c4-140">Тип расположения.</span><span class="sxs-lookup"><span data-stu-id="c82c4-140">The type of location.</span></span> <span data-ttu-id="c82c4-141">Возможные значения: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="c82c4-141">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="c82c4-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c82c4-142">Read-only.</span></span>|
| <span data-ttu-id="c82c4-143">uniqueId</span><span class="sxs-lookup"><span data-stu-id="c82c4-143">uniqueId</span></span> | <span data-ttu-id="c82c4-144">String</span><span class="sxs-lookup"><span data-stu-id="c82c4-144">String</span></span> | <span data-ttu-id="c82c4-145">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="c82c4-145">For internal use only.</span></span>|
| <span data-ttu-id="c82c4-146">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="c82c4-146">uniqueIdType</span></span> | <span data-ttu-id="c82c4-147">String</span><span class="sxs-lookup"><span data-stu-id="c82c4-147">String</span></span> | <span data-ttu-id="c82c4-148">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="c82c4-148">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c82c4-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c82c4-149">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/location.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
