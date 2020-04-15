---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Priority
doc_type: resourcePageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: 3af4a12dad40cd6f18790ddedf99ef7e3a1770f6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449427"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="605d9-103">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="605d9-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="605d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="605d9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="605d9-105">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="605d9-105">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="605d9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="605d9-106">Properties</span></span>
| <span data-ttu-id="605d9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="605d9-107">Property</span></span>     | <span data-ttu-id="605d9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="605d9-108">Type</span></span>   |<span data-ttu-id="605d9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="605d9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="605d9-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="605d9-110">dateTime</span></span>|<span data-ttu-id="605d9-111">String</span><span class="sxs-lookup"><span data-stu-id="605d9-111">String</span></span>|<span data-ttu-id="605d9-112">Один момент времени в объединенном представлении даты и времени (`{date}T{time}`; например, `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="605d9-112">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="605d9-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="605d9-113">timeZone</span></span>|<span data-ttu-id="605d9-114">String</span><span class="sxs-lookup"><span data-stu-id="605d9-114">String</span></span>|<span data-ttu-id="605d9-115">Представляет часовой пояс, например тихоокеанское время в США.</span><span class="sxs-lookup"><span data-stu-id="605d9-115">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="605d9-116">Дополнительные возможные значения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="605d9-116">See below for more possible values.</span></span>|

