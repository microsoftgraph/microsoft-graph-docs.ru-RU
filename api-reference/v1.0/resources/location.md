# <a name="location-resource-type"></a><span data-ttu-id="38907-101">Тип ресурса Location</span><span class="sxs-lookup"><span data-stu-id="38907-101">Location resource type</span></span>

<span data-ttu-id="38907-102">Представляет сведения о месте проведения [мероприятия](event.md).</span><span class="sxs-lookup"><span data-stu-id="38907-102">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="38907-103">Создавать события в календаре можно несколькими способами, например с помощью REST API [создания события](../api/user_post_events.md) в приложении либо вручную с помощью пользовательского интерфейса Outlook.</span><span class="sxs-lookup"><span data-stu-id="38907-103">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user_post_events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="38907-104">Создавая событие через пользовательский интерфейс, вы можете указать место проведения обычным текстом (например, "Бар «Окунь»") или выбрать его из списка помещений, предоставленного приложением Outlook, [Автозаполнением Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) или [локальным поиском Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="38907-104">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="38907-105">В зависимости от того, как создано событие, Outlook может по-разному задавать доступное только для чтения свойство **locationType**.</span><span class="sxs-lookup"><span data-stu-id="38907-105">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="38907-106">Способ создания события</span><span class="sxs-lookup"><span data-stu-id="38907-106">How event was created</span></span>  | <span data-ttu-id="38907-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="38907-107">Property</span></span>   | <span data-ttu-id="38907-108">Ожидаемое значение</span><span class="sxs-lookup"><span data-stu-id="38907-108">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="38907-109">REST API [создания события](../api/user_post_events.md)</span><span class="sxs-lookup"><span data-stu-id="38907-109">[create event](../api/user_post_events.md) REST API</span></span> | <span data-ttu-id="38907-110">**locationType**</span><span class="sxs-lookup"><span data-stu-id="38907-110">**locationType**</span></span> | `default` |
| <span data-ttu-id="38907-111">Пользовательский интерфейс Outlook</span><span class="sxs-lookup"><span data-stu-id="38907-111">User interface in Outlook</span></span> | <span data-ttu-id="38907-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="38907-112">**locationType**</span></span> | <span data-ttu-id="38907-113">Одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="38907-113">One of the following:</span></span> <ul><li><span data-ttu-id="38907-114">`default` для расположения, указанного обычным текстом;</span><span class="sxs-lookup"><span data-stu-id="38907-114">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="38907-115">`conferenceRoom` для помещения из списка в Outlook;</span><span class="sxs-lookup"><span data-stu-id="38907-115">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="38907-116">любое из значений `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness` и `postalAddress` для расположения из Автозаполнения Bing или локального поиска Bing.</span><span class="sxs-lookup"><span data-stu-id="38907-116">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |

## <a name="properties"></a><span data-ttu-id="38907-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="38907-117">Properties</span></span>
| <span data-ttu-id="38907-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="38907-118">Property</span></span>  | <span data-ttu-id="38907-119">Тип</span><span class="sxs-lookup"><span data-stu-id="38907-119">Type</span></span>   | <span data-ttu-id="38907-120">Описание</span><span class="sxs-lookup"><span data-stu-id="38907-120">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="38907-121">address</span><span class="sxs-lookup"><span data-stu-id="38907-121">address</span></span> | [<span data-ttu-id="38907-122">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="38907-122">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="38907-123">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="38907-123">The street address of the location.</span></span> |
| <span data-ttu-id="38907-124">coordinates</span><span class="sxs-lookup"><span data-stu-id="38907-124">coordinates</span></span> | [<span data-ttu-id="38907-125">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="38907-125">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="38907-126">Географические координаты и высота расположения.</span><span class="sxs-lookup"><span data-stu-id="38907-126">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="38907-127">displayName</span><span class="sxs-lookup"><span data-stu-id="38907-127">displayName</span></span>  | <span data-ttu-id="38907-128">Строка</span><span class="sxs-lookup"><span data-stu-id="38907-128">String</span></span> | <span data-ttu-id="38907-129">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="38907-129">The name associated with the location.</span></span>                       |
| <span data-ttu-id="38907-130">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="38907-130">locationEmailAddress</span></span> | <span data-ttu-id="38907-131">Строка</span><span class="sxs-lookup"><span data-stu-id="38907-131">String</span></span> | <span data-ttu-id="38907-132">Необязательный электронный адрес для расположения.</span><span class="sxs-lookup"><span data-stu-id="38907-132">Optional email address of the location.</span></span>              |
| <span data-ttu-id="38907-133">locationUri</span><span class="sxs-lookup"><span data-stu-id="38907-133">locationUri</span></span> | <span data-ttu-id="38907-134">Строка</span><span class="sxs-lookup"><span data-stu-id="38907-134">String</span></span> | <span data-ttu-id="38907-135">Необязательный URI, представляющий местоположение.</span><span class="sxs-lookup"><span data-stu-id="38907-135">Optional URI representing the location.</span></span> |
| <span data-ttu-id="38907-136">locationType</span><span class="sxs-lookup"><span data-stu-id="38907-136">locationType</span></span> | <span data-ttu-id="38907-137">locationType</span><span class="sxs-lookup"><span data-stu-id="38907-137">locationType</span></span> | <span data-ttu-id="38907-138">Тип расположения.</span><span class="sxs-lookup"><span data-stu-id="38907-138">The type of location.</span></span> <span data-ttu-id="38907-139">Возможные значения: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="38907-139">The possible values are `default`, `conferenceRoom`, `homeAddress`, `businessAddress`, `geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`, , or .</span></span> <span data-ttu-id="38907-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38907-140">Read-only.</span></span>|
| <span data-ttu-id="38907-141">uniqueId</span><span class="sxs-lookup"><span data-stu-id="38907-141">uniqueId</span></span> | <span data-ttu-id="38907-142">Строка</span><span class="sxs-lookup"><span data-stu-id="38907-142">String</span></span> | <span data-ttu-id="38907-143">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="38907-143">For internal use only.</span></span>|
| <span data-ttu-id="38907-144">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="38907-144">uniqueIdType</span></span> | <span data-ttu-id="38907-145">locationUniqueIdType</span><span class="sxs-lookup"><span data-stu-id="38907-145">locationUniqueIdType values</span></span> | <span data-ttu-id="38907-146">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="38907-146">For internal use only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="38907-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38907-147">JSON representation</span></span>

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
