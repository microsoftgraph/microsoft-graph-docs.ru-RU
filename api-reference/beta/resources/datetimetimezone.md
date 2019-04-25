---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Normal
ms.openlocfilehash: ee5359c0ababad2a4f785d17a02ac5bb618d2681
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535280"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="8758d-103">Тип ресурса dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8758d-103">dateTimeTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8758d-104">Описывает дату, время и часовой пояс для определенного момента.</span><span class="sxs-lookup"><span data-stu-id="8758d-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="8758d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8758d-105">Properties</span></span>
| <span data-ttu-id="8758d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8758d-106">Property</span></span>     | <span data-ttu-id="8758d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8758d-107">Type</span></span>   |<span data-ttu-id="8758d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8758d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8758d-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="8758d-109">dateTime</span></span>|<span data-ttu-id="8758d-110">String</span><span class="sxs-lookup"><span data-stu-id="8758d-110">String</span></span>|<span data-ttu-id="8758d-111">Один момент времени в объединенном представлении даты и времени (`{date}T{time}`).</span><span class="sxs-lookup"><span data-stu-id="8758d-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="8758d-112">Пример: "2019 – 04 – 16T09:00:00".</span><span class="sxs-lookup"><span data-stu-id="8758d-112">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="8758d-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="8758d-113">timeZone</span></span>|<span data-ttu-id="8758d-114">String</span><span class="sxs-lookup"><span data-stu-id="8758d-114">String</span></span>|<span data-ttu-id="8758d-115">Название часового пояса, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="8758d-115">A time zone name as described below.</span></span>|

<span data-ttu-id="8758d-116">Для свойства **TimeZone** можно задать любой часовой пояс, поддерживаемый Windows, а также следующие имена часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="8758d-116">The **timeZone** property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="8758d-117">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="8758d-117">Etc/GMT+12</span></span>

<span data-ttu-id="8758d-118">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="8758d-118">Etc/GMT+11</span></span>

<span data-ttu-id="8758d-119">Pacific/Honolulu</span><span class="sxs-lookup"><span data-stu-id="8758d-119">Pacific/Honolulu</span></span>

<span data-ttu-id="8758d-120">America/Anchorage</span><span class="sxs-lookup"><span data-stu-id="8758d-120">America/Anchorage</span></span>

<span data-ttu-id="8758d-121">America/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="8758d-121">America/Santa_Isabel</span></span>

<span data-ttu-id="8758d-122">America/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="8758d-122">America/Los_Angeles</span></span>

<span data-ttu-id="8758d-123">America/Phoenix</span><span class="sxs-lookup"><span data-stu-id="8758d-123">America/Phoenix</span></span>

<span data-ttu-id="8758d-124">America/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="8758d-124">America/Chihuahua</span></span>

<span data-ttu-id="8758d-125">America/Denver</span><span class="sxs-lookup"><span data-stu-id="8758d-125">America/Denver</span></span>

<span data-ttu-id="8758d-126">America/Guatemala</span><span class="sxs-lookup"><span data-stu-id="8758d-126">America/Guatemala</span></span>

<span data-ttu-id="8758d-127">America/Chicago</span><span class="sxs-lookup"><span data-stu-id="8758d-127">America/Chicago</span></span>

<span data-ttu-id="8758d-128">America/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="8758d-128">America/Mexico_City</span></span>

<span data-ttu-id="8758d-129">America/Regina</span><span class="sxs-lookup"><span data-stu-id="8758d-129">America/Regina</span></span>

<span data-ttu-id="8758d-130">America/Bogota</span><span class="sxs-lookup"><span data-stu-id="8758d-130">America/Bogota</span></span>

<span data-ttu-id="8758d-131">America/New_York</span><span class="sxs-lookup"><span data-stu-id="8758d-131">America/New_York</span></span>

<span data-ttu-id="8758d-132">America/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="8758d-132">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="8758d-133">America/Caracas</span><span class="sxs-lookup"><span data-stu-id="8758d-133">America/Caracas</span></span>

