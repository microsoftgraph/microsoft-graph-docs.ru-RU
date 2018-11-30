---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
ms.openlocfilehash: a95ebf35d6a47b8b39c34cab8d6d35b92eaae2c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077336"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="2603f-103">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2603f-103">dateTimeTimeZone resource type</span></span>

> <span data-ttu-id="2603f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2603f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2603f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2603f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2603f-106">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="2603f-106">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="2603f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2603f-107">Properties</span></span>
| <span data-ttu-id="2603f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2603f-108">Property</span></span>     | <span data-ttu-id="2603f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2603f-109">Type</span></span>   |<span data-ttu-id="2603f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2603f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2603f-111">DateTime</span><span class="sxs-lookup"><span data-stu-id="2603f-111">DateTime</span></span>|<span data-ttu-id="2603f-112">String</span><span class="sxs-lookup"><span data-stu-id="2603f-112">String</span></span>|<span data-ttu-id="2603f-113">Один момент времени в объединенном представлении даты и времени (`<date>T<time>`).</span><span class="sxs-lookup"><span data-stu-id="2603f-113">A single point of time in a combined date and time representation (`<date>T<time>`).</span></span>|
|<span data-ttu-id="2603f-114">TimeZone</span><span class="sxs-lookup"><span data-stu-id="2603f-114">TimeZone</span></span>|<span data-ttu-id="2603f-115">String</span><span class="sxs-lookup"><span data-stu-id="2603f-115">String</span></span>|<span data-ttu-id="2603f-116">Один из указанных ниже часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="2603f-116">One of the following time zone names.</span></span>|

<span data-ttu-id="2603f-117">Свойство _TimeZone_ можно задать для каждого из часовых поясов, которые поддерживаются в Windows, а также для указанных ниже часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="2603f-117">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="2603f-118">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="2603f-118">Etc/GMT+12</span></span>

<span data-ttu-id="2603f-119">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="2603f-119">Etc/GMT+11</span></span>

<span data-ttu-id="2603f-120">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="2603f-120">Pacific/Honolulu</span></span>

<span data-ttu-id="2603f-121">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="2603f-121">America/Anchorage</span></span>

<span data-ttu-id="2603f-122">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="2603f-122">America/Santa_Isabel</span></span>

<span data-ttu-id="2603f-123">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="2603f-123">America/Los_Angeles</span></span>

<span data-ttu-id="2603f-124">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="2603f-124">America/Phoenix</span></span>

<span data-ttu-id="2603f-125">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="2603f-125">America/Chihuahua</span></span>

<span data-ttu-id="2603f-126">America/Denver</span><span class="sxs-lookup"><span data-stu-id="2603f-126">America/Denver</span></span>

<span data-ttu-id="2603f-127">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="2603f-127">America/Guatemala</span></span>

<span data-ttu-id="2603f-128">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="2603f-128">America/Chicago</span></span>

<span data-ttu-id="2603f-129">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="2603f-129">America/Mexico_City</span></span>

<span data-ttu-id="2603f-130">America/Regina</span><span class="sxs-lookup"><span data-stu-id="2603f-130">America/Regina</span></span>

<span data-ttu-id="2603f-131">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="2603f-131">America/Bogota</span></span>

<span data-ttu-id="2603f-132">America/New_York</span><span class="sxs-lookup"><span data-stu-id="2603f-132">America/New_York</span></span>

<span data-ttu-id="2603f-133">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="2603f-133">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="2603f-134">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="2603f-134">America/Caracas</span></span>

<span data-ttu-id="2603f-135">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="2603f-135">America/Asuncion</span></span>

<span data-ttu-id="2603f-136">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="2603f-136">America/Halifax</span></span>

<span data-ttu-id="2603f-137">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="2603f-137">America/Cuiaba</span></span>

<span data-ttu-id="2603f-138">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="2603f-138">America/La_Paz</span></span>

<span data-ttu-id="2603f-139">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="2603f-139">America/Santiago</span></span>

<span data-ttu-id="2603f-140">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="2603f-140">America/St_Johns</span></span>

