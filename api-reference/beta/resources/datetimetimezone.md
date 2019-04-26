---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Normal
ms.openlocfilehash: 4bf62081d190e3af031d305c7db7f64d606926b6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340966"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="7a515-103">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7a515-103">dateTimeTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a515-104">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="7a515-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="7a515-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a515-105">Properties</span></span>
| <span data-ttu-id="7a515-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a515-106">Property</span></span>     | <span data-ttu-id="7a515-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7a515-107">Type</span></span>   |<span data-ttu-id="7a515-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7a515-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a515-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="7a515-109">dateTime</span></span>|<span data-ttu-id="7a515-110">String</span><span class="sxs-lookup"><span data-stu-id="7a515-110">String</span></span>|<span data-ttu-id="7a515-111">Один момент времени в объединенном представлении даты и времени (`{date}T{time}`).</span><span class="sxs-lookup"><span data-stu-id="7a515-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="7a515-112">Пример: "2019 – 04 – 16T09:00:00".</span><span class="sxs-lookup"><span data-stu-id="7a515-112">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="7a515-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="7a515-113">timeZone</span></span>|<span data-ttu-id="7a515-114">String</span><span class="sxs-lookup"><span data-stu-id="7a515-114">String</span></span>|<span data-ttu-id="7a515-115">Название часового пояса, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="7a515-115">A time zone name as described below.</span></span>|

<span data-ttu-id="7a515-116">Для свойства **TimeZone** можно задать любой часовой пояс, поддерживаемый Windows, а также следующие имена часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="7a515-116">The **timeZone** property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="7a515-117">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="7a515-117">Etc/GMT+12</span></span>

<span data-ttu-id="7a515-118">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="7a515-118">Etc/GMT+11</span></span>

<span data-ttu-id="7a515-119">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="7a515-119">Pacific/Honolulu</span></span>

<span data-ttu-id="7a515-120">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="7a515-120">America/Anchorage</span></span>

<span data-ttu-id="7a515-121">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="7a515-121">America/Santa_Isabel</span></span>

<span data-ttu-id="7a515-122">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="7a515-122">America/Los_Angeles</span></span>

<span data-ttu-id="7a515-123">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="7a515-123">America/Phoenix</span></span>

<span data-ttu-id="7a515-124">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="7a515-124">America/Chihuahua</span></span>

<span data-ttu-id="7a515-125">America/Denver</span><span class="sxs-lookup"><span data-stu-id="7a515-125">America/Denver</span></span>

<span data-ttu-id="7a515-126">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="7a515-126">America/Guatemala</span></span>

<span data-ttu-id="7a515-127">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="7a515-127">America/Chicago</span></span>

<span data-ttu-id="7a515-128">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="7a515-128">America/Mexico_City</span></span>

<span data-ttu-id="7a515-129">America/Regina</span><span class="sxs-lookup"><span data-stu-id="7a515-129">America/Regina</span></span>

<span data-ttu-id="7a515-130">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="7a515-130">America/Bogota</span></span>

<span data-ttu-id="7a515-131">America/New_York</span><span class="sxs-lookup"><span data-stu-id="7a515-131">America/New_York</span></span>

<span data-ttu-id="7a515-132">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="7a515-132">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="7a515-133">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="7a515-133">America/Caracas</span></span>

<span data-ttu-id="7a515-134">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="7a515-134">America/Asuncion</span></span>

<span data-ttu-id="7a515-135">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="7a515-135">America/Halifax</span></span>

<span data-ttu-id="7a515-136">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="7a515-136">America/Cuiaba</span></span>

<span data-ttu-id="7a515-137">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="7a515-137">America/La_Paz</span></span>

<span data-ttu-id="7a515-138">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="7a515-138">America/Santiago</span></span>

<span data-ttu-id="7a515-139">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="7a515-139">America/St_Johns</span></span>

<span data-ttu-id="7a515-140">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="7a515-140">America/Sao_Paulo</span></span>