<span data-ttu-id="8758d-134">America/Asuncion</span><span class="sxs-lookup"><span data-stu-id="8758d-134">America/Asuncion</span></span>

<span data-ttu-id="8758d-135">America/Halifax</span><span class="sxs-lookup"><span data-stu-id="8758d-135">America/Halifax</span></span>

<span data-ttu-id="8758d-136">America/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="8758d-136">America/Cuiaba</span></span>

<span data-ttu-id="8758d-137">America/La_Paz</span><span class="sxs-lookup"><span data-stu-id="8758d-137">America/La_Paz</span></span>

<span data-ttu-id="8758d-138">America/Santiago</span><span class="sxs-lookup"><span data-stu-id="8758d-138">America/Santiago</span></span>

<span data-ttu-id="8758d-139">America/St_Johns</span><span class="sxs-lookup"><span data-stu-id="8758d-139">America/St_Johns</span></span>

<span data-ttu-id="8758d-140">America/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="8758d-140">America/Sao_Paulo</span></span>

<span data-ttu-id="8758d-141">America/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="8758d-141">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="8758d-142">America/Cayenne</span><span class="sxs-lookup"><span data-stu-id="8758d-142">America/Cayenne</span></span>

<span data-ttu-id="8758d-143">America/Godthab</span><span class="sxs-lookup"><span data-stu-id="8758d-143">America/Godthab</span></span>

<span data-ttu-id="8758d-144">America/Montevideo</span><span class="sxs-lookup"><span data-stu-id="8758d-144">America/Montevideo</span></span>

<span data-ttu-id="8758d-145">America/Bahia</span><span class="sxs-lookup"><span data-stu-id="8758d-145">America/Bahia</span></span>

<span data-ttu-id="8758d-146">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="8758d-146">Etc/GMT+2</span></span>

<span data-ttu-id="8758d-147">Atlantic/Azores</span><span class="sxs-lookup"><span data-stu-id="8758d-147">Atlantic/Azores</span></span>

<span data-ttu-id="8758d-148">Atlantic/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="8758d-148">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="8758d-149">Africa/Casablanca</span><span class="sxs-lookup"><span data-stu-id="8758d-149">Africa/Casablanca</span></span>

<span data-ttu-id="8758d-150">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="8758d-150">Etc/GMT</span></span>

<span data-ttu-id="8758d-151">Europe/London</span><span class="sxs-lookup"><span data-stu-id="8758d-151">Europe/London</span></span>

<span data-ttu-id="8758d-152">Atlantic/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="8758d-152">Atlantic/Reykjavik</span></span>

<span data-ttu-id="8758d-153">Europe/Berlin</span><span class="sxs-lookup"><span data-stu-id="8758d-153">Europe/Berlin</span></span>

<span data-ttu-id="8758d-154">Europe/Budapest</span><span class="sxs-lookup"><span data-stu-id="8758d-154">Europe/Budapest</span></span>

<span data-ttu-id="8758d-155">Europe/Paris</span><span class="sxs-lookup"><span data-stu-id="8758d-155">Europe/Paris</span></span>

<span data-ttu-id="8758d-156">Europe/Warsaw</span><span class="sxs-lookup"><span data-stu-id="8758d-156">Europe/Warsaw</span></span>

<span data-ttu-id="8758d-157">Africa/Lagos</span><span class="sxs-lookup"><span data-stu-id="8758d-157">Africa/Lagos</span></span>

<span data-ttu-id="8758d-158">Africa/Windhoek</span><span class="sxs-lookup"><span data-stu-id="8758d-158">Africa/Windhoek</span></span>

<span data-ttu-id="8758d-159">Europe/Bucharest</span><span class="sxs-lookup"><span data-stu-id="8758d-159">Europe/Bucharest</span></span>

<span data-ttu-id="8758d-160">Asia/Beirut</span><span class="sxs-lookup"><span data-stu-id="8758d-160">Asia/Beirut</span></span>

<span data-ttu-id="8758d-161">Africa/Cairo</span><span class="sxs-lookup"><span data-stu-id="8758d-161">Africa/Cairo</span></span>

