---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Priority
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e265e6de20491e44ba7756ffd02f4dc4d09d0b31
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029542"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="41f35-103">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="41f35-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="41f35-104">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="41f35-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="41f35-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="41f35-105">Properties</span></span>
| <span data-ttu-id="41f35-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="41f35-106">Property</span></span>     | <span data-ttu-id="41f35-107">Тип</span><span class="sxs-lookup"><span data-stu-id="41f35-107">Type</span></span>   |<span data-ttu-id="41f35-108">Описание</span><span class="sxs-lookup"><span data-stu-id="41f35-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41f35-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="41f35-109">dateTime</span></span>|<span data-ttu-id="41f35-110">String</span><span class="sxs-lookup"><span data-stu-id="41f35-110">String</span></span>|<span data-ttu-id="41f35-111">Один момент времени в объединенном представлении даты и времени (`{date}T{time}`; например, `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="41f35-111">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="41f35-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="41f35-112">timeZone</span></span>|<span data-ttu-id="41f35-113">String</span><span class="sxs-lookup"><span data-stu-id="41f35-113">String</span></span>|<span data-ttu-id="41f35-114">Представляет часовой пояс, например тихоокеанское время в США.</span><span class="sxs-lookup"><span data-stu-id="41f35-114">A string representing a specific time zone for the response, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="41f35-115">Дополнительные возможные значения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="41f35-115">See below for information about the possible values.</span></span>|

<span data-ttu-id="41f35-116">Обычно свойство **timeZone** _можно_ задать для каждого из [часовых поясов, поддерживаемых в настоящее время в Windows](https://docs.microsoft.com/ru-RU/windows-hardware/manufacture/desktop/default-time-zones), а также для дополнительных [часовых поясов, поддерживаемых API календаря](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="41f35-116">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span> 

<span data-ttu-id="41f35-117">При использовании ресурса **dateTimeTimeZone** в сочетании с методом (например, при [создании](../api/user-post-events.md) или [обновлении](../api/event-update.md) события) запишите фактически поддерживаемые часовые пояса, которых может быть совсем немного.</span><span class="sxs-lookup"><span data-stu-id="41f35-117">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="41f35-118">Дополнительные часовые пояса</span><span class="sxs-lookup"><span data-stu-id="41f35-118">Additional time zones</span></span>

<span data-ttu-id="41f35-119">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="41f35-119">Etc/GMT+12</span></span>

<span data-ttu-id="41f35-120">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="41f35-120">Etc/GMT+11</span></span>

<span data-ttu-id="41f35-121">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="41f35-121">Pacific/Honolulu</span></span>

<span data-ttu-id="41f35-122">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="41f35-122">America/Anchorage</span></span>

<span data-ttu-id="41f35-123">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="41f35-123">America/Santa_Isabel</span></span>

<span data-ttu-id="41f35-124">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="41f35-124">America/Los_Angeles</span></span>

<span data-ttu-id="41f35-125">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="41f35-125">America/Phoenix</span></span>

<span data-ttu-id="41f35-126">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="41f35-126">America/Chihuahua</span></span>

<span data-ttu-id="41f35-127">America/Denver</span><span class="sxs-lookup"><span data-stu-id="41f35-127">America/Denver</span></span>

<span data-ttu-id="41f35-128">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="41f35-128">America/Guatemala</span></span>

<span data-ttu-id="41f35-129">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="41f35-129">America/Chicago</span></span>

<span data-ttu-id="41f35-130">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="41f35-130">America/Mexico_City</span></span>

<span data-ttu-id="41f35-131">America/Regina</span><span class="sxs-lookup"><span data-stu-id="41f35-131">America/Regina</span></span>

<span data-ttu-id="41f35-132">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="41f35-132">America/Bogota</span></span>

<span data-ttu-id="41f35-133">America/New_York</span><span class="sxs-lookup"><span data-stu-id="41f35-133">America/New_York</span></span>

<span data-ttu-id="41f35-134">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="41f35-134">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="41f35-135">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="41f35-135">America/Caracas</span></span>

<span data-ttu-id="41f35-136">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="41f35-136">America/Asuncion</span></span>

<span data-ttu-id="41f35-137">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="41f35-137">America/Halifax</span></span>

<span data-ttu-id="41f35-138">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="41f35-138">America/Cuiaba</span></span>

<span data-ttu-id="41f35-139">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="41f35-139">America/La_Paz</span></span>

<span data-ttu-id="41f35-140">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="41f35-140">America/Santiago</span></span>

<span data-ttu-id="41f35-141">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="41f35-141">America/St_Johns</span></span>

<span data-ttu-id="41f35-142">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="41f35-142">America/Sao_Paulo</span></span>

<span data-ttu-id="41f35-143">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="41f35-143">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="41f35-144">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="41f35-144">America/Cayenne</span></span>

<span data-ttu-id="41f35-145">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="41f35-145">America/Godthab</span></span>

<span data-ttu-id="41f35-146">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="41f35-146">America/Montevideo</span></span>

<span data-ttu-id="41f35-147">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="41f35-147">America/Bahia</span></span>

<span data-ttu-id="41f35-148">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="41f35-148">Etc/GMT+2</span></span>

<span data-ttu-id="41f35-149">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="41f35-149">Atlantic/Azores</span></span>

<span data-ttu-id="41f35-150">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="41f35-150">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="41f35-151">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="41f35-151">Africa/Casablanca</span></span>

<span data-ttu-id="41f35-152">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="41f35-152">Etc/GMT</span></span>

<span data-ttu-id="41f35-153">Europe/London</span><span class="sxs-lookup"><span data-stu-id="41f35-153">Europe/London</span></span>

<span data-ttu-id="41f35-154">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="41f35-154">Atlantic/Reykjavik</span></span>

<span data-ttu-id="41f35-155">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="41f35-155">Europe/Berlin</span></span>

<span data-ttu-id="41f35-156">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="41f35-156">Europe/Budapest</span></span>

<span data-ttu-id="41f35-157">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="41f35-157">Europe/Paris</span></span>

<span data-ttu-id="41f35-158">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="41f35-158">Europe/Warsaw</span></span>

<span data-ttu-id="41f35-159">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="41f35-159">Africa/Lagos</span></span>

<span data-ttu-id="41f35-160">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="41f35-160">Africa/Windhoek</span></span>

<span data-ttu-id="41f35-161">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="41f35-161">Europe/Bucharest</span></span>

<span data-ttu-id="41f35-162">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="41f35-162">Asia/Beirut</span></span>

<span data-ttu-id="41f35-163">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="41f35-163">Africa/Cairo</span></span>

<span data-ttu-id="41f35-164">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="41f35-164">Asia/Damascus</span></span>

<span data-ttu-id="41f35-165">Африка, Йоханнесбург</span><span class="sxs-lookup"><span data-stu-id="41f35-165">Africa/Johannesburg</span></span>

<span data-ttu-id="41f35-166">Европа, Киев</span><span class="sxs-lookup"><span data-stu-id="41f35-166">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="41f35-167">Европа, Стамбул</span><span class="sxs-lookup"><span data-stu-id="41f35-167">Europe/Istanbul</span></span>

<span data-ttu-id="41f35-168">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="41f35-168">Asia/Jerusalem</span></span>

<span data-ttu-id="41f35-169">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="41f35-169">Asia/Amman</span></span>

<span data-ttu-id="41f35-170">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="41f35-170">Asia/Baghdad</span></span>

<span data-ttu-id="41f35-171">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="41f35-171">Europe/Kaliningrad</span></span>

<span data-ttu-id="41f35-172">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="41f35-172">Asia/Riyadh</span></span>

<span data-ttu-id="41f35-173">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="41f35-173">Africa/Nairobi</span></span>

<span data-ttu-id="41f35-174">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="41f35-174">Asia/Tehran</span></span>

<span data-ttu-id="41f35-175">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="41f35-175">Asia/Dubai</span></span>

<span data-ttu-id="41f35-176">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="41f35-176">Asia/Baku</span></span>

<span data-ttu-id="41f35-177">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="41f35-177">Europe/Moscow</span></span>

<span data-ttu-id="41f35-178">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="41f35-178">Indian/Mauritius</span></span>

<span data-ttu-id="41f35-179">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="41f35-179">Asia/Tbilisi</span></span>

<span data-ttu-id="41f35-180">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="41f35-180">Asia/Yerevan</span></span>

<span data-ttu-id="41f35-181">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="41f35-181">Asia/Kabul</span></span>

<span data-ttu-id="41f35-182">Азия, Карачи</span><span class="sxs-lookup"><span data-stu-id="41f35-182">Asia/Karachi</span></span>

<span data-ttu-id="41f35-183">Азия, Ташкент</span><span class="sxs-lookup"><span data-stu-id="41f35-183">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="41f35-184">Азия, Колката</span><span class="sxs-lookup"><span data-stu-id="41f35-184">Asia/Kolkata</span></span>

<span data-ttu-id="41f35-185">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="41f35-185">Asia/Colombo</span></span>

<span data-ttu-id="41f35-186">Азия, Катманду</span><span class="sxs-lookup"><span data-stu-id="41f35-186">Asia/Kathmandu</span></span>

<span data-ttu-id="41f35-187">Азия, Астана</span><span class="sxs-lookup"><span data-stu-id="41f35-187">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="41f35-188">Азия, Дакка</span><span class="sxs-lookup"><span data-stu-id="41f35-188">Asia/Dhaka</span></span>

<span data-ttu-id="41f35-189">Азия, Екатеринбург</span><span class="sxs-lookup"><span data-stu-id="41f35-189">Asia/Yekaterinburg</span></span>

<span data-ttu-id="41f35-190">Азия, Янгон (Рангун)</span><span class="sxs-lookup"><span data-stu-id="41f35-190">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="41f35-191">Азия, Бангкок</span><span class="sxs-lookup"><span data-stu-id="41f35-191">Asia/Bangkok</span></span>

<span data-ttu-id="41f35-192">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="41f35-192">Asia/Novosibirsk</span></span>

<span data-ttu-id="41f35-193">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="41f35-193">Asia/Shanghai</span></span>

<span data-ttu-id="41f35-194">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="41f35-194">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="41f35-195">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="41f35-195">Asia/Singapore</span></span>

<span data-ttu-id="41f35-196">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="41f35-196">Australia/Perth</span></span>

<span data-ttu-id="41f35-197">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="41f35-197">Asia/Taipei</span></span>

<span data-ttu-id="41f35-198">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="41f35-198">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="41f35-199">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="41f35-199">Asia/Irkutsk</span></span>

<span data-ttu-id="41f35-200">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="41f35-200">Asia/Tokyo</span></span>

<span data-ttu-id="41f35-201">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="41f35-201">Asia/Seoul</span></span>

<span data-ttu-id="41f35-202">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="41f35-202">Australia/Adelaide</span></span>

<span data-ttu-id="41f35-203">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="41f35-203">Australia/Darwin</span></span>

<span data-ttu-id="41f35-204">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="41f35-204">Australia/Brisbane</span></span>

<span data-ttu-id="41f35-205">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="41f35-205">Australia/Sydney</span></span>

<span data-ttu-id="41f35-206">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="41f35-206">Pacific/Port_Moresby</span></span>

<span data-ttu-id="41f35-207">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="41f35-207">Australia/Hobart</span></span>

<span data-ttu-id="41f35-208">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="41f35-208">Asia/Yakutsk</span></span>

<span data-ttu-id="41f35-209">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="41f35-209">Pacific/Guadalcanal</span></span>

<span data-ttu-id="41f35-210">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="41f35-210">Asia/Vladivostok</span></span>

<span data-ttu-id="41f35-211">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="41f35-211">Pacific/Auckland</span></span>

<span data-ttu-id="41f35-212">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="41f35-212">Etc/GMT-12</span></span>

<span data-ttu-id="41f35-213">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="41f35-213">Pacific/Fiji</span></span>

<span data-ttu-id="41f35-214">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="41f35-214">Asia/Magadan</span></span>

<span data-ttu-id="41f35-215">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="41f35-215">Pacific/Tongatapu</span></span>

<span data-ttu-id="41f35-216">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="41f35-216">Pacific/Apia</span></span>

<span data-ttu-id="41f35-217">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="41f35-217">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="41f35-218">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="41f35-218">JSON representation</span></span>

<span data-ttu-id="41f35-219">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41f35-219">Here is a JSON representation of the resource</span></span>

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