<span data-ttu-id="7a515-141">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="7a515-141">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="7a515-142">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="7a515-142">America/Cayenne</span></span>

<span data-ttu-id="7a515-143">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="7a515-143">America/Godthab</span></span>

<span data-ttu-id="7a515-144">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="7a515-144">America/Montevideo</span></span>

<span data-ttu-id="7a515-145">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="7a515-145">America/Bahia</span></span>

<span data-ttu-id="7a515-146">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="7a515-146">Etc/GMT+2</span></span>

<span data-ttu-id="7a515-147">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="7a515-147">Atlantic/Azores</span></span>

<span data-ttu-id="7a515-148">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="7a515-148">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="7a515-149">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="7a515-149">Africa/Casablanca</span></span>

<span data-ttu-id="7a515-150">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="7a515-150">Etc/GMT</span></span>

<span data-ttu-id="7a515-151">Europe/London</span><span class="sxs-lookup"><span data-stu-id="7a515-151">Europe/London</span></span>

<span data-ttu-id="7a515-152">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="7a515-152">Atlantic/Reykjavik</span></span>

<span data-ttu-id="7a515-153">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="7a515-153">Europe/Berlin</span></span>

<span data-ttu-id="7a515-154">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="7a515-154">Europe/Budapest</span></span>

<span data-ttu-id="7a515-155">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="7a515-155">Europe/Paris</span></span>

<span data-ttu-id="7a515-156">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="7a515-156">Europe/Warsaw</span></span>

<span data-ttu-id="7a515-157">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="7a515-157">Africa/Lagos</span></span>

<span data-ttu-id="7a515-158">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="7a515-158">Africa/Windhoek</span></span>

<span data-ttu-id="7a515-159">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="7a515-159">Europe/Bucharest</span></span>

<span data-ttu-id="7a515-160">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="7a515-160">Asia/Beirut</span></span>

<span data-ttu-id="7a515-161">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="7a515-161">Africa/Cairo</span></span>

<span data-ttu-id="7a515-162">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="7a515-162">Asia/Damascus</span></span>

<span data-ttu-id="7a515-163">Африка, Йоханнесбург</span><span class="sxs-lookup"><span data-stu-id="7a515-163">Africa/Johannesburg</span></span>

<span data-ttu-id="7a515-164">Европа, Киев</span><span class="sxs-lookup"><span data-stu-id="7a515-164">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="7a515-165">Европа, Стамбул</span><span class="sxs-lookup"><span data-stu-id="7a515-165">Europe/Istanbul</span></span>

<span data-ttu-id="7a515-166">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="7a515-166">Asia/Jerusalem</span></span>

<span data-ttu-id="7a515-167">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="7a515-167">Asia/Amman</span></span>

<span data-ttu-id="7a515-168">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="7a515-168">Asia/Baghdad</span></span>

<span data-ttu-id="7a515-169">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="7a515-169">Europe/Kaliningrad</span></span>

<span data-ttu-id="7a515-170">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="7a515-170">Asia/Riyadh</span></span>

<span data-ttu-id="7a515-171">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="7a515-171">Africa/Nairobi</span></span>

<span data-ttu-id="7a515-172">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="7a515-172">Asia/Tehran</span></span>

<span data-ttu-id="7a515-173">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="7a515-173">Asia/Dubai</span></span>

<span data-ttu-id="7a515-174">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="7a515-174">Asia/Baku</span></span>

<span data-ttu-id="7a515-175">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="7a515-175">Europe/Moscow</span></span>

<span data-ttu-id="7a515-176">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="7a515-176">Indian/Mauritius</span></span>

<span data-ttu-id="7a515-177">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="7a515-177">Asia/Tbilisi</span></span>

<span data-ttu-id="7a515-178">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="7a515-178">Asia/Yerevan</span></span>

<span data-ttu-id="7a515-179">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="7a515-179">Asia/Kabul</span></span>

<span data-ttu-id="7a515-180">Азия, Карачи</span><span class="sxs-lookup"><span data-stu-id="7a515-180">Asia/Karachi</span></span>

