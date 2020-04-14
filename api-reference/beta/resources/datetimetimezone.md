---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Normal
doc_type: resourcePageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: 592e8cecccdf8d1514515c4b67a9517352f5a643
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463062"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="b0c9b-103">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b0c9b-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="b0c9b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0c9b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c9b-105">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="b0c9b-105">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="b0c9b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0c9b-106">Properties</span></span>
| <span data-ttu-id="b0c9b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0c9b-107">Property</span></span>     | <span data-ttu-id="b0c9b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b0c9b-108">Type</span></span>   |<span data-ttu-id="b0c9b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b0c9b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0c9b-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="b0c9b-110">dateTime</span></span>|<span data-ttu-id="b0c9b-111">String</span><span class="sxs-lookup"><span data-stu-id="b0c9b-111">String</span></span>|<span data-ttu-id="b0c9b-112">Один момент времени в объединенном представлении даты и времени (`{date}T{time}`).</span><span class="sxs-lookup"><span data-stu-id="b0c9b-112">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="b0c9b-113">Пример: "2019 – 04 – 16T09:00:00".</span><span class="sxs-lookup"><span data-stu-id="b0c9b-113">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="b0c9b-114">timeZone</span><span class="sxs-lookup"><span data-stu-id="b0c9b-114">timeZone</span></span>|<span data-ttu-id="b0c9b-115">String</span><span class="sxs-lookup"><span data-stu-id="b0c9b-115">String</span></span>|<span data-ttu-id="b0c9b-116">Представляет часовой пояс, например тихоокеанское время в США.</span><span class="sxs-lookup"><span data-stu-id="b0c9b-116">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="b0c9b-117">Ниже приведены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="b0c9b-117">See below for possible values.</span></span>|

