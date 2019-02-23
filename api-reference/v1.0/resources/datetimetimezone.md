---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Priority
ms.openlocfilehash: 9e031b053ebc185ee02fa11571019529a870cf04
ms.sourcegitcommit: 7412dd2f2d5ed66afa2b0759c861ad23b4c6ecdf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/23/2019
ms.locfileid: "30212363"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="aac22-103">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="aac22-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="aac22-104">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="aac22-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="aac22-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="aac22-105">Properties</span></span>
| <span data-ttu-id="aac22-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="aac22-106">Property</span></span>     | <span data-ttu-id="aac22-107">Тип</span><span class="sxs-lookup"><span data-stu-id="aac22-107">Type</span></span>   |<span data-ttu-id="aac22-108">Описание</span><span class="sxs-lookup"><span data-stu-id="aac22-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aac22-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="aac22-109">dateTime</span></span>|<span data-ttu-id="aac22-110">String</span><span class="sxs-lookup"><span data-stu-id="aac22-110">String</span></span>|<span data-ttu-id="aac22-111">Один момент времени в объединенном представлении даты и времени (`{date}T{time}`; например, `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="aac22-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span>|
|<span data-ttu-id="aac22-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="aac22-112">timeZone</span></span>|<span data-ttu-id="aac22-113">String</span><span class="sxs-lookup"><span data-stu-id="aac22-113">String</span></span>|<span data-ttu-id="aac22-114">Один из указанных ниже часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="aac22-114">One of the following time zone names.</span></span>|

<span data-ttu-id="aac22-115">Свойство _TimeZone_ можно задать для каждого из часовых поясов, которые поддерживаются в Windows, а также для указанных ниже часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="aac22-115">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="aac22-116">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="aac22-116">Etc/GMT+12</span></span>

<span data-ttu-id="aac22-117">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="aac22-117">Etc/GMT+11</span></span>

<span data-ttu-id="aac22-118">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="aac22-118">Pacific/Honolulu</span></span>

<span data-ttu-id="aac22-119">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="aac22-119">America/Anchorage</span></span>

<span data-ttu-id="aac22-120">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="aac22-120">America/Santa_Isabel</span></span>

<span data-ttu-id="aac22-121">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="aac22-121">America/Los_Angeles</span></span>

<span data-ttu-id="aac22-122">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="aac22-122">America/Phoenix</span></span>

<span data-ttu-id="aac22-123">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="aac22-123">America/Chihuahua</span></span>

<span data-ttu-id="aac22-124">America/Denver</span><span class="sxs-lookup"><span data-stu-id="aac22-124">America/Denver</span></span>

<span data-ttu-id="aac22-125">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="aac22-125">America/Guatemala</span></span>

<span data-ttu-id="aac22-126">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="aac22-126">America/Chicago</span></span>

<span data-ttu-id="aac22-127">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="aac22-127">America/Mexico_City</span></span>

<span data-ttu-id="aac22-128">America/Regina</span><span class="sxs-lookup"><span data-stu-id="aac22-128">America/Regina</span></span>

<span data-ttu-id="aac22-129">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="aac22-129">America/Bogota</span></span>

<span data-ttu-id="aac22-130">America/New_York</span><span class="sxs-lookup"><span data-stu-id="aac22-130">America/New_York</span></span>

<span data-ttu-id="aac22-131">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="aac22-131">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="aac22-132">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="aac22-132">America/Caracas</span></span>

<span data-ttu-id="aac22-133">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="aac22-133">America/Asuncion</span></span>

<span data-ttu-id="aac22-134">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="aac22-134">America/Halifax</span></span>

<span data-ttu-id="aac22-135">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="aac22-135">America/Cuiaba</span></span>

<span data-ttu-id="aac22-136">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="aac22-136">America/La_Paz</span></span>

<span data-ttu-id="aac22-137">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="aac22-137">America/Santiago</span></span>

<span data-ttu-id="aac22-138">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="aac22-138">America/St_Johns</span></span>

<span data-ttu-id="aac22-139">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="aac22-139">America/Sao_Paulo</span></span>

<span data-ttu-id="aac22-140">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="aac22-140">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="aac22-141">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="aac22-141">America/Cayenne</span></span>

<span data-ttu-id="aac22-142">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="aac22-142">America/Godthab</span></span>

<span data-ttu-id="aac22-143">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="aac22-143">America/Montevideo</span></span>

<span data-ttu-id="aac22-144">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="aac22-144">America/Bahia</span></span>

<span data-ttu-id="aac22-145">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="aac22-145">Etc/GMT+2</span></span>

<span data-ttu-id="aac22-146">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="aac22-146">Atlantic/Azores</span></span>

<span data-ttu-id="aac22-147">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="aac22-147">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="aac22-148">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="aac22-148">Africa/Casablanca</span></span>

<span data-ttu-id="aac22-149">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="aac22-149">Etc/GMT</span></span>

<span data-ttu-id="aac22-150">Europe/London</span><span class="sxs-lookup"><span data-stu-id="aac22-150">Europe/London</span></span>

<span data-ttu-id="aac22-151">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="aac22-151">Atlantic/Reykjavik</span></span>

<span data-ttu-id="aac22-152">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="aac22-152">Europe/Berlin</span></span>

<span data-ttu-id="aac22-153">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="aac22-153">Europe/Budapest</span></span>

<span data-ttu-id="aac22-154">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="aac22-154">Europe/Paris</span></span>

<span data-ttu-id="aac22-155">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="aac22-155">Europe/Warsaw</span></span>

<span data-ttu-id="aac22-156">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="aac22-156">Africa/Lagos</span></span>

<span data-ttu-id="aac22-157">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="aac22-157">Africa/Windhoek</span></span>

<span data-ttu-id="aac22-158">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="aac22-158">Europe/Bucharest</span></span>

<span data-ttu-id="aac22-159">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="aac22-159">Asia/Beirut</span></span>

<span data-ttu-id="aac22-160">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="aac22-160">Africa/Cairo</span></span>

<span data-ttu-id="aac22-161">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="aac22-161">Asia/Damascus</span></span>

<span data-ttu-id="aac22-162">Африка, Йоханнесбург</span><span class="sxs-lookup"><span data-stu-id="aac22-162">Africa/Johannesburg</span></span>

<span data-ttu-id="aac22-163">Европа, Киев</span><span class="sxs-lookup"><span data-stu-id="aac22-163">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="aac22-164">Европа, Стамбул</span><span class="sxs-lookup"><span data-stu-id="aac22-164">Europe/Istanbul</span></span>

<span data-ttu-id="aac22-165">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="aac22-165">Asia/Jerusalem</span></span>

<span data-ttu-id="aac22-166">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="aac22-166">Asia/Amman</span></span>

<span data-ttu-id="aac22-167">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="aac22-167">Asia/Baghdad</span></span>

<span data-ttu-id="aac22-168">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="aac22-168">Europe/Kaliningrad</span></span>

<span data-ttu-id="aac22-169">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="aac22-169">Asia/Riyadh</span></span>

<span data-ttu-id="aac22-170">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="aac22-170">Africa/Nairobi</span></span>

<span data-ttu-id="aac22-171">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="aac22-171">Asia/Tehran</span></span>

<span data-ttu-id="aac22-172">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="aac22-172">Asia/Dubai</span></span>

<span data-ttu-id="aac22-173">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="aac22-173">Asia/Baku</span></span>

<span data-ttu-id="aac22-174">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="aac22-174">Europe/Moscow</span></span>

<span data-ttu-id="aac22-175">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="aac22-175">Indian/Mauritius</span></span>

<span data-ttu-id="aac22-176">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="aac22-176">Asia/Tbilisi</span></span>

<span data-ttu-id="aac22-177">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="aac22-177">Asia/Yerevan</span></span>

<span data-ttu-id="aac22-178">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="aac22-178">Asia/Kabul</span></span>

<span data-ttu-id="aac22-179">Азия, Карачи</span><span class="sxs-lookup"><span data-stu-id="aac22-179">Asia/Karachi</span></span>

<span data-ttu-id="aac22-180">Азия, Ташкент</span><span class="sxs-lookup"><span data-stu-id="aac22-180">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="aac22-181">Азия, Колката</span><span class="sxs-lookup"><span data-stu-id="aac22-181">Asia/Kolkata</span></span>

<span data-ttu-id="aac22-182">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="aac22-182">Asia/Colombo</span></span>

<span data-ttu-id="aac22-183">Азия, Катманду</span><span class="sxs-lookup"><span data-stu-id="aac22-183">Asia/Kathmandu</span></span>

<span data-ttu-id="aac22-184">Азия, Астана</span><span class="sxs-lookup"><span data-stu-id="aac22-184">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="aac22-185">Азия, Дакка</span><span class="sxs-lookup"><span data-stu-id="aac22-185">Asia/Dhaka</span></span>

<span data-ttu-id="aac22-186">Азия, Екатеринбург</span><span class="sxs-lookup"><span data-stu-id="aac22-186">Asia/Yekaterinburg</span></span>

<span data-ttu-id="aac22-187">Азия, Янгон (Рангун)</span><span class="sxs-lookup"><span data-stu-id="aac22-187">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="aac22-188">Азия, Бангкок</span><span class="sxs-lookup"><span data-stu-id="aac22-188">Asia/Bangkok</span></span>

<span data-ttu-id="aac22-189">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="aac22-189">Asia/Novosibirsk</span></span>

<span data-ttu-id="aac22-190">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="aac22-190">Asia/Shanghai</span></span>

<span data-ttu-id="aac22-191">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="aac22-191">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="aac22-192">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="aac22-192">Asia/Singapore</span></span>

<span data-ttu-id="aac22-193">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="aac22-193">Australia/Perth</span></span>

<span data-ttu-id="aac22-194">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="aac22-194">Asia/Taipei</span></span>

<span data-ttu-id="aac22-195">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="aac22-195">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="aac22-196">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="aac22-196">Asia/Irkutsk</span></span>

<span data-ttu-id="aac22-197">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="aac22-197">Asia/Tokyo</span></span>

<span data-ttu-id="aac22-198">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="aac22-198">Asia/Seoul</span></span>

<span data-ttu-id="aac22-199">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="aac22-199">Australia/Adelaide</span></span>

<span data-ttu-id="aac22-200">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="aac22-200">Australia/Darwin</span></span>

<span data-ttu-id="aac22-201">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="aac22-201">Australia/Brisbane</span></span>

<span data-ttu-id="aac22-202">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="aac22-202">Australia/Sydney</span></span>

<span data-ttu-id="aac22-203">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="aac22-203">Pacific/Port_Moresby</span></span>

<span data-ttu-id="aac22-204">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="aac22-204">Australia/Hobart</span></span>

<span data-ttu-id="aac22-205">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="aac22-205">Asia/Yakutsk</span></span>

<span data-ttu-id="aac22-206">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="aac22-206">Pacific/Guadalcanal</span></span>

<span data-ttu-id="aac22-207">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="aac22-207">Asia/Vladivostok</span></span>

<span data-ttu-id="aac22-208">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="aac22-208">Pacific/Auckland</span></span>

<span data-ttu-id="aac22-209">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="aac22-209">Etc/GMT-12</span></span>

<span data-ttu-id="aac22-210">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="aac22-210">Pacific/Fiji</span></span>

<span data-ttu-id="aac22-211">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="aac22-211">Asia/Magadan</span></span>

<span data-ttu-id="aac22-212">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="aac22-212">Pacific/Tongatapu</span></span>

<span data-ttu-id="aac22-213">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="aac22-213">Pacific/Apia</span></span>

<span data-ttu-id="aac22-214">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="aac22-214">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="aac22-215">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aac22-215">JSON representation</span></span>

<span data-ttu-id="aac22-216">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aac22-216">Here is a JSON representation of the resource</span></span>

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
