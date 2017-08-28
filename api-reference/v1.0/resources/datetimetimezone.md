# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="192c2-101">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="192c2-101">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="192c2-102">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="192c2-102">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="192c2-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="192c2-103">Properties</span></span>
| <span data-ttu-id="192c2-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="192c2-104">Property</span></span>     | <span data-ttu-id="192c2-105">Тип</span><span class="sxs-lookup"><span data-stu-id="192c2-105">Type</span></span>   |<span data-ttu-id="192c2-106">Описание</span><span class="sxs-lookup"><span data-stu-id="192c2-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="192c2-107">DateTime</span><span class="sxs-lookup"><span data-stu-id="192c2-107">DateTime</span></span>|<span data-ttu-id="192c2-108">String</span><span class="sxs-lookup"><span data-stu-id="192c2-108">String</span></span>|<span data-ttu-id="192c2-109">Один момент времени в объединенном представлении даты и времени (`<date>T<time>`).</span><span class="sxs-lookup"><span data-stu-id="192c2-109">A single point of time in a combined date and time representation (`<date>T<time>`).</span></span>|
|<span data-ttu-id="192c2-110">TimeZone</span><span class="sxs-lookup"><span data-stu-id="192c2-110">TimeZone</span></span>|<span data-ttu-id="192c2-111">String</span><span class="sxs-lookup"><span data-stu-id="192c2-111">String</span></span>|<span data-ttu-id="192c2-112">Один из указанных ниже часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="192c2-112">One of the following time zone names.</span></span>|

<span data-ttu-id="192c2-113">Свойство _TimeZone_ можно задать для каждого из часовых поясов, которые поддерживаются в Windows, а также для указанных ниже часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="192c2-113">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="192c2-114">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="192c2-114">Etc/GMT+12</span></span>

<span data-ttu-id="192c2-115">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="192c2-115">Etc/GMT+11</span></span>

<span data-ttu-id="192c2-116">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="192c2-116">Pacific/Honolulu</span></span>

<span data-ttu-id="192c2-117">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="192c2-117">America/Anchorage</span></span>

<span data-ttu-id="192c2-118">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="192c2-118">America/Santa_Isabel</span></span>

<span data-ttu-id="192c2-119">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="192c2-119">America/Los_Angeles</span></span>

<span data-ttu-id="192c2-120">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="192c2-120">America/Phoenix</span></span>

<span data-ttu-id="192c2-121">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="192c2-121">America/Chihuahua</span></span>

<span data-ttu-id="192c2-122">America/Denver</span><span class="sxs-lookup"><span data-stu-id="192c2-122">America/Denver</span></span>

<span data-ttu-id="192c2-123">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="192c2-123">America/Guatemala</span></span>

<span data-ttu-id="192c2-124">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="192c2-124">America/Chicago</span></span>

<span data-ttu-id="192c2-125">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="192c2-125">America/Mexico_City</span></span>

<span data-ttu-id="192c2-126">America/Regina</span><span class="sxs-lookup"><span data-stu-id="192c2-126">America/Regina</span></span>

<span data-ttu-id="192c2-127">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="192c2-127">America/Bogota</span></span>

<span data-ttu-id="192c2-128">America/New_York</span><span class="sxs-lookup"><span data-stu-id="192c2-128">America/New_York</span></span>

<span data-ttu-id="192c2-129">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="192c2-129">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="192c2-130">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="192c2-130">America/Caracas</span></span>

<span data-ttu-id="192c2-131">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="192c2-131">America/Asuncion</span></span>

<span data-ttu-id="192c2-132">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="192c2-132">America/Halifax</span></span>

<span data-ttu-id="192c2-133">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="192c2-133">America/Cuiaba</span></span>

<span data-ttu-id="192c2-134">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="192c2-134">America/La_Paz</span></span>

<span data-ttu-id="192c2-135">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="192c2-135">America/Santiago</span></span>

<span data-ttu-id="192c2-136">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="192c2-136">America/St_Johns</span></span>

<span data-ttu-id="192c2-137">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="192c2-137">America/Sao_Paulo</span></span>