<span data-ttu-id="7a515-181">Азия, Ташкент</span><span class="sxs-lookup"><span data-stu-id="7a515-181">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="7a515-182">Азия, Колката</span><span class="sxs-lookup"><span data-stu-id="7a515-182">Asia/Kolkata</span></span>

<span data-ttu-id="7a515-183">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="7a515-183">Asia/Colombo</span></span>

<span data-ttu-id="7a515-184">Азия, Катманду</span><span class="sxs-lookup"><span data-stu-id="7a515-184">Asia/Kathmandu</span></span>

<span data-ttu-id="7a515-185">Азия, Астана</span><span class="sxs-lookup"><span data-stu-id="7a515-185">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="7a515-186">Азия, Дакка</span><span class="sxs-lookup"><span data-stu-id="7a515-186">Asia/Dhaka</span></span>

<span data-ttu-id="7a515-187">Азия, Екатеринбург</span><span class="sxs-lookup"><span data-stu-id="7a515-187">Asia/Yekaterinburg</span></span>

<span data-ttu-id="7a515-188">Азия, Янгон (Рангун)</span><span class="sxs-lookup"><span data-stu-id="7a515-188">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="7a515-189">Азия, Бангкок</span><span class="sxs-lookup"><span data-stu-id="7a515-189">Asia/Bangkok</span></span>

<span data-ttu-id="7a515-190">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="7a515-190">Asia/Novosibirsk</span></span>

<span data-ttu-id="7a515-191">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="7a515-191">Asia/Shanghai</span></span>

<span data-ttu-id="7a515-192">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="7a515-192">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="7a515-193">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="7a515-193">Asia/Singapore</span></span>

<span data-ttu-id="7a515-194">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="7a515-194">Australia/Perth</span></span>

<span data-ttu-id="7a515-195">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="7a515-195">Asia/Taipei</span></span>

<span data-ttu-id="7a515-196">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="7a515-196">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="7a515-197">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="7a515-197">Asia/Irkutsk</span></span>

<span data-ttu-id="7a515-198">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="7a515-198">Asia/Tokyo</span></span>

<span data-ttu-id="7a515-199">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="7a515-199">Asia/Seoul</span></span>

<span data-ttu-id="7a515-200">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="7a515-200">Australia/Adelaide</span></span>

<span data-ttu-id="7a515-201">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="7a515-201">Australia/Darwin</span></span>

<span data-ttu-id="7a515-202">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="7a515-202">Australia/Brisbane</span></span>

<span data-ttu-id="7a515-203">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="7a515-203">Australia/Sydney</span></span>

<span data-ttu-id="7a515-204">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="7a515-204">Pacific/Port_Moresby</span></span>

<span data-ttu-id="7a515-205">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="7a515-205">Australia/Hobart</span></span>

<span data-ttu-id="7a515-206">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="7a515-206">Asia/Yakutsk</span></span>

<span data-ttu-id="7a515-207">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="7a515-207">Pacific/Guadalcanal</span></span>

<span data-ttu-id="7a515-208">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="7a515-208">Asia/Vladivostok</span></span>

<span data-ttu-id="7a515-209">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="7a515-209">Pacific/Auckland</span></span>

<span data-ttu-id="7a515-210">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="7a515-210">Etc/GMT-12</span></span>

<span data-ttu-id="7a515-211">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="7a515-211">Pacific/Fiji</span></span>

<span data-ttu-id="7a515-212">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="7a515-212">Asia/Magadan</span></span>

<span data-ttu-id="7a515-213">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="7a515-213">Pacific/Tongatapu</span></span>

<span data-ttu-id="7a515-214">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="7a515-214">Pacific/Apia</span></span>

<span data-ttu-id="7a515-215">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="7a515-215">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a515-216">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7a515-216">JSON representation</span></span>

<span data-ttu-id="7a515-217">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a515-217">Here is a JSON representation of the resource</span></span>

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