<span data-ttu-id="2603f-141">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="2603f-141">America/Sao_Paulo</span></span>

<span data-ttu-id="2603f-142">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="2603f-142">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="2603f-143">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="2603f-143">America/Cayenne</span></span>

<span data-ttu-id="2603f-144">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="2603f-144">America/Godthab</span></span>

<span data-ttu-id="2603f-145">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="2603f-145">America/Montevideo</span></span>

<span data-ttu-id="2603f-146">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="2603f-146">America/Bahia</span></span>

<span data-ttu-id="2603f-147">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="2603f-147">Etc/GMT+2</span></span>

<span data-ttu-id="2603f-148">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="2603f-148">Atlantic/Azores</span></span>

<span data-ttu-id="2603f-149">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="2603f-149">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="2603f-150">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="2603f-150">Africa/Casablanca</span></span>

<span data-ttu-id="2603f-151">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="2603f-151">Etc/GMT</span></span>

<span data-ttu-id="2603f-152">Europe/London</span><span class="sxs-lookup"><span data-stu-id="2603f-152">Europe/London</span></span>

<span data-ttu-id="2603f-153">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="2603f-153">Atlantic/Reykjavik</span></span>

<span data-ttu-id="2603f-154">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="2603f-154">Europe/Berlin</span></span>

<span data-ttu-id="2603f-155">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="2603f-155">Europe/Budapest</span></span>

<span data-ttu-id="2603f-156">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="2603f-156">Europe/Paris</span></span>

<span data-ttu-id="2603f-157">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="2603f-157">Europe/Warsaw</span></span>

<span data-ttu-id="2603f-158">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="2603f-158">Africa/Lagos</span></span>

<span data-ttu-id="2603f-159">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="2603f-159">Africa/Windhoek</span></span>

<span data-ttu-id="2603f-160">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="2603f-160">Europe/Bucharest</span></span>

<span data-ttu-id="2603f-161">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="2603f-161">Asia/Beirut</span></span>

<span data-ttu-id="2603f-162">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="2603f-162">Africa/Cairo</span></span>

<span data-ttu-id="2603f-163">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="2603f-163">Asia/Damascus</span></span>

<span data-ttu-id="2603f-164">Африка, Йоханнесбург</span><span class="sxs-lookup"><span data-stu-id="2603f-164">Africa/Johannesburg</span></span>

<span data-ttu-id="2603f-165">Европа, Киев</span><span class="sxs-lookup"><span data-stu-id="2603f-165">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="2603f-166">Европа, Стамбул</span><span class="sxs-lookup"><span data-stu-id="2603f-166">Europe/Istanbul</span></span>

<span data-ttu-id="2603f-167">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="2603f-167">Asia/Jerusalem</span></span>

<span data-ttu-id="2603f-168">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="2603f-168">Asia/Amman</span></span>

<span data-ttu-id="2603f-169">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="2603f-169">Asia/Baghdad</span></span>

<span data-ttu-id="2603f-170">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="2603f-170">Europe/Kaliningrad</span></span>

<span data-ttu-id="2603f-171">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="2603f-171">Asia/Riyadh</span></span>

<span data-ttu-id="2603f-172">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="2603f-172">Africa/Nairobi</span></span>

<span data-ttu-id="2603f-173">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="2603f-173">Asia/Tehran</span></span>

<span data-ttu-id="2603f-174">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="2603f-174">Asia/Dubai</span></span>

<span data-ttu-id="2603f-175">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="2603f-175">Asia/Baku</span></span>

<span data-ttu-id="2603f-176">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="2603f-176">Europe/Moscow</span></span>

<span data-ttu-id="2603f-177">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="2603f-177">Indian/Mauritius</span></span>

<span data-ttu-id="2603f-178">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="2603f-178">Asia/Tbilisi</span></span>

<span data-ttu-id="2603f-179">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="2603f-179">Asia/Yerevan</span></span>

<span data-ttu-id="2603f-180">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="2603f-180">Asia/Kabul</span></span>