<span data-ttu-id="192c2-138">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="192c2-138">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="192c2-139">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="192c2-139">America/Cayenne</span></span>

<span data-ttu-id="192c2-140">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="192c2-140">America/Godthab</span></span>

<span data-ttu-id="192c2-141">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="192c2-141">America/Montevideo</span></span>

<span data-ttu-id="192c2-142">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="192c2-142">America/Bahia</span></span>

<span data-ttu-id="192c2-143">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="192c2-143">Etc/GMT+2</span></span>

<span data-ttu-id="192c2-144">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="192c2-144">Atlantic/Azores</span></span>

<span data-ttu-id="192c2-145">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="192c2-145">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="192c2-146">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="192c2-146">Africa/Casablanca</span></span>

<span data-ttu-id="192c2-147">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="192c2-147">Etc/GMT</span></span>

<span data-ttu-id="192c2-148">Europe/London</span><span class="sxs-lookup"><span data-stu-id="192c2-148">Europe/London</span></span>

<span data-ttu-id="192c2-149">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="192c2-149">Atlantic/Reykjavik</span></span>

<span data-ttu-id="192c2-150">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="192c2-150">Europe/Berlin</span></span>

<span data-ttu-id="192c2-151">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="192c2-151">Europe/Budapest</span></span>

<span data-ttu-id="192c2-152">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="192c2-152">Europe/Paris</span></span>

<span data-ttu-id="192c2-153">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="192c2-153">Europe/Warsaw</span></span>

<span data-ttu-id="192c2-154">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="192c2-154">Africa/Lagos</span></span>

<span data-ttu-id="192c2-155">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="192c2-155">Africa/Windhoek</span></span>

<span data-ttu-id="192c2-156">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="192c2-156">Europe/Bucharest</span></span>

<span data-ttu-id="192c2-157">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="192c2-157">Asia/Beirut</span></span>

<span data-ttu-id="192c2-158">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="192c2-158">Africa/Cairo</span></span>

<span data-ttu-id="192c2-159">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="192c2-159">Asia/Damascus</span></span>

<span data-ttu-id="192c2-160">Africa/Johannesburg</span><span class="sxs-lookup"><span data-stu-id="192c2-160">Africa/Johannesburg</span></span>

<span data-ttu-id="192c2-161">Europe/Kiev</span><span class="sxs-lookup"><span data-stu-id="192c2-161">Europe/Kiev</span></span>

<span data-ttu-id="192c2-162">Europe/Istanbul</span><span class="sxs-lookup"><span data-stu-id="192c2-162">Europe/Istanbul</span></span>

<span data-ttu-id="192c2-163">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="192c2-163">Asia/Jerusalem</span></span>

<span data-ttu-id="192c2-164">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="192c2-164">Asia/Amman</span></span>

<span data-ttu-id="192c2-165">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="192c2-165">Asia/Baghdad</span></span>

<span data-ttu-id="192c2-166">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="192c2-166">Europe/Kaliningrad</span></span>

<span data-ttu-id="192c2-167">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="192c2-167">Asia/Riyadh</span></span>

<span data-ttu-id="192c2-168">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="192c2-168">Africa/Nairobi</span></span>

<span data-ttu-id="192c2-169">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="192c2-169">Asia/Tehran</span></span>

<span data-ttu-id="192c2-170">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="192c2-170">Asia/Dubai</span></span>

<span data-ttu-id="192c2-171">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="192c2-171">Asia/Baku</span></span>

<span data-ttu-id="192c2-172">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="192c2-172">Europe/Moscow</span></span>

<span data-ttu-id="192c2-173">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="192c2-173">Indian/Mauritius</span></span>

<span data-ttu-id="192c2-174">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="192c2-174">Asia/Tbilisi</span></span>

<span data-ttu-id="192c2-175">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="192c2-175">Asia/Yerevan</span></span>

<span data-ttu-id="192c2-176">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="192c2-176">Asia/Kabul</span></span>

<span data-ttu-id="192c2-177">Asia/Karachi</span><span class="sxs-lookup"><span data-stu-id="192c2-177">Asia/Karachi</span></span>

