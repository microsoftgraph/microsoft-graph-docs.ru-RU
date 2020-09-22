---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Priority
doc_type: resourcePageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: 7f5b728dd487f9802c65309c36694516b4e35455
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018790"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="f6758-103">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f6758-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="f6758-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6758-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6758-105">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="f6758-105">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="f6758-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6758-106">Properties</span></span>
| <span data-ttu-id="f6758-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6758-107">Property</span></span>     | <span data-ttu-id="f6758-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f6758-108">Type</span></span>   |<span data-ttu-id="f6758-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f6758-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6758-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="f6758-110">dateTime</span></span>|<span data-ttu-id="f6758-111">String</span><span class="sxs-lookup"><span data-stu-id="f6758-111">String</span></span>|<span data-ttu-id="f6758-112">Один момент времени в объединенном представлении даты и времени (`{date}T{time}`; например, `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="f6758-112">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="f6758-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="f6758-113">timeZone</span></span>|<span data-ttu-id="f6758-114">String</span><span class="sxs-lookup"><span data-stu-id="f6758-114">String</span></span>|<span data-ttu-id="f6758-115">Представляет часовой пояс, например тихоокеанское время в США.</span><span class="sxs-lookup"><span data-stu-id="f6758-115">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="f6758-116">Дополнительные возможные значения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="f6758-116">See below for more possible values.</span></span>|