<span data-ttu-id="b0c9b-118">Обычно свойство **timeZone** _можно_ задать для каждого из [часовых поясов, поддерживаемых в настоящее время в Windows](/windows-hardware/manufacture/desktop/default-time-zones), а также для дополнительных [часовых поясов, поддерживаемых API календаря](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="b0c9b-118">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="b0c9b-119">При использовании ресурса **dateTimeTimeZone** в сочетании с методом (например, при [создании](../api/user-post-events.md) или [обновлении](../api/event-update.md) события) запишите фактически поддерживаемые часовые пояса, которых может быть совсем немного.</span><span class="sxs-lookup"><span data-stu-id="b0c9b-119">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="b0c9b-120">Дополнительные часовые пояса</span><span class="sxs-lookup"><span data-stu-id="b0c9b-120">Additional time zones</span></span>

<span data-ttu-id="b0c9b-121">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="b0c9b-121">Etc/GMT+12</span></span>

<span data-ttu-id="b0c9b-122">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="b0c9b-122">Etc/GMT+11</span></span>

<span data-ttu-id="b0c9b-123">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="b0c9b-123">Pacific/Honolulu</span></span>

<span data-ttu-id="b0c9b-124">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="b0c9b-124">America/Anchorage</span></span>

<span data-ttu-id="b0c9b-125">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="b0c9b-125">America/Santa_Isabel</span></span>

<span data-ttu-id="b0c9b-126">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="b0c9b-126">America/Los_Angeles</span></span>

<span data-ttu-id="b0c9b-127">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="b0c9b-127">America/Phoenix</span></span>

<span data-ttu-id="b0c9b-128">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="b0c9b-128">America/Chihuahua</span></span>

<span data-ttu-id="b0c9b-129">America/Denver</span><span class="sxs-lookup"><span data-stu-id="b0c9b-129">America/Denver</span></span>

<span data-ttu-id="b0c9b-130">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="b0c9b-130">America/Guatemala</span></span>

<span data-ttu-id="b0c9b-131">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="b0c9b-131">America/Chicago</span></span>

<span data-ttu-id="b0c9b-132">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="b0c9b-132">America/Mexico_City</span></span>

<span data-ttu-id="b0c9b-133">America/Regina</span><span class="sxs-lookup"><span data-stu-id="b0c9b-133">America/Regina</span></span>

<span data-ttu-id="b0c9b-134">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="b0c9b-134">America/Bogota</span></span>

<span data-ttu-id="b0c9b-135">America/New_York</span><span class="sxs-lookup"><span data-stu-id="b0c9b-135">America/New_York</span></span>

<span data-ttu-id="b0c9b-136">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="b0c9b-136">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="b0c9b-137">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="b0c9b-137">America/Caracas</span></span>

<span data-ttu-id="b0c9b-138">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="b0c9b-138">America/Asuncion</span></span>

<span data-ttu-id="b0c9b-139">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="b0c9b-139">America/Halifax</span></span>

<span data-ttu-id="b0c9b-140">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="b0c9b-140">America/Cuiaba</span></span>

<span data-ttu-id="b0c9b-141">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="b0c9b-141">America/La_Paz</span></span>

<span data-ttu-id="b0c9b-142">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="b0c9b-142">America/Santiago</span></span>

<span data-ttu-id="b0c9b-143">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="b0c9b-143">America/St_Johns</span></span>

<span data-ttu-id="b0c9b-144">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="b0c9b-144">America/Sao_Paulo</span></span>

<span data-ttu-id="b0c9b-145">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="b0c9b-145">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="b0c9b-146">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="b0c9b-146">America/Cayenne</span></span>

<span data-ttu-id="b0c9b-147">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="b0c9b-147">America/Godthab</span></span>

<span data-ttu-id="b0c9b-148">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="b0c9b-148">America/Montevideo</span></span>

<span data-ttu-id="b0c9b-149">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="b0c9b-149">America/Bahia</span></span>

<span data-ttu-id="b0c9b-150">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="b0c9b-150">Etc/GMT+2</span></span>

<span data-ttu-id="b0c9b-151">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="b0c9b-151">Atlantic/Azores</span></span>

<span data-ttu-id="b0c9b-152">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="b0c9b-152">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="b0c9b-153">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="b0c9b-153">Africa/Casablanca</span></span>

<span data-ttu-id="b0c9b-154">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="b0c9b-154">Etc/GMT</span></span>

<span data-ttu-id="b0c9b-155">Europe/London</span><span class="sxs-lookup"><span data-stu-id="b0c9b-155">Europe/London</span></span>

<span data-ttu-id="b0c9b-156">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="b0c9b-156">Atlantic/Reykjavik</span></span>

<span data-ttu-id="b0c9b-157">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="b0c9b-157">Europe/Berlin</span></span>

<span data-ttu-id="b0c9b-158">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="b0c9b-158">Europe/Budapest</span></span>

<span data-ttu-id="b0c9b-159">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="b0c9b-159">Europe/Paris</span></span>

<span data-ttu-id="b0c9b-160">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="b0c9b-160">Europe/Warsaw</span></span>

<span data-ttu-id="b0c9b-161">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="b0c9b-161">Africa/Lagos</span></span>

<span data-ttu-id="b0c9b-162">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="b0c9b-162">Africa/Windhoek</span></span>

<span data-ttu-id="b0c9b-163">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="b0c9b-163">Europe/Bucharest</span></span>

<span data-ttu-id="b0c9b-164">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="b0c9b-164">Asia/Beirut</span></span>

<span data-ttu-id="b0c9b-165">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="b0c9b-165">Africa/Cairo</span></span>

<span data-ttu-id="b0c9b-166">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="b0c9b-166">Asia/Damascus</span></span>

<span data-ttu-id="b0c9b-167">Африка, Йоханнесбург</span><span class="sxs-lookup"><span data-stu-id="b0c9b-167">Africa/Johannesburg</span></span>

<span data-ttu-id="b0c9b-168">Европа, Киев</span><span class="sxs-lookup"><span data-stu-id="b0c9b-168">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="b0c9b-169">Европа, Стамбул</span><span class="sxs-lookup"><span data-stu-id="b0c9b-169">Europe/Istanbul</span></span>

<span data-ttu-id="b0c9b-170">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="b0c9b-170">Asia/Jerusalem</span></span>

<span data-ttu-id="b0c9b-171">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="b0c9b-171">Asia/Amman</span></span>

<span data-ttu-id="b0c9b-172">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="b0c9b-172">Asia/Baghdad</span></span>

<span data-ttu-id="b0c9b-173">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="b0c9b-173">Europe/Kaliningrad</span></span>

<span data-ttu-id="b0c9b-174">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="b0c9b-174">Asia/Riyadh</span></span>

<span data-ttu-id="b0c9b-175">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="b0c9b-175">Africa/Nairobi</span></span>

<span data-ttu-id="b0c9b-176">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="b0c9b-176">Asia/Tehran</span></span>

<span data-ttu-id="b0c9b-177">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="b0c9b-177">Asia/Dubai</span></span>

<span data-ttu-id="b0c9b-178">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="b0c9b-178">Asia/Baku</span></span>

<span data-ttu-id="b0c9b-179">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="b0c9b-179">Europe/Moscow</span></span>

<span data-ttu-id="b0c9b-180">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="b0c9b-180">Indian/Mauritius</span></span>

<span data-ttu-id="b0c9b-181">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="b0c9b-181">Asia/Tbilisi</span></span>

<span data-ttu-id="b0c9b-182">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="b0c9b-182">Asia/Yerevan</span></span>

<span data-ttu-id="b0c9b-183">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="b0c9b-183">Asia/Kabul</span></span>

<span data-ttu-id="b0c9b-184">Азия, Карачи</span><span class="sxs-lookup"><span data-stu-id="b0c9b-184">Asia/Karachi</span></span>

<span data-ttu-id="b0c9b-185">Азия, Ташкент</span><span class="sxs-lookup"><span data-stu-id="b0c9b-185">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="b0c9b-186">Азия, Колката</span><span class="sxs-lookup"><span data-stu-id="b0c9b-186">Asia/Kolkata</span></span>

<span data-ttu-id="b0c9b-187">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="b0c9b-187">Asia/Colombo</span></span>

<span data-ttu-id="b0c9b-188">Азия, Катманду</span><span class="sxs-lookup"><span data-stu-id="b0c9b-188">Asia/Kathmandu</span></span>

<span data-ttu-id="b0c9b-189">Азия, Астана</span><span class="sxs-lookup"><span data-stu-id="b0c9b-189">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="b0c9b-190">Азия, Дакка</span><span class="sxs-lookup"><span data-stu-id="b0c9b-190">Asia/Dhaka</span></span>

<span data-ttu-id="b0c9b-191">Азия, Екатеринбург</span><span class="sxs-lookup"><span data-stu-id="b0c9b-191">Asia/Yekaterinburg</span></span>

<span data-ttu-id="b0c9b-192">Азия, Янгон (Рангун)</span><span class="sxs-lookup"><span data-stu-id="b0c9b-192">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="b0c9b-193">Азия, Бангкок</span><span class="sxs-lookup"><span data-stu-id="b0c9b-193">Asia/Bangkok</span></span>

<span data-ttu-id="b0c9b-194">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="b0c9b-194">Asia/Novosibirsk</span></span>

<span data-ttu-id="b0c9b-195">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="b0c9b-195">Asia/Shanghai</span></span>

<span data-ttu-id="b0c9b-196">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="b0c9b-196">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="b0c9b-197">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="b0c9b-197">Asia/Singapore</span></span>

<span data-ttu-id="b0c9b-198">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="b0c9b-198">Australia/Perth</span></span>

<span data-ttu-id="b0c9b-199">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="b0c9b-199">Asia/Taipei</span></span>

<span data-ttu-id="b0c9b-200">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="b0c9b-200">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="b0c9b-201">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="b0c9b-201">Asia/Irkutsk</span></span>

<span data-ttu-id="b0c9b-202">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="b0c9b-202">Asia/Tokyo</span></span>

<span data-ttu-id="b0c9b-203">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="b0c9b-203">Asia/Seoul</span></span>

<span data-ttu-id="b0c9b-204">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="b0c9b-204">Australia/Adelaide</span></span>

<span data-ttu-id="b0c9b-205">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="b0c9b-205">Australia/Darwin</span></span>

<span data-ttu-id="b0c9b-206">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="b0c9b-206">Australia/Brisbane</span></span>

<span data-ttu-id="b0c9b-207">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="b0c9b-207">Australia/Sydney</span></span>

<span data-ttu-id="b0c9b-208">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="b0c9b-208">Pacific/Port_Moresby</span></span>

<span data-ttu-id="b0c9b-209">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="b0c9b-209">Australia/Hobart</span></span>

<span data-ttu-id="b0c9b-210">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="b0c9b-210">Asia/Yakutsk</span></span>

<span data-ttu-id="b0c9b-211">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="b0c9b-211">Pacific/Guadalcanal</span></span>

<span data-ttu-id="b0c9b-212">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="b0c9b-212">Asia/Vladivostok</span></span>

<span data-ttu-id="b0c9b-213">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="b0c9b-213">Pacific/Auckland</span></span>

<span data-ttu-id="b0c9b-214">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="b0c9b-214">Etc/GMT-12</span></span>

<span data-ttu-id="b0c9b-215">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="b0c9b-215">Pacific/Fiji</span></span>

<span data-ttu-id="b0c9b-216">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="b0c9b-216">Asia/Magadan</span></span>

<span data-ttu-id="b0c9b-217">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="b0c9b-217">Pacific/Tongatapu</span></span>

<span data-ttu-id="b0c9b-218">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="b0c9b-218">Pacific/Apia</span></span>

<span data-ttu-id="b0c9b-219">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="b0c9b-219">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0c9b-220">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b0c9b-220">JSON representation</span></span>

<span data-ttu-id="b0c9b-221">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0c9b-221">Here is a JSON representation of the resource</span></span>

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
