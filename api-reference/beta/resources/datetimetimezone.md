---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6c1bae369b71744e69753b9e7b38e5b193db00a7
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870339"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="5dba9-103">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5dba9-103">dateTimeTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dba9-104">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="5dba9-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="5dba9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5dba9-105">Properties</span></span>
| <span data-ttu-id="5dba9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5dba9-106">Property</span></span>     | <span data-ttu-id="5dba9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5dba9-107">Type</span></span>   |<span data-ttu-id="5dba9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5dba9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dba9-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="5dba9-109">dateTime</span></span>|<span data-ttu-id="5dba9-110">String</span><span class="sxs-lookup"><span data-stu-id="5dba9-110">String</span></span>|<span data-ttu-id="5dba9-111">Один момент времени в объединенном представлении даты и времени (`{date}T{time}`).</span><span class="sxs-lookup"><span data-stu-id="5dba9-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="5dba9-112">Пример: "2019 – 04 – 16T09:00:00".</span><span class="sxs-lookup"><span data-stu-id="5dba9-112">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="5dba9-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="5dba9-113">timeZone</span></span>|<span data-ttu-id="5dba9-114">String</span><span class="sxs-lookup"><span data-stu-id="5dba9-114">String</span></span>|<span data-ttu-id="5dba9-115">Представляет часовой пояс, например тихоокеанское время в США.</span><span class="sxs-lookup"><span data-stu-id="5dba9-115">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="5dba9-116">Ниже приведены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="5dba9-116">See below for possible values.</span></span>|