<span data-ttu-id="f6758-117">Обычно свойство **timeZone** _можно_ задать для каждого из [часовых поясов, поддерживаемых в настоящее время в Windows](/windows-hardware/manufacture/desktop/default-time-zones), а также для дополнительных [часовых поясов, поддерживаемых API календаря](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="f6758-117">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="f6758-118">При использовании ресурса **dateTimeTimeZone** в сочетании с методом (например, при [создании](../api/user-post-events.md) или [обновлении](../api/event-update.md) события) запишите фактически поддерживаемые часовые пояса, которых может быть совсем немного.</span><span class="sxs-lookup"><span data-stu-id="f6758-118">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="f6758-119">Дополнительные часовые пояса</span><span class="sxs-lookup"><span data-stu-id="f6758-119">Additional time zones</span></span>

<span data-ttu-id="f6758-120">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="f6758-120">Etc/GMT+12</span></span>

<span data-ttu-id="f6758-121">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="f6758-121">Etc/GMT+11</span></span>

<span data-ttu-id="f6758-122">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="f6758-122">Pacific/Honolulu</span></span>

<span data-ttu-id="f6758-123">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="f6758-123">America/Anchorage</span></span>

<span data-ttu-id="f6758-124">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="f6758-124">America/Santa_Isabel</span></span>

<span data-ttu-id="f6758-125">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="f6758-125">America/Los_Angeles</span></span>

<span data-ttu-id="f6758-126">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="f6758-126">America/Phoenix</span></span>

<span data-ttu-id="f6758-127">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="f6758-127">America/Chihuahua</span></span>

<span data-ttu-id="f6758-128">America/Denver</span><span class="sxs-lookup"><span data-stu-id="f6758-128">America/Denver</span></span>

<span data-ttu-id="f6758-129">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="f6758-129">America/Guatemala</span></span>

<span data-ttu-id="f6758-130">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="f6758-130">America/Chicago</span></span>

<span data-ttu-id="f6758-131">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="f6758-131">America/Mexico_City</span></span>

<span data-ttu-id="f6758-132">America/Regina</span><span class="sxs-lookup"><span data-stu-id="f6758-132">America/Regina</span></span>

<span data-ttu-id="f6758-133">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="f6758-133">America/Bogota</span></span>

<span data-ttu-id="f6758-134">America/New_York</span><span class="sxs-lookup"><span data-stu-id="f6758-134">America/New_York</span></span>

<span data-ttu-id="f6758-135">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="f6758-135">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="f6758-136">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="f6758-136">America/Caracas</span></span>

<span data-ttu-id="f6758-137">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="f6758-137">America/Asuncion</span></span>

<span data-ttu-id="f6758-138">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="f6758-138">America/Halifax</span></span>

<span data-ttu-id="f6758-139">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="f6758-139">America/Cuiaba</span></span>

<span data-ttu-id="f6758-140">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="f6758-140">America/La_Paz</span></span>

<span data-ttu-id="f6758-141">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="f6758-141">America/Santiago</span></span>

<span data-ttu-id="f6758-142">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="f6758-142">America/St_Johns</span></span>

<span data-ttu-id="f6758-143">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="f6758-143">America/Sao_Paulo</span></span>

<span data-ttu-id="f6758-144">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="f6758-144">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="f6758-145">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="f6758-145">America/Cayenne</span></span>

<span data-ttu-id="f6758-146">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="f6758-146">America/Godthab</span></span>

<span data-ttu-id="f6758-147">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="f6758-147">America/Montevideo</span></span>

<span data-ttu-id="f6758-148">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="f6758-148">America/Bahia</span></span>

<span data-ttu-id="f6758-149">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="f6758-149">Etc/GMT+2</span></span>

<span data-ttu-id="f6758-150">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="f6758-150">Atlantic/Azores</span></span>

<span data-ttu-id="f6758-151">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="f6758-151">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="f6758-152">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="f6758-152">Africa/Casablanca</span></span>

<span data-ttu-id="f6758-153">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="f6758-153">Etc/GMT</span></span>

<span data-ttu-id="f6758-154">Europe/London</span><span class="sxs-lookup"><span data-stu-id="f6758-154">Europe/London</span></span>

<span data-ttu-id="f6758-155">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="f6758-155">Atlantic/Reykjavik</span></span>

<span data-ttu-id="f6758-156">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="f6758-156">Europe/Berlin</span></span>

<span data-ttu-id="f6758-157">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="f6758-157">Europe/Budapest</span></span>

<span data-ttu-id="f6758-158">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="f6758-158">Europe/Paris</span></span>

<span data-ttu-id="f6758-159">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="f6758-159">Europe/Warsaw</span></span>

<span data-ttu-id="f6758-160">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="f6758-160">Africa/Lagos</span></span>

<span data-ttu-id="f6758-161">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="f6758-161">Africa/Windhoek</span></span>

<span data-ttu-id="f6758-162">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="f6758-162">Europe/Bucharest</span></span>

<span data-ttu-id="f6758-163">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="f6758-163">Asia/Beirut</span></span>

<span data-ttu-id="f6758-164">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="f6758-164">Africa/Cairo</span></span>

<span data-ttu-id="f6758-165">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="f6758-165">Asia/Damascus</span></span>

<span data-ttu-id="f6758-166">Африка, Йоханнесбург</span><span class="sxs-lookup"><span data-stu-id="f6758-166">Africa/Johannesburg</span></span>

<span data-ttu-id="f6758-167">Европа, Киев</span><span class="sxs-lookup"><span data-stu-id="f6758-167">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="f6758-168">Европа, Стамбул</span><span class="sxs-lookup"><span data-stu-id="f6758-168">Europe/Istanbul</span></span>

<span data-ttu-id="f6758-169">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="f6758-169">Asia/Jerusalem</span></span>

<span data-ttu-id="f6758-170">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="f6758-170">Asia/Amman</span></span>

<span data-ttu-id="f6758-171">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="f6758-171">Asia/Baghdad</span></span>

<span data-ttu-id="f6758-172">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="f6758-172">Europe/Kaliningrad</span></span>

<span data-ttu-id="f6758-173">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="f6758-173">Asia/Riyadh</span></span>

<span data-ttu-id="f6758-174">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="f6758-174">Africa/Nairobi</span></span>

<span data-ttu-id="f6758-175">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="f6758-175">Asia/Tehran</span></span>

<span data-ttu-id="f6758-176">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="f6758-176">Asia/Dubai</span></span>

<span data-ttu-id="f6758-177">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="f6758-177">Asia/Baku</span></span>

<span data-ttu-id="f6758-178">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="f6758-178">Europe/Moscow</span></span>

<span data-ttu-id="f6758-179">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="f6758-179">Indian/Mauritius</span></span>

<span data-ttu-id="f6758-180">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="f6758-180">Asia/Tbilisi</span></span>

<span data-ttu-id="f6758-181">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="f6758-181">Asia/Yerevan</span></span>

<span data-ttu-id="f6758-182">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="f6758-182">Asia/Kabul</span></span>

<span data-ttu-id="f6758-183">Азия, Карачи</span><span class="sxs-lookup"><span data-stu-id="f6758-183">Asia/Karachi</span></span>

<span data-ttu-id="f6758-184">Азия, Ташкент</span><span class="sxs-lookup"><span data-stu-id="f6758-184">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="f6758-185">Азия, Колката</span><span class="sxs-lookup"><span data-stu-id="f6758-185">Asia/Kolkata</span></span>

<span data-ttu-id="f6758-186">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="f6758-186">Asia/Colombo</span></span>

<span data-ttu-id="f6758-187">Азия, Катманду</span><span class="sxs-lookup"><span data-stu-id="f6758-187">Asia/Kathmandu</span></span>

<span data-ttu-id="f6758-188">Азия, Астана</span><span class="sxs-lookup"><span data-stu-id="f6758-188">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="f6758-189">Азия, Дакка</span><span class="sxs-lookup"><span data-stu-id="f6758-189">Asia/Dhaka</span></span>

<span data-ttu-id="f6758-190">Азия, Екатеринбург</span><span class="sxs-lookup"><span data-stu-id="f6758-190">Asia/Yekaterinburg</span></span>

<span data-ttu-id="f6758-191">Азия, Янгон (Рангун)</span><span class="sxs-lookup"><span data-stu-id="f6758-191">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="f6758-192">Азия, Бангкок</span><span class="sxs-lookup"><span data-stu-id="f6758-192">Asia/Bangkok</span></span>

<span data-ttu-id="f6758-193">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="f6758-193">Asia/Novosibirsk</span></span>

<span data-ttu-id="f6758-194">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="f6758-194">Asia/Shanghai</span></span>

<span data-ttu-id="f6758-195">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="f6758-195">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="f6758-196">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="f6758-196">Asia/Singapore</span></span>

<span data-ttu-id="f6758-197">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="f6758-197">Australia/Perth</span></span>

<span data-ttu-id="f6758-198">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="f6758-198">Asia/Taipei</span></span>

<span data-ttu-id="f6758-199">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="f6758-199">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="f6758-200">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="f6758-200">Asia/Irkutsk</span></span>

<span data-ttu-id="f6758-201">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="f6758-201">Asia/Tokyo</span></span>

<span data-ttu-id="f6758-202">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="f6758-202">Asia/Seoul</span></span>

<span data-ttu-id="f6758-203">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="f6758-203">Australia/Adelaide</span></span>

<span data-ttu-id="f6758-204">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="f6758-204">Australia/Darwin</span></span>

<span data-ttu-id="f6758-205">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="f6758-205">Australia/Brisbane</span></span>

<span data-ttu-id="f6758-206">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="f6758-206">Australia/Sydney</span></span>

<span data-ttu-id="f6758-207">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="f6758-207">Pacific/Port_Moresby</span></span>

<span data-ttu-id="f6758-208">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="f6758-208">Australia/Hobart</span></span>

<span data-ttu-id="f6758-209">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="f6758-209">Asia/Yakutsk</span></span>

<span data-ttu-id="f6758-210">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="f6758-210">Pacific/Guadalcanal</span></span>

<span data-ttu-id="f6758-211">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="f6758-211">Asia/Vladivostok</span></span>

<span data-ttu-id="f6758-212">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="f6758-212">Pacific/Auckland</span></span>

<span data-ttu-id="f6758-213">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="f6758-213">Etc/GMT-12</span></span>

<span data-ttu-id="f6758-214">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="f6758-214">Pacific/Fiji</span></span>

<span data-ttu-id="f6758-215">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="f6758-215">Asia/Magadan</span></span>

<span data-ttu-id="f6758-216">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="f6758-216">Pacific/Tongatapu</span></span>

<span data-ttu-id="f6758-217">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="f6758-217">Pacific/Apia</span></span>

<span data-ttu-id="f6758-218">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="f6758-218">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6758-219">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f6758-219">JSON representation</span></span>

<span data-ttu-id="f6758-220">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6758-220">Here is a JSON representation of the resource</span></span>

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

