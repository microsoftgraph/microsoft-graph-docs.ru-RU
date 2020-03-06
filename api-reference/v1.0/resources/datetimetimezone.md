---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Priority
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: cd60bf4416ae02b74d9c49fdb69c93ffa19c7c66
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531713"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="326ed-103">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="326ed-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="326ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="326ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="326ed-105">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="326ed-105">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="326ed-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="326ed-106">Properties</span></span>
| <span data-ttu-id="326ed-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="326ed-107">Property</span></span>     | <span data-ttu-id="326ed-108">Тип</span><span class="sxs-lookup"><span data-stu-id="326ed-108">Type</span></span>   |<span data-ttu-id="326ed-109">Описание</span><span class="sxs-lookup"><span data-stu-id="326ed-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="326ed-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="326ed-110">dateTime</span></span>|<span data-ttu-id="326ed-111">String</span><span class="sxs-lookup"><span data-stu-id="326ed-111">String</span></span>|<span data-ttu-id="326ed-112">Один момент времени в объединенном представлении даты и времени (`{date}T{time}`; например, `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="326ed-112">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="326ed-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="326ed-113">timeZone</span></span>|<span data-ttu-id="326ed-114">String</span><span class="sxs-lookup"><span data-stu-id="326ed-114">String</span></span>|<span data-ttu-id="326ed-115">Представляет часовой пояс, например тихоокеанское время в США.</span><span class="sxs-lookup"><span data-stu-id="326ed-115">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="326ed-116">Дополнительные возможные значения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="326ed-116">See below for more possible values.</span></span>|

