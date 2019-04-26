---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Priority
ms.openlocfilehash: 9e031b053ebc185ee02fa11571019529a870cf04
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574773"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="ef867-103">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ef867-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="ef867-104">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="ef867-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="ef867-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef867-105">Properties</span></span>
| <span data-ttu-id="ef867-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef867-106">Property</span></span>     | <span data-ttu-id="ef867-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ef867-107">Type</span></span>   |<span data-ttu-id="ef867-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ef867-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef867-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="ef867-109">dateTime</span></span>|<span data-ttu-id="ef867-110">String</span><span class="sxs-lookup"><span data-stu-id="ef867-110">String</span></span>|<span data-ttu-id="ef867-111">Один момент времени в объединенном представлении даты и времени (`{date}T{time}`; например, `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="ef867-111">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="ef867-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="ef867-112">timeZone</span></span>|<span data-ttu-id="ef867-113">String</span><span class="sxs-lookup"><span data-stu-id="ef867-113">String</span></span>|<span data-ttu-id="ef867-114">Один из указанных ниже часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="ef867-114">One of the following time zone names.</span></span>|

<span data-ttu-id="ef867-115">Свойство _TimeZone_ можно задать для каждого из часовых поясов, которые поддерживаются в Windows, а также для указанных ниже часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="ef867-115">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="ef867-116">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="ef867-116">Etc/GMT+12</span></span>

<span data-ttu-id="ef867-117">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="ef867-117">Etc/GMT+11</span></span>

<span data-ttu-id="ef867-118">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="ef867-118">Pacific/Honolulu</span></span>

<span data-ttu-id="ef867-119">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="ef867-119">America/Anchorage</span></span>

<span data-ttu-id="ef867-120">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="ef867-120">America/Santa_Isabel</span></span>

<span data-ttu-id="ef867-121">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="ef867-121">America/Los_Angeles</span></span>

<span data-ttu-id="ef867-122">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="ef867-122">America/Phoenix</span></span>

<span data-ttu-id="ef867-123">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="ef867-123">America/Chihuahua</span></span>

<span data-ttu-id="ef867-124">America/Denver</span><span class="sxs-lookup"><span data-stu-id="ef867-124">America/Denver</span></span>

<span data-ttu-id="ef867-125">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="ef867-125">America/Guatemala</span></span>

<span data-ttu-id="ef867-126">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="ef867-126">America/Chicago</span></span>

<span data-ttu-id="ef867-127">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="ef867-127">America/Mexico_City</span></span>

<span data-ttu-id="ef867-128">America/Regina</span><span class="sxs-lookup"><span data-stu-id="ef867-128">America/Regina</span></span>

<span data-ttu-id="ef867-129">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="ef867-129">America/Bogota</span></span>

<span data-ttu-id="ef867-130">America/New_York</span><span class="sxs-lookup"><span data-stu-id="ef867-130">America/New_York</span></span>

<span data-ttu-id="ef867-131">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="ef867-131">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="ef867-132">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="ef867-132">America/Caracas</span></span>

<span data-ttu-id="ef867-133">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="ef867-133">America/Asuncion</span></span>

<span data-ttu-id="ef867-134">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="ef867-134">America/Halifax</span></span>

<span data-ttu-id="ef867-135">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="ef867-135">America/Cuiaba</span></span>

<span data-ttu-id="ef867-136">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="ef867-136">America/La_Paz</span></span>

<span data-ttu-id="ef867-137">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="ef867-137">America/Santiago</span></span>

<span data-ttu-id="ef867-138">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="ef867-138">America/St_Johns</span></span>

<span data-ttu-id="ef867-139">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="ef867-139">America/Sao_Paulo</span></span>

<span data-ttu-id="ef867-140">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="ef867-140">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="ef867-141">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="ef867-141">America/Cayenne</span></span>

<span data-ttu-id="ef867-142">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="ef867-142">America/Godthab</span></span>

