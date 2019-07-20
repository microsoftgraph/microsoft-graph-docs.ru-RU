---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e3554386c599b4d36f4041f6e42dc091f9763817
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805261"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="11edf-103">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="11edf-103">dateTimeTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11edf-104">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="11edf-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="11edf-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="11edf-105">Properties</span></span>
| <span data-ttu-id="11edf-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="11edf-106">Property</span></span>     | <span data-ttu-id="11edf-107">Тип</span><span class="sxs-lookup"><span data-stu-id="11edf-107">Type</span></span>   |<span data-ttu-id="11edf-108">Описание</span><span class="sxs-lookup"><span data-stu-id="11edf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11edf-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="11edf-109">dateTime</span></span>|<span data-ttu-id="11edf-110">String</span><span class="sxs-lookup"><span data-stu-id="11edf-110">String</span></span>|<span data-ttu-id="11edf-111">Один момент времени в объединенном представлении даты и времени (`{date}T{time}`).</span><span class="sxs-lookup"><span data-stu-id="11edf-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="11edf-112">Пример: "2019 – 04 – 16T09:00:00".</span><span class="sxs-lookup"><span data-stu-id="11edf-112">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="11edf-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="11edf-113">timeZone</span></span>|<span data-ttu-id="11edf-114">String</span><span class="sxs-lookup"><span data-stu-id="11edf-114">String</span></span>|<span data-ttu-id="11edf-115">Представляет часовой пояс, например "Тихоокеанское время (зима)".</span><span class="sxs-lookup"><span data-stu-id="11edf-115">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="11edf-116">Ниже приведены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="11edf-116">See below for possible values.</span></span>|