<span data-ttu-id="605d9-117">Обычно свойство **timeZone** _можно_ задать для каждого из [часовых поясов, поддерживаемых в настоящее время в Windows](/windows-hardware/manufacture/desktop/default-time-zones), а также для дополнительных [часовых поясов, поддерживаемых API календаря](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="605d9-117">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="605d9-118">При использовании ресурса **dateTimeTimeZone** в сочетании с методом (например, при [создании](../api/user-post-events.md) или [обновлении](../api/event-update.md) события) запишите фактически поддерживаемые часовые пояса, которых может быть совсем немного.</span><span class="sxs-lookup"><span data-stu-id="605d9-118">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="605d9-119">Дополнительные часовые пояса</span><span class="sxs-lookup"><span data-stu-id="605d9-119">Additional time zones</span></span>

<span data-ttu-id="605d9-120">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="605d9-120">Etc/GMT+12</span></span>

<span data-ttu-id="605d9-121">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="605d9-121">Etc/GMT+11</span></span>

<span data-ttu-id="605d9-122">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="605d9-122">Pacific/Honolulu</span></span>

<span data-ttu-id="605d9-123">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="605d9-123">America/Anchorage</span></span>

<span data-ttu-id="605d9-124">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="605d9-124">America/Santa_Isabel</span></span>

<span data-ttu-id="605d9-125">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="605d9-125">America/Los_Angeles</span></span>

<span data-ttu-id="605d9-126">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="605d9-126">America/Phoenix</span></span>

<span data-ttu-id="605d9-127">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="605d9-127">America/Chihuahua</span></span>

<span data-ttu-id="605d9-128">America/Denver</span><span class="sxs-lookup"><span data-stu-id="605d9-128">America/Denver</span></span>

<span data-ttu-id="605d9-129">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="605d9-129">America/Guatemala</span></span>

<span data-ttu-id="605d9-130">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="605d9-130">America/Chicago</span></span>

<span data-ttu-id="605d9-131">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="605d9-131">America/Mexico_City</span></span>

<span data-ttu-id="605d9-132">America/Regina</span><span class="sxs-lookup"><span data-stu-id="605d9-132">America/Regina</span></span>

<span data-ttu-id="605d9-133">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="605d9-133">America/Bogota</span></span>

<span data-ttu-id="605d9-134">America/New_York</span><span class="sxs-lookup"><span data-stu-id="605d9-134">America/New_York</span></span>

<span data-ttu-id="605d9-135">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="605d9-135">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="605d9-136">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="605d9-136">America/Caracas</span></span>

<span data-ttu-id="605d9-137">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="605d9-137">America/Asuncion</span></span>

<span data-ttu-id="605d9-138">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="605d9-138">America/Halifax</span></span>

<span data-ttu-id="605d9-139">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="605d9-139">America/Cuiaba</span></span>

<span data-ttu-id="605d9-140">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="605d9-140">America/La_Paz</span></span>

<span data-ttu-id="605d9-141">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="605d9-141">America/Santiago</span></span>

<span data-ttu-id="605d9-142">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="605d9-142">America/St_Johns</span></span>

<span data-ttu-id="605d9-143">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="605d9-143">America/Sao_Paulo</span></span>

<span data-ttu-id="605d9-144">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="605d9-144">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="605d9-145">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="605d9-145">America/Cayenne</span></span>

<span data-ttu-id="605d9-146">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="605d9-146">America/Godthab</span></span>

<span data-ttu-id="605d9-147">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="605d9-147">America/Montevideo</span></span>

<span data-ttu-id="605d9-148">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="605d9-148">America/Bahia</span></span>

<span data-ttu-id="605d9-149">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="605d9-149">Etc/GMT+2</span></span>

<span data-ttu-id="605d9-150">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="605d9-150">Atlantic/Azores</span></span>

<span data-ttu-id="605d9-151">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="605d9-151">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="605d9-152">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="605d9-152">Africa/Casablanca</span></span>

<span data-ttu-id="605d9-153">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="605d9-153">Etc/GMT</span></span>

<span data-ttu-id="605d9-154">Europe/London</span><span class="sxs-lookup"><span data-stu-id="605d9-154">Europe/London</span></span>

<span data-ttu-id="605d9-155">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="605d9-155">Atlantic/Reykjavik</span></span>

<span data-ttu-id="605d9-156">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="605d9-156">Europe/Berlin</span></span>

<span data-ttu-id="605d9-157">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="605d9-157">Europe/Budapest</span></span>

<span data-ttu-id="605d9-158">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="605d9-158">Europe/Paris</span></span>

<span data-ttu-id="605d9-159">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="605d9-159">Europe/Warsaw</span></span>

<span data-ttu-id="605d9-160">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="605d9-160">Africa/Lagos</span></span>

<span data-ttu-id="605d9-161">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="605d9-161">Africa/Windhoek</span></span>

<span data-ttu-id="605d9-162">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="605d9-162">Europe/Bucharest</span></span>

<span data-ttu-id="605d9-163">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="605d9-163">Asia/Beirut</span></span>

<span data-ttu-id="605d9-164">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="605d9-164">Africa/Cairo</span></span>

<span data-ttu-id="605d9-165">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="605d9-165">Asia/Damascus</span></span>

<span data-ttu-id="605d9-166">Африка, Йоханнесбург</span><span class="sxs-lookup"><span data-stu-id="605d9-166">Africa/Johannesburg</span></span>

<span data-ttu-id="605d9-167">Европа, Киев</span><span class="sxs-lookup"><span data-stu-id="605d9-167">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="605d9-168">Европа, Стамбул</span><span class="sxs-lookup"><span data-stu-id="605d9-168">Europe/Istanbul</span></span>

<span data-ttu-id="605d9-169">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="605d9-169">Asia/Jerusalem</span></span>

<span data-ttu-id="605d9-170">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="605d9-170">Asia/Amman</span></span>

<span data-ttu-id="605d9-171">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="605d9-171">Asia/Baghdad</span></span>

<span data-ttu-id="605d9-172">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="605d9-172">Europe/Kaliningrad</span></span>

<span data-ttu-id="605d9-173">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="605d9-173">Asia/Riyadh</span></span>

<span data-ttu-id="605d9-174">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="605d9-174">Africa/Nairobi</span></span>

<span data-ttu-id="605d9-175">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="605d9-175">Asia/Tehran</span></span>

<span data-ttu-id="605d9-176">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="605d9-176">Asia/Dubai</span></span>

<span data-ttu-id="605d9-177">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="605d9-177">Asia/Baku</span></span>

<span data-ttu-id="605d9-178">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="605d9-178">Europe/Moscow</span></span>

<span data-ttu-id="605d9-179">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="605d9-179">Indian/Mauritius</span></span>

<span data-ttu-id="605d9-180">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="605d9-180">Asia/Tbilisi</span></span>

<span data-ttu-id="605d9-181">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="605d9-181">Asia/Yerevan</span></span>

<span data-ttu-id="605d9-182">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="605d9-182">Asia/Kabul</span></span>

<span data-ttu-id="605d9-183">Азия, Карачи</span><span class="sxs-lookup"><span data-stu-id="605d9-183">Asia/Karachi</span></span>

<span data-ttu-id="605d9-184">Азия, Ташкент</span><span class="sxs-lookup"><span data-stu-id="605d9-184">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="605d9-185">Азия, Колката</span><span class="sxs-lookup"><span data-stu-id="605d9-185">Asia/Kolkata</span></span>

<span data-ttu-id="605d9-186">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="605d9-186">Asia/Colombo</span></span>

<span data-ttu-id="605d9-187">Азия, Катманду</span><span class="sxs-lookup"><span data-stu-id="605d9-187">Asia/Kathmandu</span></span>

<span data-ttu-id="605d9-188">Азия, Астана</span><span class="sxs-lookup"><span data-stu-id="605d9-188">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="605d9-189">Азия, Дакка</span><span class="sxs-lookup"><span data-stu-id="605d9-189">Asia/Dhaka</span></span>

<span data-ttu-id="605d9-190">Азия, Екатеринбург</span><span class="sxs-lookup"><span data-stu-id="605d9-190">Asia/Yekaterinburg</span></span>

<span data-ttu-id="605d9-191">Азия, Янгон (Рангун)</span><span class="sxs-lookup"><span data-stu-id="605d9-191">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="605d9-192">Азия, Бангкок</span><span class="sxs-lookup"><span data-stu-id="605d9-192">Asia/Bangkok</span></span>

<span data-ttu-id="605d9-193">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="605d9-193">Asia/Novosibirsk</span></span>

<span data-ttu-id="605d9-194">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="605d9-194">Asia/Shanghai</span></span>

<span data-ttu-id="605d9-195">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="605d9-195">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="605d9-196">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="605d9-196">Asia/Singapore</span></span>

<span data-ttu-id="605d9-197">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="605d9-197">Australia/Perth</span></span>

<span data-ttu-id="605d9-198">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="605d9-198">Asia/Taipei</span></span>

<span data-ttu-id="605d9-199">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="605d9-199">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="605d9-200">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="605d9-200">Asia/Irkutsk</span></span>

<span data-ttu-id="605d9-201">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="605d9-201">Asia/Tokyo</span></span>

<span data-ttu-id="605d9-202">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="605d9-202">Asia/Seoul</span></span>

<span data-ttu-id="605d9-203">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="605d9-203">Australia/Adelaide</span></span>

<span data-ttu-id="605d9-204">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="605d9-204">Australia/Darwin</span></span>

<span data-ttu-id="605d9-205">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="605d9-205">Australia/Brisbane</span></span>

<span data-ttu-id="605d9-206">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="605d9-206">Australia/Sydney</span></span>

<span data-ttu-id="605d9-207">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="605d9-207">Pacific/Port_Moresby</span></span>

<span data-ttu-id="605d9-208">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="605d9-208">Australia/Hobart</span></span>

<span data-ttu-id="605d9-209">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="605d9-209">Asia/Yakutsk</span></span>

<span data-ttu-id="605d9-210">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="605d9-210">Pacific/Guadalcanal</span></span>

<span data-ttu-id="605d9-211">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="605d9-211">Asia/Vladivostok</span></span>

<span data-ttu-id="605d9-212">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="605d9-212">Pacific/Auckland</span></span>

<span data-ttu-id="605d9-213">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="605d9-213">Etc/GMT-12</span></span>

<span data-ttu-id="605d9-214">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="605d9-214">Pacific/Fiji</span></span>

<span data-ttu-id="605d9-215">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="605d9-215">Asia/Magadan</span></span>

<span data-ttu-id="605d9-216">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="605d9-216">Pacific/Tongatapu</span></span>

<span data-ttu-id="605d9-217">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="605d9-217">Pacific/Apia</span></span>

<span data-ttu-id="605d9-218">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="605d9-218">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="605d9-219">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="605d9-219">JSON representation</span></span>

<span data-ttu-id="605d9-220">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="605d9-220">Here is a JSON representation of the resource</span></span>

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