<span data-ttu-id="326ed-117">Обычно свойство **timeZone** _можно_ задать для каждого из [часовых поясов, поддерживаемых в настоящее время в Windows](/windows-hardware/manufacture/desktop/default-time-zones), а также для дополнительных [часовых поясов, поддерживаемых API календаря](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="326ed-117">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="326ed-118">При использовании ресурса **dateTimeTimeZone** в сочетании с методом (например, при [создании](../api/user-post-events.md) или [обновлении](../api/event-update.md) события) запишите фактически поддерживаемые часовые пояса, которых может быть совсем немного.</span><span class="sxs-lookup"><span data-stu-id="326ed-118">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="326ed-119">Дополнительные часовые пояса</span><span class="sxs-lookup"><span data-stu-id="326ed-119">Additional time zones</span></span>

<span data-ttu-id="326ed-120">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="326ed-120">Etc/GMT+12</span></span>

<span data-ttu-id="326ed-121">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="326ed-121">Etc/GMT+11</span></span>

<span data-ttu-id="326ed-122">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="326ed-122">Pacific/Honolulu</span></span>

<span data-ttu-id="326ed-123">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="326ed-123">America/Anchorage</span></span>

<span data-ttu-id="326ed-124">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="326ed-124">America/Santa_Isabel</span></span>

<span data-ttu-id="326ed-125">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="326ed-125">America/Los_Angeles</span></span>

<span data-ttu-id="326ed-126">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="326ed-126">America/Phoenix</span></span>

<span data-ttu-id="326ed-127">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="326ed-127">America/Chihuahua</span></span>

<span data-ttu-id="326ed-128">America/Denver</span><span class="sxs-lookup"><span data-stu-id="326ed-128">America/Denver</span></span>

<span data-ttu-id="326ed-129">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="326ed-129">America/Guatemala</span></span>

<span data-ttu-id="326ed-130">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="326ed-130">America/Chicago</span></span>

<span data-ttu-id="326ed-131">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="326ed-131">America/Mexico_City</span></span>

<span data-ttu-id="326ed-132">America/Regina</span><span class="sxs-lookup"><span data-stu-id="326ed-132">America/Regina</span></span>

<span data-ttu-id="326ed-133">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="326ed-133">America/Bogota</span></span>

<span data-ttu-id="326ed-134">America/New_York</span><span class="sxs-lookup"><span data-stu-id="326ed-134">America/New_York</span></span>

<span data-ttu-id="326ed-135">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="326ed-135">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="326ed-136">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="326ed-136">America/Caracas</span></span>

<span data-ttu-id="326ed-137">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="326ed-137">America/Asuncion</span></span>

<span data-ttu-id="326ed-138">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="326ed-138">America/Halifax</span></span>

<span data-ttu-id="326ed-139">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="326ed-139">America/Cuiaba</span></span>

<span data-ttu-id="326ed-140">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="326ed-140">America/La_Paz</span></span>

<span data-ttu-id="326ed-141">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="326ed-141">America/Santiago</span></span>

<span data-ttu-id="326ed-142">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="326ed-142">America/St_Johns</span></span>

<span data-ttu-id="326ed-143">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="326ed-143">America/Sao_Paulo</span></span>

<span data-ttu-id="326ed-144">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="326ed-144">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="326ed-145">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="326ed-145">America/Cayenne</span></span>

<span data-ttu-id="326ed-146">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="326ed-146">America/Godthab</span></span>

<span data-ttu-id="326ed-147">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="326ed-147">America/Montevideo</span></span>

<span data-ttu-id="326ed-148">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="326ed-148">America/Bahia</span></span>

<span data-ttu-id="326ed-149">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="326ed-149">Etc/GMT+2</span></span>

<span data-ttu-id="326ed-150">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="326ed-150">Atlantic/Azores</span></span>

<span data-ttu-id="326ed-151">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="326ed-151">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="326ed-152">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="326ed-152">Africa/Casablanca</span></span>

<span data-ttu-id="326ed-153">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="326ed-153">Etc/GMT</span></span>

<span data-ttu-id="326ed-154">Europe/London</span><span class="sxs-lookup"><span data-stu-id="326ed-154">Europe/London</span></span>

<span data-ttu-id="326ed-155">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="326ed-155">Atlantic/Reykjavik</span></span>

<span data-ttu-id="326ed-156">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="326ed-156">Europe/Berlin</span></span>

<span data-ttu-id="326ed-157">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="326ed-157">Europe/Budapest</span></span>

<span data-ttu-id="326ed-158">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="326ed-158">Europe/Paris</span></span>

<span data-ttu-id="326ed-159">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="326ed-159">Europe/Warsaw</span></span>

<span data-ttu-id="326ed-160">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="326ed-160">Africa/Lagos</span></span>

<span data-ttu-id="326ed-161">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="326ed-161">Africa/Windhoek</span></span>

<span data-ttu-id="326ed-162">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="326ed-162">Europe/Bucharest</span></span>

<span data-ttu-id="326ed-163">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="326ed-163">Asia/Beirut</span></span>

<span data-ttu-id="326ed-164">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="326ed-164">Africa/Cairo</span></span>

<span data-ttu-id="326ed-165">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="326ed-165">Asia/Damascus</span></span>

<span data-ttu-id="326ed-166">Африка, Йоханнесбург</span><span class="sxs-lookup"><span data-stu-id="326ed-166">Africa/Johannesburg</span></span>

<span data-ttu-id="326ed-167">Европа, Киев</span><span class="sxs-lookup"><span data-stu-id="326ed-167">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="326ed-168">Европа, Стамбул</span><span class="sxs-lookup"><span data-stu-id="326ed-168">Europe/Istanbul</span></span>

<span data-ttu-id="326ed-169">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="326ed-169">Asia/Jerusalem</span></span>

<span data-ttu-id="326ed-170">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="326ed-170">Asia/Amman</span></span>

<span data-ttu-id="326ed-171">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="326ed-171">Asia/Baghdad</span></span>

<span data-ttu-id="326ed-172">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="326ed-172">Europe/Kaliningrad</span></span>

<span data-ttu-id="326ed-173">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="326ed-173">Asia/Riyadh</span></span>

<span data-ttu-id="326ed-174">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="326ed-174">Africa/Nairobi</span></span>

<span data-ttu-id="326ed-175">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="326ed-175">Asia/Tehran</span></span>

<span data-ttu-id="326ed-176">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="326ed-176">Asia/Dubai</span></span>

<span data-ttu-id="326ed-177">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="326ed-177">Asia/Baku</span></span>

<span data-ttu-id="326ed-178">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="326ed-178">Europe/Moscow</span></span>

<span data-ttu-id="326ed-179">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="326ed-179">Indian/Mauritius</span></span>

<span data-ttu-id="326ed-180">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="326ed-180">Asia/Tbilisi</span></span>

<span data-ttu-id="326ed-181">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="326ed-181">Asia/Yerevan</span></span>

<span data-ttu-id="326ed-182">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="326ed-182">Asia/Kabul</span></span>

<span data-ttu-id="326ed-183">Азия, Карачи</span><span class="sxs-lookup"><span data-stu-id="326ed-183">Asia/Karachi</span></span>

<span data-ttu-id="326ed-184">Азия, Ташкент</span><span class="sxs-lookup"><span data-stu-id="326ed-184">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="326ed-185">Азия, Колката</span><span class="sxs-lookup"><span data-stu-id="326ed-185">Asia/Kolkata</span></span>

<span data-ttu-id="326ed-186">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="326ed-186">Asia/Colombo</span></span>

<span data-ttu-id="326ed-187">Азия, Катманду</span><span class="sxs-lookup"><span data-stu-id="326ed-187">Asia/Kathmandu</span></span>

<span data-ttu-id="326ed-188">Азия, Астана</span><span class="sxs-lookup"><span data-stu-id="326ed-188">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="326ed-189">Азия, Дакка</span><span class="sxs-lookup"><span data-stu-id="326ed-189">Asia/Dhaka</span></span>

<span data-ttu-id="326ed-190">Азия, Екатеринбург</span><span class="sxs-lookup"><span data-stu-id="326ed-190">Asia/Yekaterinburg</span></span>

<span data-ttu-id="326ed-191">Азия, Янгон (Рангун)</span><span class="sxs-lookup"><span data-stu-id="326ed-191">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="326ed-192">Азия, Бангкок</span><span class="sxs-lookup"><span data-stu-id="326ed-192">Asia/Bangkok</span></span>

<span data-ttu-id="326ed-193">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="326ed-193">Asia/Novosibirsk</span></span>

<span data-ttu-id="326ed-194">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="326ed-194">Asia/Shanghai</span></span>

<span data-ttu-id="326ed-195">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="326ed-195">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="326ed-196">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="326ed-196">Asia/Singapore</span></span>

<span data-ttu-id="326ed-197">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="326ed-197">Australia/Perth</span></span>

<span data-ttu-id="326ed-198">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="326ed-198">Asia/Taipei</span></span>

<span data-ttu-id="326ed-199">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="326ed-199">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="326ed-200">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="326ed-200">Asia/Irkutsk</span></span>

<span data-ttu-id="326ed-201">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="326ed-201">Asia/Tokyo</span></span>

<span data-ttu-id="326ed-202">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="326ed-202">Asia/Seoul</span></span>

<span data-ttu-id="326ed-203">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="326ed-203">Australia/Adelaide</span></span>

<span data-ttu-id="326ed-204">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="326ed-204">Australia/Darwin</span></span>

<span data-ttu-id="326ed-205">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="326ed-205">Australia/Brisbane</span></span>

<span data-ttu-id="326ed-206">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="326ed-206">Australia/Sydney</span></span>

<span data-ttu-id="326ed-207">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="326ed-207">Pacific/Port_Moresby</span></span>

<span data-ttu-id="326ed-208">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="326ed-208">Australia/Hobart</span></span>

<span data-ttu-id="326ed-209">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="326ed-209">Asia/Yakutsk</span></span>

<span data-ttu-id="326ed-210">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="326ed-210">Pacific/Guadalcanal</span></span>

<span data-ttu-id="326ed-211">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="326ed-211">Asia/Vladivostok</span></span>

<span data-ttu-id="326ed-212">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="326ed-212">Pacific/Auckland</span></span>

<span data-ttu-id="326ed-213">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="326ed-213">Etc/GMT-12</span></span>

<span data-ttu-id="326ed-214">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="326ed-214">Pacific/Fiji</span></span>

<span data-ttu-id="326ed-215">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="326ed-215">Asia/Magadan</span></span>

<span data-ttu-id="326ed-216">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="326ed-216">Pacific/Tongatapu</span></span>

<span data-ttu-id="326ed-217">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="326ed-217">Pacific/Apia</span></span>

<span data-ttu-id="326ed-218">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="326ed-218">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="326ed-219">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="326ed-219">JSON representation</span></span>

<span data-ttu-id="326ed-220">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="326ed-220">Here is a JSON representation of the resource</span></span>

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