<span data-ttu-id="8758d-162">Asia/Damascus</span><span class="sxs-lookup"><span data-stu-id="8758d-162">Asia/Damascus</span></span>

<span data-ttu-id="8758d-163">Африка, Йоханнесбург</span><span class="sxs-lookup"><span data-stu-id="8758d-163">Africa/Johannesburg</span></span>

<span data-ttu-id="8758d-164">Европа, Киев</span><span class="sxs-lookup"><span data-stu-id="8758d-164">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="8758d-165">Европа, Стамбул</span><span class="sxs-lookup"><span data-stu-id="8758d-165">Europe/Istanbul</span></span>

<span data-ttu-id="8758d-166">Asia/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="8758d-166">Asia/Jerusalem</span></span>

<span data-ttu-id="8758d-167">Asia/Amman</span><span class="sxs-lookup"><span data-stu-id="8758d-167">Asia/Amman</span></span>

<span data-ttu-id="8758d-168">Asia/Baghdad</span><span class="sxs-lookup"><span data-stu-id="8758d-168">Asia/Baghdad</span></span>

<span data-ttu-id="8758d-169">Europe/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="8758d-169">Europe/Kaliningrad</span></span>

<span data-ttu-id="8758d-170">Asia/Riyadh</span><span class="sxs-lookup"><span data-stu-id="8758d-170">Asia/Riyadh</span></span>

<span data-ttu-id="8758d-171">Africa/Nairobi</span><span class="sxs-lookup"><span data-stu-id="8758d-171">Africa/Nairobi</span></span>

<span data-ttu-id="8758d-172">Asia/Tehran</span><span class="sxs-lookup"><span data-stu-id="8758d-172">Asia/Tehran</span></span>

<span data-ttu-id="8758d-173">Asia/Dubai</span><span class="sxs-lookup"><span data-stu-id="8758d-173">Asia/Dubai</span></span>

<span data-ttu-id="8758d-174">Asia/Baku</span><span class="sxs-lookup"><span data-stu-id="8758d-174">Asia/Baku</span></span>

<span data-ttu-id="8758d-175">Europe/Moscow</span><span class="sxs-lookup"><span data-stu-id="8758d-175">Europe/Moscow</span></span>

<span data-ttu-id="8758d-176">Indian/Mauritius</span><span class="sxs-lookup"><span data-stu-id="8758d-176">Indian/Mauritius</span></span>

<span data-ttu-id="8758d-177">Asia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="8758d-177">Asia/Tbilisi</span></span>

<span data-ttu-id="8758d-178">Asia/Yerevan</span><span class="sxs-lookup"><span data-stu-id="8758d-178">Asia/Yerevan</span></span>

<span data-ttu-id="8758d-179">Asia/Kabul</span><span class="sxs-lookup"><span data-stu-id="8758d-179">Asia/Kabul</span></span>

<span data-ttu-id="8758d-180">Азия, Карачи</span><span class="sxs-lookup"><span data-stu-id="8758d-180">Asia/Karachi</span></span>

<span data-ttu-id="8758d-181">Азия, Ташкент</span><span class="sxs-lookup"><span data-stu-id="8758d-181">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="8758d-182">Азия, Колката</span><span class="sxs-lookup"><span data-stu-id="8758d-182">Asia/Kolkata</span></span>

<span data-ttu-id="8758d-183">Asia/Colombo</span><span class="sxs-lookup"><span data-stu-id="8758d-183">Asia/Colombo</span></span>

<span data-ttu-id="8758d-184">Азия, Катманду</span><span class="sxs-lookup"><span data-stu-id="8758d-184">Asia/Kathmandu</span></span>

<span data-ttu-id="8758d-185">Азия, Астана</span><span class="sxs-lookup"><span data-stu-id="8758d-185">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="8758d-186">Азия, Дакка</span><span class="sxs-lookup"><span data-stu-id="8758d-186">Asia/Dhaka</span></span>

<span data-ttu-id="8758d-187">Азия, Екатеринбург</span><span class="sxs-lookup"><span data-stu-id="8758d-187">Asia/Yekaterinburg</span></span>