<span data-ttu-id="ef867-143">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="ef867-143">America/Montevideo</span></span>

<span data-ttu-id="ef867-144">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="ef867-144">America/Bahia</span></span>

<span data-ttu-id="ef867-145">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="ef867-145">Etc/GMT+2</span></span>

<span data-ttu-id="ef867-146">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="ef867-146">Atlantic/Azores</span></span>

<span data-ttu-id="ef867-147">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="ef867-147">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="ef867-148">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="ef867-148">Africa/Casablanca</span></span>

<span data-ttu-id="ef867-149">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="ef867-149">Etc/GMT</span></span>

<span data-ttu-id="ef867-150">Europe/London</span><span class="sxs-lookup"><span data-stu-id="ef867-150">Europe/London</span></span>

<span data-ttu-id="ef867-151">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="ef867-151">Atlantic/Reykjavik</span></span>

<span data-ttu-id="ef867-152">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="ef867-152">Europe/Berlin</span></span>

<span data-ttu-id="ef867-153">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="ef867-153">Europe/Budapest</span></span>

<span data-ttu-id="ef867-154">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="ef867-154">Europe/Paris</span></span>

<span data-ttu-id="ef867-155">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="ef867-155">Europe/Warsaw</span></span>

<span data-ttu-id="ef867-156">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="ef867-156">Africa/Lagos</span></span>

<span data-ttu-id="ef867-157">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="ef867-157">Africa/Windhoek</span></span>

<span data-ttu-id="ef867-158">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="ef867-158">Europe/Bucharest</span></span>

<span data-ttu-id="ef867-159">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="ef867-159">Asia/Beirut</span></span>

<span data-ttu-id="ef867-160">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="ef867-160">Africa/Cairo</span></span>

<span data-ttu-id="ef867-161">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="ef867-161">Asia/Damascus</span></span>

<span data-ttu-id="ef867-162">Африка, Йоханнесбург</span><span class="sxs-lookup"><span data-stu-id="ef867-162">Africa/Johannesburg</span></span>

<span data-ttu-id="ef867-163">Европа, Киев</span><span class="sxs-lookup"><span data-stu-id="ef867-163">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="ef867-164">Европа, Стамбул</span><span class="sxs-lookup"><span data-stu-id="ef867-164">Europe/Istanbul</span></span>

<span data-ttu-id="ef867-165">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="ef867-165">Asia/Jerusalem</span></span>

<span data-ttu-id="ef867-166">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="ef867-166">Asia/Amman</span></span>

<span data-ttu-id="ef867-167">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="ef867-167">Asia/Baghdad</span></span>

<span data-ttu-id="ef867-168">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="ef867-168">Europe/Kaliningrad</span></span>

<span data-ttu-id="ef867-169">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="ef867-169">Asia/Riyadh</span></span>

<span data-ttu-id="ef867-170">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="ef867-170">Africa/Nairobi</span></span>

<span data-ttu-id="ef867-171">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="ef867-171">Asia/Tehran</span></span>

<span data-ttu-id="ef867-172">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="ef867-172">Asia/Dubai</span></span>

<span data-ttu-id="ef867-173">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="ef867-173">Asia/Baku</span></span>

<span data-ttu-id="ef867-174">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="ef867-174">Europe/Moscow</span></span>

<span data-ttu-id="ef867-175">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="ef867-175">Indian/Mauritius</span></span>

<span data-ttu-id="ef867-176">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="ef867-176">Asia/Tbilisi</span></span>

<span data-ttu-id="ef867-177">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="ef867-177">Asia/Yerevan</span></span>

<span data-ttu-id="ef867-178">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="ef867-178">Asia/Kabul</span></span>

<span data-ttu-id="ef867-179">Азия, Карачи</span><span class="sxs-lookup"><span data-stu-id="ef867-179">Asia/Karachi</span></span>