<span data-ttu-id="2603f-181">Азия, Карачи</span><span class="sxs-lookup"><span data-stu-id="2603f-181">Asia/Karachi</span></span>

<span data-ttu-id="2603f-182">Азия, Ташкент</span><span class="sxs-lookup"><span data-stu-id="2603f-182">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="2603f-183">Азия, Колката</span><span class="sxs-lookup"><span data-stu-id="2603f-183">Asia/Kolkata</span></span>

<span data-ttu-id="2603f-184">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="2603f-184">Asia/Colombo</span></span>

<span data-ttu-id="2603f-185">Азия, Катманду</span><span class="sxs-lookup"><span data-stu-id="2603f-185">Asia/Kathmandu</span></span>

<span data-ttu-id="2603f-186">Азия, Астана</span><span class="sxs-lookup"><span data-stu-id="2603f-186">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="2603f-187">Азия, Дакка</span><span class="sxs-lookup"><span data-stu-id="2603f-187">Asia/Dhaka</span></span>

<span data-ttu-id="2603f-188">Азия, Екатеринбург</span><span class="sxs-lookup"><span data-stu-id="2603f-188">Asia/Yekaterinburg</span></span>

<span data-ttu-id="2603f-189">Азия, Янгон (Рангун)</span><span class="sxs-lookup"><span data-stu-id="2603f-189">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="2603f-190">Азия, Бангкок</span><span class="sxs-lookup"><span data-stu-id="2603f-190">Asia/Bangkok</span></span>

<span data-ttu-id="2603f-191">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="2603f-191">Asia/Novosibirsk</span></span>

<span data-ttu-id="2603f-192">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="2603f-192">Asia/Shanghai</span></span>

<span data-ttu-id="2603f-193">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="2603f-193">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="2603f-194">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="2603f-194">Asia/Singapore</span></span>

<span data-ttu-id="2603f-195">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="2603f-195">Australia/Perth</span></span>

<span data-ttu-id="2603f-196">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="2603f-196">Asia/Taipei</span></span>

<span data-ttu-id="2603f-197">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="2603f-197">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="2603f-198">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="2603f-198">Asia/Irkutsk</span></span>

<span data-ttu-id="2603f-199">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="2603f-199">Asia/Tokyo</span></span>

<span data-ttu-id="2603f-200">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="2603f-200">Asia/Seoul</span></span>

<span data-ttu-id="2603f-201">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="2603f-201">Australia/Adelaide</span></span>

<span data-ttu-id="2603f-202">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="2603f-202">Australia/Darwin</span></span>

<span data-ttu-id="2603f-203">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="2603f-203">Australia/Brisbane</span></span>

<span data-ttu-id="2603f-204">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="2603f-204">Australia/Sydney</span></span>

<span data-ttu-id="2603f-205">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="2603f-205">Pacific/Port_Moresby</span></span>

<span data-ttu-id="2603f-206">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="2603f-206">Australia/Hobart</span></span>

<span data-ttu-id="2603f-207">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="2603f-207">Asia/Yakutsk</span></span>

<span data-ttu-id="2603f-208">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="2603f-208">Pacific/Guadalcanal</span></span>

<span data-ttu-id="2603f-209">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="2603f-209">Asia/Vladivostok</span></span>

<span data-ttu-id="2603f-210">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="2603f-210">Pacific/Auckland</span></span>

<span data-ttu-id="2603f-211">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="2603f-211">Etc/GMT-12</span></span>

<span data-ttu-id="2603f-212">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="2603f-212">Pacific/Fiji</span></span>

<span data-ttu-id="2603f-213">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="2603f-213">Asia/Magadan</span></span>

<span data-ttu-id="2603f-214">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="2603f-214">Pacific/Tongatapu</span></span>

<span data-ttu-id="2603f-215">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="2603f-215">Pacific/Apia</span></span>

<span data-ttu-id="2603f-216">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="2603f-216">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="2603f-217">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2603f-217">JSON representation</span></span>

<span data-ttu-id="2603f-218">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2603f-218">Here is a JSON representation of the resource</span></span>

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
