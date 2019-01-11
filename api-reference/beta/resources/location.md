---
title: Тип ресурса Location
description: Представляет сведения о месте проведения события.
localization_priority: Normal
ms.openlocfilehash: 650876596e2cf9336054957cfd4c95bf4dad16b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879403"
---
# <a name="location-resource-type"></a><span data-ttu-id="a925c-103">Тип ресурса Location</span><span class="sxs-lookup"><span data-stu-id="a925c-103">Location resource type</span></span>

> <span data-ttu-id="a925c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a925c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a925c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a925c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a925c-106">Представляет сведения о месте проведения [мероприятия](event.md).</span><span class="sxs-lookup"><span data-stu-id="a925c-106">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="a925c-107">Создавать события в календаре можно несколькими способами, например с помощью REST API [создания события](../api/user-post-events.md) в приложении либо вручную с помощью пользовательского интерфейса Outlook.</span><span class="sxs-lookup"><span data-stu-id="a925c-107">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="a925c-108">Создавая событие через пользовательский интерфейс, вы можете указать место проведения обычным текстом (например, "Бар «Окунь»") или выбрать его из списка помещений, предоставленного приложением Outlook, [Автозаполнением Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) или [локальным поиском Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="a925c-108">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="a925c-109">В зависимости от того, как создано событие, Outlook может по-разному задавать доступное только для чтения свойство **locationType**.</span><span class="sxs-lookup"><span data-stu-id="a925c-109">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="a925c-110">Способ создания события</span><span class="sxs-lookup"><span data-stu-id="a925c-110">How event was created</span></span>  | <span data-ttu-id="a925c-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="a925c-111">Property</span></span>   | <span data-ttu-id="a925c-112">Ожидаемое значение</span><span class="sxs-lookup"><span data-stu-id="a925c-112">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="a925c-113">REST API [создания события](../api/user-post-events.md)</span><span class="sxs-lookup"><span data-stu-id="a925c-113">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="a925c-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="a925c-114">**locationType**</span></span> | `default` |
| <span data-ttu-id="a925c-115">Пользовательский интерфейс Outlook</span><span class="sxs-lookup"><span data-stu-id="a925c-115">User interface in Outlook</span></span> | <span data-ttu-id="a925c-116">**locationType**</span><span class="sxs-lookup"><span data-stu-id="a925c-116">**locationType**</span></span> | <span data-ttu-id="a925c-117">Одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="a925c-117">One of the following:</span></span> <ul><li><span data-ttu-id="a925c-118">`default` для расположения, указанного обычным текстом;</span><span class="sxs-lookup"><span data-stu-id="a925c-118">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="a925c-119">`conferenceRoom` для помещения из списка в Outlook;</span><span class="sxs-lookup"><span data-stu-id="a925c-119">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="a925c-120">любое из значений `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness` и `postalAddress` для расположения из Автозаполнения Bing или локального поиска Bing.</span><span class="sxs-lookup"><span data-stu-id="a925c-120">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="a925c-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="a925c-121">Properties</span></span>
| <span data-ttu-id="a925c-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="a925c-122">Property</span></span>  | <span data-ttu-id="a925c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="a925c-123">Type</span></span>   | <span data-ttu-id="a925c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a925c-124">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="a925c-125">address</span><span class="sxs-lookup"><span data-stu-id="a925c-125">address</span></span> | [<span data-ttu-id="a925c-126">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="a925c-126">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="a925c-127">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="a925c-127">The street address of the location.</span></span> |
| <span data-ttu-id="a925c-128">coordinates</span><span class="sxs-lookup"><span data-stu-id="a925c-128">coordinates</span></span> | [<span data-ttu-id="a925c-129">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a925c-129">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="a925c-130">Географические координаты и высота расположения.</span><span class="sxs-lookup"><span data-stu-id="a925c-130">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="a925c-131">displayName</span><span class="sxs-lookup"><span data-stu-id="a925c-131">displayName</span></span>  | <span data-ttu-id="a925c-132">String</span><span class="sxs-lookup"><span data-stu-id="a925c-132">String</span></span> | <span data-ttu-id="a925c-133">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="a925c-133">The name associated with the location.</span></span>                       |
| <span data-ttu-id="a925c-134">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a925c-134">locationEmailAddress</span></span> | <span data-ttu-id="a925c-135">String</span><span class="sxs-lookup"><span data-stu-id="a925c-135">String</span></span> | <span data-ttu-id="a925c-136">Необязательный электронный адрес для расположения.</span><span class="sxs-lookup"><span data-stu-id="a925c-136">Optional email address of the location.</span></span> |
| <span data-ttu-id="a925c-137">locationUri</span><span class="sxs-lookup"><span data-stu-id="a925c-137">locationUri</span></span> | <span data-ttu-id="a925c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="a925c-138">String</span></span> | <span data-ttu-id="a925c-139">Необязательный URI, представляющий местоположение.</span><span class="sxs-lookup"><span data-stu-id="a925c-139">Optional URI representing the location.</span></span> |
| <span data-ttu-id="a925c-140">locationType</span><span class="sxs-lookup"><span data-stu-id="a925c-140">locationType</span></span> | <span data-ttu-id="a925c-141">Строка</span><span class="sxs-lookup"><span data-stu-id="a925c-141">String</span></span> | <span data-ttu-id="a925c-142">Тип расположения.</span><span class="sxs-lookup"><span data-stu-id="a925c-142">The type of location.</span></span> <span data-ttu-id="a925c-143">Возможные значения: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="a925c-143">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="a925c-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a925c-144">Read-only.</span></span>|
| <span data-ttu-id="a925c-145">uniqueId</span><span class="sxs-lookup"><span data-stu-id="a925c-145">uniqueId</span></span> | <span data-ttu-id="a925c-146">Строка</span><span class="sxs-lookup"><span data-stu-id="a925c-146">String</span></span> | <span data-ttu-id="a925c-147">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="a925c-147">For internal use only.</span></span>|
| <span data-ttu-id="a925c-148">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="a925c-148">uniqueIdType</span></span> | <span data-ttu-id="a925c-149">Строка</span><span class="sxs-lookup"><span data-stu-id="a925c-149">String</span></span> | <span data-ttu-id="a925c-150">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="a925c-150">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a925c-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a925c-151">JSON representation</span></span>

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