<span data-ttu-id="ef867-180">Азия, Ташкент</span><span class="sxs-lookup"><span data-stu-id="ef867-180">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="ef867-181">Азия, Колката</span><span class="sxs-lookup"><span data-stu-id="ef867-181">Asia/Kolkata</span></span>

<span data-ttu-id="ef867-182">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="ef867-182">Asia/Colombo</span></span>

<span data-ttu-id="ef867-183">Азия, Катманду</span><span class="sxs-lookup"><span data-stu-id="ef867-183">Asia/Kathmandu</span></span>

<span data-ttu-id="ef867-184">Азия, Астана</span><span class="sxs-lookup"><span data-stu-id="ef867-184">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="ef867-185">Азия, Дакка</span><span class="sxs-lookup"><span data-stu-id="ef867-185">Asia/Dhaka</span></span>

<span data-ttu-id="ef867-186">Азия, Екатеринбург</span><span class="sxs-lookup"><span data-stu-id="ef867-186">Asia/Yekaterinburg</span></span>

<span data-ttu-id="ef867-187">Азия, Янгон (Рангун)</span><span class="sxs-lookup"><span data-stu-id="ef867-187">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="ef867-188">Азия, Бангкок</span><span class="sxs-lookup"><span data-stu-id="ef867-188">Asia/Bangkok</span></span>

<span data-ttu-id="ef867-189">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="ef867-189">Asia/Novosibirsk</span></span>

<span data-ttu-id="ef867-190">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="ef867-190">Asia/Shanghai</span></span>

<span data-ttu-id="ef867-191">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="ef867-191">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="ef867-192">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="ef867-192">Asia/Singapore</span></span>

<span data-ttu-id="ef867-193">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="ef867-193">Australia/Perth</span></span>

<span data-ttu-id="ef867-194">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="ef867-194">Asia/Taipei</span></span>

<span data-ttu-id="ef867-195">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="ef867-195">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="ef867-196">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="ef867-196">Asia/Irkutsk</span></span>

<span data-ttu-id="ef867-197">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="ef867-197">Asia/Tokyo</span></span>

<span data-ttu-id="ef867-198">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="ef867-198">Asia/Seoul</span></span>

<span data-ttu-id="ef867-199">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="ef867-199">Australia/Adelaide</span></span>

<span data-ttu-id="ef867-200">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="ef867-200">Australia/Darwin</span></span>

<span data-ttu-id="ef867-201">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="ef867-201">Australia/Brisbane</span></span>

<span data-ttu-id="ef867-202">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="ef867-202">Australia/Sydney</span></span>

<span data-ttu-id="ef867-203">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="ef867-203">Pacific/Port_Moresby</span></span>

<span data-ttu-id="ef867-204">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="ef867-204">Australia/Hobart</span></span>

<span data-ttu-id="ef867-205">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="ef867-205">Asia/Yakutsk</span></span>

<span data-ttu-id="ef867-206">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="ef867-206">Pacific/Guadalcanal</span></span>

<span data-ttu-id="ef867-207">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="ef867-207">Asia/Vladivostok</span></span>

<span data-ttu-id="ef867-208">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="ef867-208">Pacific/Auckland</span></span>

<span data-ttu-id="ef867-209">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="ef867-209">Etc/GMT-12</span></span>

<span data-ttu-id="ef867-210">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="ef867-210">Pacific/Fiji</span></span>

<span data-ttu-id="ef867-211">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="ef867-211">Asia/Magadan</span></span>

<span data-ttu-id="ef867-212">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="ef867-212">Pacific/Tongatapu</span></span>

<span data-ttu-id="ef867-213">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="ef867-213">Pacific/Apia</span></span>

<span data-ttu-id="ef867-214">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="ef867-214">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef867-215">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ef867-215">JSON representation</span></span>

<span data-ttu-id="ef867-216">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef867-216">Here is a JSON representation of the resource</span></span>

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