<span data-ttu-id="8758d-188">Азия, Янгон (Рангун)</span><span class="sxs-lookup"><span data-stu-id="8758d-188">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="8758d-189">Азия, Бангкок</span><span class="sxs-lookup"><span data-stu-id="8758d-189">Asia/Bangkok</span></span>

<span data-ttu-id="8758d-190">Asia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="8758d-190">Asia/Novosibirsk</span></span>

<span data-ttu-id="8758d-191">Asia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="8758d-191">Asia/Shanghai</span></span>

<span data-ttu-id="8758d-192">Asia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="8758d-192">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="8758d-193">Asia/Singapore</span><span class="sxs-lookup"><span data-stu-id="8758d-193">Asia/Singapore</span></span>

<span data-ttu-id="8758d-194">Australia/Perth</span><span class="sxs-lookup"><span data-stu-id="8758d-194">Australia/Perth</span></span>

<span data-ttu-id="8758d-195">Asia/Taipei</span><span class="sxs-lookup"><span data-stu-id="8758d-195">Asia/Taipei</span></span>

<span data-ttu-id="8758d-196">Asia/Ulaanbaatar</span><span class="sxs-lookup"><span data-stu-id="8758d-196">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="8758d-197">Asia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="8758d-197">Asia/Irkutsk</span></span>

<span data-ttu-id="8758d-198">Asia/Tokyo</span><span class="sxs-lookup"><span data-stu-id="8758d-198">Asia/Tokyo</span></span>

<span data-ttu-id="8758d-199">Asia/Seoul</span><span class="sxs-lookup"><span data-stu-id="8758d-199">Asia/Seoul</span></span>

<span data-ttu-id="8758d-200">Australia/Adelaide</span><span class="sxs-lookup"><span data-stu-id="8758d-200">Australia/Adelaide</span></span>

<span data-ttu-id="8758d-201">Australia/Darwin</span><span class="sxs-lookup"><span data-stu-id="8758d-201">Australia/Darwin</span></span>

<span data-ttu-id="8758d-202">Australia/Brisbane</span><span class="sxs-lookup"><span data-stu-id="8758d-202">Australia/Brisbane</span></span>

<span data-ttu-id="8758d-203">Australia/Sydney</span><span class="sxs-lookup"><span data-stu-id="8758d-203">Australia/Sydney</span></span>

<span data-ttu-id="8758d-204">Pacific/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="8758d-204">Pacific/Port_Moresby</span></span>

<span data-ttu-id="8758d-205">Australia/Hobart</span><span class="sxs-lookup"><span data-stu-id="8758d-205">Australia/Hobart</span></span>

<span data-ttu-id="8758d-206">Asia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="8758d-206">Asia/Yakutsk</span></span>

<span data-ttu-id="8758d-207">Pacific/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="8758d-207">Pacific/Guadalcanal</span></span>

<span data-ttu-id="8758d-208">Asia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="8758d-208">Asia/Vladivostok</span></span>

<span data-ttu-id="8758d-209">Pacific/Auckland</span><span class="sxs-lookup"><span data-stu-id="8758d-209">Pacific/Auckland</span></span>

<span data-ttu-id="8758d-210">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="8758d-210">Etc/GMT-12</span></span>

<span data-ttu-id="8758d-211">Pacific/Fiji</span><span class="sxs-lookup"><span data-stu-id="8758d-211">Pacific/Fiji</span></span>

<span data-ttu-id="8758d-212">Asia/Magadan</span><span class="sxs-lookup"><span data-stu-id="8758d-212">Asia/Magadan</span></span>

<span data-ttu-id="8758d-213">Pacific/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="8758d-213">Pacific/Tongatapu</span></span>

<span data-ttu-id="8758d-214">Pacific/Apia</span><span class="sxs-lookup"><span data-stu-id="8758d-214">Pacific/Apia</span></span>

<span data-ttu-id="8758d-215">Pacific/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="8758d-215">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="8758d-216">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8758d-216">JSON representation</span></span>

<span data-ttu-id="8758d-217">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8758d-217">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/datetimetimezone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
