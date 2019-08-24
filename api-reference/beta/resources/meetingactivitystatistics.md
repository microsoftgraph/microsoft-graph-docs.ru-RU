---
title: Тип ресурса Митингактивитистатистикс
description: Представляет сведения о действиях с собраниями для пользователей.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 14d926a41680f1292b7599bd76b458705b426719
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622539"
---
# <a name="meetingactivitystatistics-resource-type"></a><span data-ttu-id="b993e-103">Тип ресурса Митингактивитистатистикс</span><span class="sxs-lookup"><span data-stu-id="b993e-103">meetingActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b993e-104">Представляет данные о времени пользователя, затраченного на собрания в Microsoft Outlook, Microsoft Teams или Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b993e-104">Represents data about the user's time spent in meetings in Microsoft Outlook, Microsoft Teams, or Skype for Business.</span></span> <span data-ttu-id="b993e-105">Это основано на [активитистатистикс](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="b993e-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>
<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Read properties and relationships of meetingActivityStatistics object; name of the activity for which statistics are returned as “meeting.” |
-->
## <a name="properties"></a><span data-ttu-id="b993e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b993e-106">Properties</span></span>

| <span data-ttu-id="b993e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b993e-107">Property</span></span>     | <span data-ttu-id="b993e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b993e-108">Type</span></span>        | <span data-ttu-id="b993e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b993e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b993e-110">activity</span><span class="sxs-lookup"><span data-stu-id="b993e-110">activity</span></span>|<span data-ttu-id="b993e-111">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="b993e-111">analyticsActivityType</span></span>| <span data-ttu-id="b993e-112">Действия собраний, для которых возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="b993e-112">Meeting activity for which statistics are returned.</span></span>|
|<span data-ttu-id="b993e-113">duration</span><span class="sxs-lookup"><span data-stu-id="b993e-113">duration</span></span>|<span data-ttu-id="b993e-114">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="b993e-114">Duration</span></span>|<span data-ttu-id="b993e-115">Общее количество часов, потраченных на собрания.</span><span class="sxs-lookup"><span data-stu-id="b993e-115">Total hours spent on meetings.</span></span> <span data-ttu-id="b993e-116">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="b993e-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="b993e-117">endDate</span><span class="sxs-lookup"><span data-stu-id="b993e-117">endDate</span></span>|<span data-ttu-id="b993e-118">Date</span><span class="sxs-lookup"><span data-stu-id="b993e-118">Date</span></span>|<span data-ttu-id="b993e-119">Дата завершения действия собрания.</span><span class="sxs-lookup"><span data-stu-id="b993e-119">Date when the meeting activity ended.</span></span> <span data-ttu-id="b993e-120">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="b993e-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="b993e-121">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="b993e-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="b993e-122">id</span><span class="sxs-lookup"><span data-stu-id="b993e-122">id</span></span>|<span data-ttu-id="b993e-123">String</span><span class="sxs-lookup"><span data-stu-id="b993e-123">String</span></span>| <span data-ttu-id="b993e-124">Идентификатор, предназначенный только для чтения, для действия собрания.</span><span class="sxs-lookup"><span data-stu-id="b993e-124">Read-only ID for the meeting activity.</span></span>|
|<span data-ttu-id="b993e-125">startDate</span><span class="sxs-lookup"><span data-stu-id="b993e-125">startDate</span></span>|<span data-ttu-id="b993e-126">Дата</span><span class="sxs-lookup"><span data-stu-id="b993e-126">Date</span></span>|<span data-ttu-id="b993e-127">Дата начала действия собрания.</span><span class="sxs-lookup"><span data-stu-id="b993e-127">Date when the meeting activity started.</span></span> <span data-ttu-id="b993e-128">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="b993e-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="b993e-129">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="b993e-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="b993e-130">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="b993e-130">timeZoneUsed</span></span>|<span data-ttu-id="b993e-131">String.</span><span class="sxs-lookup"><span data-stu-id="b993e-131">String</span></span>|<span data-ttu-id="b993e-132">Для вычисления используется часовой пояс Outlook, который пользователь задает в календаре Outlook.</span><span class="sxs-lookup"><span data-stu-id="b993e-132">The Outlook time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="b993e-133">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="b993e-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="b993e-134">афтерхаурс</span><span class="sxs-lookup"><span data-stu-id="b993e-134">afterHours</span></span>|<span data-ttu-id="b993e-135">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="b993e-135">Duration</span></span>|<span data-ttu-id="b993e-136">Время, затраченное на собрания в нерабочее время, которое основано на параметре календаря пользователя Outlook для рабочих часов.</span><span class="sxs-lookup"><span data-stu-id="b993e-136">Time spent on meetings outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="b993e-137">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="b993e-137">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="b993e-138">конфликтующие</span><span class="sxs-lookup"><span data-stu-id="b993e-138">conflicting</span></span>|<span data-ttu-id="b993e-139">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="b993e-139">Duration</span></span>|<span data-ttu-id="b993e-140">Время, затраченное на конфликтующие собрания (собрания, перекрывающиеся с другими собраниями, которые он принял, и состоянием "занято").</span><span class="sxs-lookup"><span data-stu-id="b993e-140">Time spent in conflicting meetings (meetings that overlap with other meetings that the person accepted and where the person’s status is set to Busy).</span></span> <span data-ttu-id="b993e-141">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="b993e-141">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="b993e-142">long</span><span class="sxs-lookup"><span data-stu-id="b993e-142">long</span></span>|<span data-ttu-id="b993e-143">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="b993e-143">Duration</span></span>|<span data-ttu-id="b993e-144">Время, затраченное на длительные собрания (более часа в течение длительного времени).</span><span class="sxs-lookup"><span data-stu-id="b993e-144">Time spent in long meetings (more than an hour in duration).</span></span> <span data-ttu-id="b993e-145">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="b993e-145">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="b993e-146">многозадачность</span><span class="sxs-lookup"><span data-stu-id="b993e-146">multitasking</span></span>|<span data-ttu-id="b993e-147">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="b993e-147">Duration</span></span>|<span data-ttu-id="b993e-148">Время, затраченное на собрания, в которых пользователь выполнял многозадачность (чтение и отправка превышает минимальное количество сообщений электронной почты и/или отправляет больше минимального количества сообщений в Teams или Skype для бизнеса).</span><span class="sxs-lookup"><span data-stu-id="b993e-148">Time spent in meetings where the person was multitasking (read/sent more than a minimum number of emails and/or sent more than a minimum number of messages in Teams or in Skype for Business).</span></span> <span data-ttu-id="b993e-149">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="b993e-149">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="b993e-150">распределяют</span><span class="sxs-lookup"><span data-stu-id="b993e-150">organized</span></span>|<span data-ttu-id="b993e-151">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="b993e-151">Duration</span></span>|<span data-ttu-id="b993e-152">Время, затраченное на собрания, организованные пользователем.</span><span class="sxs-lookup"><span data-stu-id="b993e-152">Time spent in meetings organized by the user.</span></span> <span data-ttu-id="b993e-153">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="b993e-153">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="b993e-154">повторяющихся</span><span class="sxs-lookup"><span data-stu-id="b993e-154">recurring</span></span>|<span data-ttu-id="b993e-155">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="b993e-155">Duration</span></span>|<span data-ttu-id="b993e-156">Время, затраченное на повторяющиеся собрания.</span><span class="sxs-lookup"><span data-stu-id="b993e-156">Time spent on recurring meetings.</span></span> <span data-ttu-id="b993e-157">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="b993e-157">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b993e-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="b993e-158">Relationships</span></span>

<span data-ttu-id="b993e-159">Нет</span><span class="sxs-lookup"><span data-stu-id="b993e-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b993e-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b993e-160">JSON representation</span></span>

<span data-ttu-id="b993e-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b993e-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)",
  "conflicting": "String (ISO 8601 duration)",
  "long": "String (ISO 8601 duration)",
  "multitasking": "String (ISO 8601 duration)",
  "organized": "String (ISO 8601 duration)",
  "recurring": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->