<span data-ttu-id="192c2-178">Asia/Tashkent</span><span class="sxs-lookup"><span data-stu-id="192c2-178">Asia/Tashkent</span></span>

<span data-ttu-id="192c2-179">Asia/Kolkata</span><span class="sxs-lookup"><span data-stu-id="192c2-179">Asia/Kolkata</span></span>

<span data-ttu-id="192c2-180">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="192c2-180">Asia/Colombo</span></span>

<span data-ttu-id="192c2-181">Asia/Kathmandu</span><span class="sxs-lookup"><span data-stu-id="192c2-181">Asia/Kathmandu</span></span>

<span data-ttu-id="192c2-182">Asia/Almaty</span><span class="sxs-lookup"><span data-stu-id="192c2-182">Asia/Almaty</span></span>

<span data-ttu-id="192c2-183">Asia/Dhaka</span><span class="sxs-lookup"><span data-stu-id="192c2-183">Asia/Dhaka</span></span>

<span data-ttu-id="192c2-184">Asia/Yekaterinburg</span><span class="sxs-lookup"><span data-stu-id="192c2-184">Asia/Yekaterinburg</span></span>

<span data-ttu-id="192c2-185">Asia/Rangoon</span><span class="sxs-lookup"><span data-stu-id="192c2-185">Asia/Rangoon</span></span>

<span data-ttu-id="192c2-186">Asia/Bangkok</span><span class="sxs-lookup"><span data-stu-id="192c2-186">Asia/Bangkok</span></span>

<span data-ttu-id="192c2-187">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="192c2-187">Asia/Novosibirsk</span></span>

<span data-ttu-id="192c2-188">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="192c2-188">Asia/Shanghai</span></span>

<span data-ttu-id="192c2-189">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="192c2-189">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="192c2-190">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="192c2-190">Asia/Singapore</span></span>

<span data-ttu-id="192c2-191">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="192c2-191">Australia/Perth</span></span>

<span data-ttu-id="192c2-192">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="192c2-192">Asia/Taipei</span></span>

<span data-ttu-id="192c2-193">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="192c2-193">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="192c2-194">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="192c2-194">Asia/Irkutsk</span></span>

<span data-ttu-id="192c2-195">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="192c2-195">Asia/Tokyo</span></span>

<span data-ttu-id="192c2-196">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="192c2-196">Asia/Seoul</span></span>

<span data-ttu-id="192c2-197">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="192c2-197">Australia/Adelaide</span></span>

<span data-ttu-id="192c2-198">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="192c2-198">Australia/Darwin</span></span>

<span data-ttu-id="192c2-199">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="192c2-199">Australia/Brisbane</span></span>

<span data-ttu-id="192c2-200">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="192c2-200">Australia/Sydney</span></span>

<span data-ttu-id="192c2-201">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="192c2-201">Pacific/Port_Moresby</span></span>

<span data-ttu-id="192c2-202">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="192c2-202">Australia/Hobart</span></span>

<span data-ttu-id="192c2-203">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="192c2-203">Asia/Yakutsk</span></span>

<span data-ttu-id="192c2-204">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="192c2-204">Pacific/Guadalcanal</span></span>

<span data-ttu-id="192c2-205">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="192c2-205">Asia/Vladivostok</span></span>

<span data-ttu-id="192c2-206">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="192c2-206">Pacific/Auckland</span></span>

<span data-ttu-id="192c2-207">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="192c2-207">Etc/GMT-12</span></span>

<span data-ttu-id="192c2-208">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="192c2-208">Pacific/Fiji</span></span>

<span data-ttu-id="192c2-209">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="192c2-209">Asia/Magadan</span></span>

<span data-ttu-id="192c2-210">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="192c2-210">Pacific/Tongatapu</span></span>

<span data-ttu-id="192c2-211">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="192c2-211">Pacific/Apia</span></span>

<span data-ttu-id="192c2-212">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="192c2-212">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="192c2-213">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="192c2-213">JSON representation</span></span>

<span data-ttu-id="192c2-214">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="192c2-214">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dateTimeTimeZone"
}-->

```json
{
  "dateTime": "string",
  "timeZone": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