<span data-ttu-id="11edf-117">В общем случае для \*\*\*\* свойства TimeZone _можно_ задать любой часовой пояс, который [в настоящее время поддерживается в Windows](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/default-time-zones), а также дополнительные часовые [пояса, поддерживаемые API календаря](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="11edf-117">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span> 

<span data-ttu-id="11edf-118">При использовании **dateTimeTimeZone** вместе с методом (например, при [создании](../api/user-post-events.md) или [обновлении](../api/event-update.md) события) Обратите внимание на поддерживаемые Часовые пояса, которые могут быть меньше подмножества.</span><span class="sxs-lookup"><span data-stu-id="11edf-118">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="11edf-119">Дополнительные Часовые пояса</span><span class="sxs-lookup"><span data-stu-id="11edf-119">Additional time zones</span></span>

<span data-ttu-id="11edf-120">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="11edf-120">Etc/GMT+12</span></span>

<span data-ttu-id="11edf-121">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="11edf-121">Etc/GMT+11</span></span>

<span data-ttu-id="11edf-122">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="11edf-122">Pacific/Honolulu</span></span>

<span data-ttu-id="11edf-123">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="11edf-123">America/Anchorage</span></span>

<span data-ttu-id="11edf-124">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="11edf-124">America/Santa_Isabel</span></span>

<span data-ttu-id="11edf-125">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="11edf-125">America/Los_Angeles</span></span>

<span data-ttu-id="11edf-126">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="11edf-126">America/Phoenix</span></span>

<span data-ttu-id="11edf-127">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="11edf-127">America/Chihuahua</span></span>

<span data-ttu-id="11edf-128">America/Denver</span><span class="sxs-lookup"><span data-stu-id="11edf-128">America/Denver</span></span>

<span data-ttu-id="11edf-129">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="11edf-129">America/Guatemala</span></span>

<span data-ttu-id="11edf-130">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="11edf-130">America/Chicago</span></span>

<span data-ttu-id="11edf-131">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="11edf-131">America/Mexico_City</span></span>

<span data-ttu-id="11edf-132">America/Regina</span><span class="sxs-lookup"><span data-stu-id="11edf-132">America/Regina</span></span>

<span data-ttu-id="11edf-133">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="11edf-133">America/Bogota</span></span>

<span data-ttu-id="11edf-134">America/New_York</span><span class="sxs-lookup"><span data-stu-id="11edf-134">America/New_York</span></span>

<span data-ttu-id="11edf-135">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="11edf-135">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="11edf-136">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="11edf-136">America/Caracas</span></span>

<span data-ttu-id="11edf-137">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="11edf-137">America/Asuncion</span></span>

<span data-ttu-id="11edf-138">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="11edf-138">America/Halifax</span></span>

<span data-ttu-id="11edf-139">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="11edf-139">America/Cuiaba</span></span>

<span data-ttu-id="11edf-140">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="11edf-140">America/La_Paz</span></span>

<span data-ttu-id="11edf-141">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="11edf-141">America/Santiago</span></span>

<span data-ttu-id="11edf-142">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="11edf-142">America/St_Johns</span></span>

<span data-ttu-id="11edf-143">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="11edf-143">America/Sao_Paulo</span></span>

<span data-ttu-id="11edf-144">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="11edf-144">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="11edf-145">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="11edf-145">America/Cayenne</span></span>

<span data-ttu-id="11edf-146">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="11edf-146">America/Godthab</span></span>

<span data-ttu-id="11edf-147">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="11edf-147">America/Montevideo</span></span>

<span data-ttu-id="11edf-148">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="11edf-148">America/Bahia</span></span>

<span data-ttu-id="11edf-149">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="11edf-149">Etc/GMT+2</span></span>

<span data-ttu-id="11edf-150">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="11edf-150">Atlantic/Azores</span></span>

<span data-ttu-id="11edf-151">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="11edf-151">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="11edf-152">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="11edf-152">Africa/Casablanca</span></span>

<span data-ttu-id="11edf-153">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="11edf-153">Etc/GMT</span></span>

<span data-ttu-id="11edf-154">Europe/London</span><span class="sxs-lookup"><span data-stu-id="11edf-154">Europe/London</span></span>

<span data-ttu-id="11edf-155">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="11edf-155">Atlantic/Reykjavik</span></span>

<span data-ttu-id="11edf-156">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="11edf-156">Europe/Berlin</span></span>

<span data-ttu-id="11edf-157">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="11edf-157">Europe/Budapest</span></span>

<span data-ttu-id="11edf-158">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="11edf-158">Europe/Paris</span></span>

<span data-ttu-id="11edf-159">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="11edf-159">Europe/Warsaw</span></span>

<span data-ttu-id="11edf-160">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="11edf-160">Africa/Lagos</span></span>

<span data-ttu-id="11edf-161">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="11edf-161">Africa/Windhoek</span></span>

<span data-ttu-id="11edf-162">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="11edf-162">Europe/Bucharest</span></span>

<span data-ttu-id="11edf-163">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="11edf-163">Asia/Beirut</span></span>

<span data-ttu-id="11edf-164">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="11edf-164">Africa/Cairo</span></span>

<span data-ttu-id="11edf-165">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="11edf-165">Asia/Damascus</span></span>

<span data-ttu-id="11edf-166">Африка, Йоханнесбург</span><span class="sxs-lookup"><span data-stu-id="11edf-166">Africa/Johannesburg</span></span>

<span data-ttu-id="11edf-167">Европа, Киев</span><span class="sxs-lookup"><span data-stu-id="11edf-167">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="11edf-168">Европа, Стамбул</span><span class="sxs-lookup"><span data-stu-id="11edf-168">Europe/Istanbul</span></span>

<span data-ttu-id="11edf-169">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="11edf-169">Asia/Jerusalem</span></span>

<span data-ttu-id="11edf-170">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="11edf-170">Asia/Amman</span></span>

<span data-ttu-id="11edf-171">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="11edf-171">Asia/Baghdad</span></span>

<span data-ttu-id="11edf-172">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="11edf-172">Europe/Kaliningrad</span></span>

<span data-ttu-id="11edf-173">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="11edf-173">Asia/Riyadh</span></span>

<span data-ttu-id="11edf-174">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="11edf-174">Africa/Nairobi</span></span>

<span data-ttu-id="11edf-175">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="11edf-175">Asia/Tehran</span></span>

<span data-ttu-id="11edf-176">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="11edf-176">Asia/Dubai</span></span>

<span data-ttu-id="11edf-177">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="11edf-177">Asia/Baku</span></span>

<span data-ttu-id="11edf-178">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="11edf-178">Europe/Moscow</span></span>

<span data-ttu-id="11edf-179">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="11edf-179">Indian/Mauritius</span></span>

<span data-ttu-id="11edf-180">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="11edf-180">Asia/Tbilisi</span></span>

<span data-ttu-id="11edf-181">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="11edf-181">Asia/Yerevan</span></span>

<span data-ttu-id="11edf-182">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="11edf-182">Asia/Kabul</span></span>

<span data-ttu-id="11edf-183">Азия, Карачи</span><span class="sxs-lookup"><span data-stu-id="11edf-183">Asia/Karachi</span></span>

<span data-ttu-id="11edf-184">Азия, Ташкент</span><span class="sxs-lookup"><span data-stu-id="11edf-184">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="11edf-185">Азия, Колката</span><span class="sxs-lookup"><span data-stu-id="11edf-185">Asia/Kolkata</span></span>

<span data-ttu-id="11edf-186">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="11edf-186">Asia/Colombo</span></span>

<span data-ttu-id="11edf-187">Азия, Катманду</span><span class="sxs-lookup"><span data-stu-id="11edf-187">Asia/Kathmandu</span></span>

<span data-ttu-id="11edf-188">Азия, Астана</span><span class="sxs-lookup"><span data-stu-id="11edf-188">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="11edf-189">Азия, Дакка</span><span class="sxs-lookup"><span data-stu-id="11edf-189">Asia/Dhaka</span></span>

<span data-ttu-id="11edf-190">Азия, Екатеринбург</span><span class="sxs-lookup"><span data-stu-id="11edf-190">Asia/Yekaterinburg</span></span>

<span data-ttu-id="11edf-191">Азия, Янгон (Рангун)</span><span class="sxs-lookup"><span data-stu-id="11edf-191">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="11edf-192">Азия, Бангкок</span><span class="sxs-lookup"><span data-stu-id="11edf-192">Asia/Bangkok</span></span>

<span data-ttu-id="11edf-193">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="11edf-193">Asia/Novosibirsk</span></span>

<span data-ttu-id="11edf-194">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="11edf-194">Asia/Shanghai</span></span>

<span data-ttu-id="11edf-195">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="11edf-195">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="11edf-196">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="11edf-196">Asia/Singapore</span></span>

<span data-ttu-id="11edf-197">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="11edf-197">Australia/Perth</span></span>

<span data-ttu-id="11edf-198">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="11edf-198">Asia/Taipei</span></span>

<span data-ttu-id="11edf-199">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="11edf-199">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="11edf-200">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="11edf-200">Asia/Irkutsk</span></span>

<span data-ttu-id="11edf-201">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="11edf-201">Asia/Tokyo</span></span>

<span data-ttu-id="11edf-202">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="11edf-202">Asia/Seoul</span></span>

<span data-ttu-id="11edf-203">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="11edf-203">Australia/Adelaide</span></span>

<span data-ttu-id="11edf-204">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="11edf-204">Australia/Darwin</span></span>

<span data-ttu-id="11edf-205">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="11edf-205">Australia/Brisbane</span></span>

<span data-ttu-id="11edf-206">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="11edf-206">Australia/Sydney</span></span>

<span data-ttu-id="11edf-207">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="11edf-207">Pacific/Port_Moresby</span></span>

<span data-ttu-id="11edf-208">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="11edf-208">Australia/Hobart</span></span>

<span data-ttu-id="11edf-209">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="11edf-209">Asia/Yakutsk</span></span>

<span data-ttu-id="11edf-210">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="11edf-210">Pacific/Guadalcanal</span></span>

<span data-ttu-id="11edf-211">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="11edf-211">Asia/Vladivostok</span></span>

<span data-ttu-id="11edf-212">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="11edf-212">Pacific/Auckland</span></span>

<span data-ttu-id="11edf-213">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="11edf-213">Etc/GMT-12</span></span>

<span data-ttu-id="11edf-214">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="11edf-214">Pacific/Fiji</span></span>

<span data-ttu-id="11edf-215">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="11edf-215">Asia/Magadan</span></span>

<span data-ttu-id="11edf-216">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="11edf-216">Pacific/Tongatapu</span></span>

<span data-ttu-id="11edf-217">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="11edf-217">Pacific/Apia</span></span>

<span data-ttu-id="11edf-218">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="11edf-218">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="11edf-219">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="11edf-219">JSON representation</span></span>

<span data-ttu-id="11edf-220">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11edf-220">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