<span data-ttu-id="5dba9-117">Обычно свойство **timeZone** _можно_ задать для каждого из [часовых поясов, поддерживаемых в настоящее время в Windows](/windows-hardware/manufacture/desktop/default-time-zones), а также для дополнительных [часовых поясов, поддерживаемых API календаря](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="5dba9-117">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="5dba9-118">При использовании ресурса **dateTimeTimeZone** в сочетании с методом (например, при [создании](../api/user-post-events.md) или [обновлении](../api/event-update.md) события) запишите фактически поддерживаемые часовые пояса, которых может быть совсем немного.</span><span class="sxs-lookup"><span data-stu-id="5dba9-118">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="5dba9-119">Дополнительные часовые пояса</span><span class="sxs-lookup"><span data-stu-id="5dba9-119">Additional time zones</span></span>

<span data-ttu-id="5dba9-120">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="5dba9-120">Etc/GMT+12</span></span>

<span data-ttu-id="5dba9-121">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="5dba9-121">Etc/GMT+11</span></span>

<span data-ttu-id="5dba9-122">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="5dba9-122">Pacific/Honolulu</span></span>

<span data-ttu-id="5dba9-123">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="5dba9-123">America/Anchorage</span></span>

<span data-ttu-id="5dba9-124">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="5dba9-124">America/Santa_Isabel</span></span>

<span data-ttu-id="5dba9-125">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="5dba9-125">America/Los_Angeles</span></span>

<span data-ttu-id="5dba9-126">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="5dba9-126">America/Phoenix</span></span>

<span data-ttu-id="5dba9-127">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="5dba9-127">America/Chihuahua</span></span>

<span data-ttu-id="5dba9-128">America/Denver</span><span class="sxs-lookup"><span data-stu-id="5dba9-128">America/Denver</span></span>

<span data-ttu-id="5dba9-129">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="5dba9-129">America/Guatemala</span></span>

<span data-ttu-id="5dba9-130">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="5dba9-130">America/Chicago</span></span>

<span data-ttu-id="5dba9-131">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="5dba9-131">America/Mexico_City</span></span>

<span data-ttu-id="5dba9-132">America/Regina</span><span class="sxs-lookup"><span data-stu-id="5dba9-132">America/Regina</span></span>

<span data-ttu-id="5dba9-133">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="5dba9-133">America/Bogota</span></span>

<span data-ttu-id="5dba9-134">America/New_York</span><span class="sxs-lookup"><span data-stu-id="5dba9-134">America/New_York</span></span>

<span data-ttu-id="5dba9-135">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="5dba9-135">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="5dba9-136">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="5dba9-136">America/Caracas</span></span>

<span data-ttu-id="5dba9-137">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="5dba9-137">America/Asuncion</span></span>

<span data-ttu-id="5dba9-138">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="5dba9-138">America/Halifax</span></span>

<span data-ttu-id="5dba9-139">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="5dba9-139">America/Cuiaba</span></span>

<span data-ttu-id="5dba9-140">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="5dba9-140">America/La_Paz</span></span>

<span data-ttu-id="5dba9-141">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="5dba9-141">America/Santiago</span></span>

<span data-ttu-id="5dba9-142">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="5dba9-142">America/St_Johns</span></span>

<span data-ttu-id="5dba9-143">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="5dba9-143">America/Sao_Paulo</span></span>

<span data-ttu-id="5dba9-144">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="5dba9-144">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="5dba9-145">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="5dba9-145">America/Cayenne</span></span>

<span data-ttu-id="5dba9-146">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="5dba9-146">America/Godthab</span></span>

<span data-ttu-id="5dba9-147">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="5dba9-147">America/Montevideo</span></span>

<span data-ttu-id="5dba9-148">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="5dba9-148">America/Bahia</span></span>

<span data-ttu-id="5dba9-149">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="5dba9-149">Etc/GMT+2</span></span>

<span data-ttu-id="5dba9-150">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="5dba9-150">Atlantic/Azores</span></span>

<span data-ttu-id="5dba9-151">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="5dba9-151">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="5dba9-152">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="5dba9-152">Africa/Casablanca</span></span>

<span data-ttu-id="5dba9-153">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="5dba9-153">Etc/GMT</span></span>

<span data-ttu-id="5dba9-154">Europe/London</span><span class="sxs-lookup"><span data-stu-id="5dba9-154">Europe/London</span></span>

<span data-ttu-id="5dba9-155">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="5dba9-155">Atlantic/Reykjavik</span></span>

<span data-ttu-id="5dba9-156">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="5dba9-156">Europe/Berlin</span></span>

<span data-ttu-id="5dba9-157">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="5dba9-157">Europe/Budapest</span></span>

<span data-ttu-id="5dba9-158">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="5dba9-158">Europe/Paris</span></span>

<span data-ttu-id="5dba9-159">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="5dba9-159">Europe/Warsaw</span></span>

<span data-ttu-id="5dba9-160">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="5dba9-160">Africa/Lagos</span></span>

<span data-ttu-id="5dba9-161">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="5dba9-161">Africa/Windhoek</span></span>

<span data-ttu-id="5dba9-162">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="5dba9-162">Europe/Bucharest</span></span>

<span data-ttu-id="5dba9-163">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="5dba9-163">Asia/Beirut</span></span>

<span data-ttu-id="5dba9-164">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="5dba9-164">Africa/Cairo</span></span>

<span data-ttu-id="5dba9-165">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="5dba9-165">Asia/Damascus</span></span>

<span data-ttu-id="5dba9-166">Африка, Йоханнесбург</span><span class="sxs-lookup"><span data-stu-id="5dba9-166">Africa/Johannesburg</span></span>

<span data-ttu-id="5dba9-167">Европа, Киев</span><span class="sxs-lookup"><span data-stu-id="5dba9-167">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="5dba9-168">Европа, Стамбул</span><span class="sxs-lookup"><span data-stu-id="5dba9-168">Europe/Istanbul</span></span>

<span data-ttu-id="5dba9-169">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="5dba9-169">Asia/Jerusalem</span></span>

<span data-ttu-id="5dba9-170">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="5dba9-170">Asia/Amman</span></span>

<span data-ttu-id="5dba9-171">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="5dba9-171">Asia/Baghdad</span></span>

<span data-ttu-id="5dba9-172">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="5dba9-172">Europe/Kaliningrad</span></span>

<span data-ttu-id="5dba9-173">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="5dba9-173">Asia/Riyadh</span></span>

<span data-ttu-id="5dba9-174">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="5dba9-174">Africa/Nairobi</span></span>

<span data-ttu-id="5dba9-175">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="5dba9-175">Asia/Tehran</span></span>

<span data-ttu-id="5dba9-176">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="5dba9-176">Asia/Dubai</span></span>

<span data-ttu-id="5dba9-177">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="5dba9-177">Asia/Baku</span></span>

<span data-ttu-id="5dba9-178">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="5dba9-178">Europe/Moscow</span></span>

<span data-ttu-id="5dba9-179">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="5dba9-179">Indian/Mauritius</span></span>

<span data-ttu-id="5dba9-180">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="5dba9-180">Asia/Tbilisi</span></span>

<span data-ttu-id="5dba9-181">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="5dba9-181">Asia/Yerevan</span></span>

<span data-ttu-id="5dba9-182">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="5dba9-182">Asia/Kabul</span></span>

<span data-ttu-id="5dba9-183">Азия, Карачи</span><span class="sxs-lookup"><span data-stu-id="5dba9-183">Asia/Karachi</span></span>

<span data-ttu-id="5dba9-184">Азия, Ташкент</span><span class="sxs-lookup"><span data-stu-id="5dba9-184">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="5dba9-185">Азия, Колката</span><span class="sxs-lookup"><span data-stu-id="5dba9-185">Asia/Kolkata</span></span>

<span data-ttu-id="5dba9-186">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="5dba9-186">Asia/Colombo</span></span>

<span data-ttu-id="5dba9-187">Азия, Катманду</span><span class="sxs-lookup"><span data-stu-id="5dba9-187">Asia/Kathmandu</span></span>

<span data-ttu-id="5dba9-188">Азия, Астана</span><span class="sxs-lookup"><span data-stu-id="5dba9-188">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="5dba9-189">Азия, Дакка</span><span class="sxs-lookup"><span data-stu-id="5dba9-189">Asia/Dhaka</span></span>

<span data-ttu-id="5dba9-190">Азия, Екатеринбург</span><span class="sxs-lookup"><span data-stu-id="5dba9-190">Asia/Yekaterinburg</span></span>

<span data-ttu-id="5dba9-191">Азия, Янгон (Рангун)</span><span class="sxs-lookup"><span data-stu-id="5dba9-191">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="5dba9-192">Азия, Бангкок</span><span class="sxs-lookup"><span data-stu-id="5dba9-192">Asia/Bangkok</span></span>

<span data-ttu-id="5dba9-193">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="5dba9-193">Asia/Novosibirsk</span></span>

<span data-ttu-id="5dba9-194">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="5dba9-194">Asia/Shanghai</span></span>

<span data-ttu-id="5dba9-195">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="5dba9-195">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="5dba9-196">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="5dba9-196">Asia/Singapore</span></span>

<span data-ttu-id="5dba9-197">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="5dba9-197">Australia/Perth</span></span>

<span data-ttu-id="5dba9-198">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="5dba9-198">Asia/Taipei</span></span>

<span data-ttu-id="5dba9-199">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="5dba9-199">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="5dba9-200">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="5dba9-200">Asia/Irkutsk</span></span>

<span data-ttu-id="5dba9-201">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="5dba9-201">Asia/Tokyo</span></span>

<span data-ttu-id="5dba9-202">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="5dba9-202">Asia/Seoul</span></span>

<span data-ttu-id="5dba9-203">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="5dba9-203">Australia/Adelaide</span></span>

<span data-ttu-id="5dba9-204">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="5dba9-204">Australia/Darwin</span></span>

<span data-ttu-id="5dba9-205">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="5dba9-205">Australia/Brisbane</span></span>

<span data-ttu-id="5dba9-206">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="5dba9-206">Australia/Sydney</span></span>

<span data-ttu-id="5dba9-207">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="5dba9-207">Pacific/Port_Moresby</span></span>

<span data-ttu-id="5dba9-208">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="5dba9-208">Australia/Hobart</span></span>

<span data-ttu-id="5dba9-209">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="5dba9-209">Asia/Yakutsk</span></span>

<span data-ttu-id="5dba9-210">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="5dba9-210">Pacific/Guadalcanal</span></span>

<span data-ttu-id="5dba9-211">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="5dba9-211">Asia/Vladivostok</span></span>

<span data-ttu-id="5dba9-212">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="5dba9-212">Pacific/Auckland</span></span>

<span data-ttu-id="5dba9-213">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="5dba9-213">Etc/GMT-12</span></span>

<span data-ttu-id="5dba9-214">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="5dba9-214">Pacific/Fiji</span></span>

<span data-ttu-id="5dba9-215">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="5dba9-215">Asia/Magadan</span></span>

<span data-ttu-id="5dba9-216">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="5dba9-216">Pacific/Tongatapu</span></span>

<span data-ttu-id="5dba9-217">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="5dba9-217">Pacific/Apia</span></span>

<span data-ttu-id="5dba9-218">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="5dba9-218">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="5dba9-219">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5dba9-219">JSON representation</span></span>

<span data-ttu-id="5dba9-220">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5dba9-220">Here is a JSON representation of the resource</span></span>

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
