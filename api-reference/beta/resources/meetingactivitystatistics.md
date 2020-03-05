---
title: Тип ресурса Митингактивитистатистикс
description: Представляет сведения о действиях с собраниями для пользователей.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 039d2be82a08057c9f9a5405d3591898304a8bcc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522752"
---
# <a name="meetingactivitystatistics-resource-type"></a><span data-ttu-id="94ea5-103">Тип ресурса Митингактивитистатистикс</span><span class="sxs-lookup"><span data-stu-id="94ea5-103">meetingActivityStatistics resource type</span></span>

<span data-ttu-id="94ea5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="94ea5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94ea5-105">Представляет данные о времени пользователя, затраченного на собрания в Microsoft Outlook, Microsoft Teams или Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="94ea5-105">Represents data about the user's time spent in meetings in Microsoft Outlook, Microsoft Teams, or Skype for Business.</span></span> <span data-ttu-id="94ea5-106">Это основано на [активитистатистикс](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="94ea5-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>
<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Read properties and relationships of meetingActivityStatistics object; name of the activity for which statistics are returned as “meeting.” |
-->
## <a name="properties"></a><span data-ttu-id="94ea5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="94ea5-107">Properties</span></span>

| <span data-ttu-id="94ea5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="94ea5-108">Property</span></span>     | <span data-ttu-id="94ea5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="94ea5-109">Type</span></span>        | <span data-ttu-id="94ea5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="94ea5-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94ea5-111">activity</span><span class="sxs-lookup"><span data-stu-id="94ea5-111">activity</span></span>|<span data-ttu-id="94ea5-112">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="94ea5-112">analyticsActivityType</span></span>| <span data-ttu-id="94ea5-113">Действия собраний, для которых возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="94ea5-113">Meeting activity for which statistics are returned.</span></span>|
|<span data-ttu-id="94ea5-114">duration</span><span class="sxs-lookup"><span data-stu-id="94ea5-114">duration</span></span>|<span data-ttu-id="94ea5-115">Длительность</span><span class="sxs-lookup"><span data-stu-id="94ea5-115">Duration</span></span>|<span data-ttu-id="94ea5-116">Общее количество часов, потраченных на собрания.</span><span class="sxs-lookup"><span data-stu-id="94ea5-116">Total hours spent on meetings.</span></span> <span data-ttu-id="94ea5-117">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="94ea5-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="94ea5-118">endDate</span><span class="sxs-lookup"><span data-stu-id="94ea5-118">endDate</span></span>|<span data-ttu-id="94ea5-119">Date</span><span class="sxs-lookup"><span data-stu-id="94ea5-119">Date</span></span>|<span data-ttu-id="94ea5-120">Дата завершения действия собрания.</span><span class="sxs-lookup"><span data-stu-id="94ea5-120">Date when the meeting activity ended.</span></span> <span data-ttu-id="94ea5-121">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="94ea5-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="94ea5-122">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="94ea5-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="94ea5-123">id</span><span class="sxs-lookup"><span data-stu-id="94ea5-123">id</span></span>|<span data-ttu-id="94ea5-124">String</span><span class="sxs-lookup"><span data-stu-id="94ea5-124">String</span></span>| <span data-ttu-id="94ea5-125">Идентификатор, предназначенный только для чтения, для действия собрания.</span><span class="sxs-lookup"><span data-stu-id="94ea5-125">Read-only ID for the meeting activity.</span></span>|
|<span data-ttu-id="94ea5-126">startDate</span><span class="sxs-lookup"><span data-stu-id="94ea5-126">startDate</span></span>|<span data-ttu-id="94ea5-127">Дата</span><span class="sxs-lookup"><span data-stu-id="94ea5-127">Date</span></span>|<span data-ttu-id="94ea5-128">Дата начала действия собрания.</span><span class="sxs-lookup"><span data-stu-id="94ea5-128">Date when the meeting activity started.</span></span> <span data-ttu-id="94ea5-129">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="94ea5-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="94ea5-130">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="94ea5-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="94ea5-131">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="94ea5-131">timeZoneUsed</span></span>|<span data-ttu-id="94ea5-132">String</span><span class="sxs-lookup"><span data-stu-id="94ea5-132">String</span></span>|<span data-ttu-id="94ea5-133">Для вычисления используется часовой пояс Outlook, который пользователь задает в календаре Outlook.</span><span class="sxs-lookup"><span data-stu-id="94ea5-133">The Outlook time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="94ea5-134">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="94ea5-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="94ea5-135">афтерхаурс</span><span class="sxs-lookup"><span data-stu-id="94ea5-135">afterHours</span></span>|<span data-ttu-id="94ea5-136">Длительность</span><span class="sxs-lookup"><span data-stu-id="94ea5-136">Duration</span></span>|<span data-ttu-id="94ea5-137">Время, затраченное на собрания в нерабочее время, которое основано на параметре календаря пользователя Outlook для рабочих часов.</span><span class="sxs-lookup"><span data-stu-id="94ea5-137">Time spent on meetings outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="94ea5-138">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="94ea5-138">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="94ea5-139">конфликтующие</span><span class="sxs-lookup"><span data-stu-id="94ea5-139">conflicting</span></span>|<span data-ttu-id="94ea5-140">Длительность</span><span class="sxs-lookup"><span data-stu-id="94ea5-140">Duration</span></span>|<span data-ttu-id="94ea5-141">Время, затраченное на конфликтующие собрания (собрания, перекрывающиеся с другими собраниями, которые он принял, и состоянием "занято").</span><span class="sxs-lookup"><span data-stu-id="94ea5-141">Time spent in conflicting meetings (meetings that overlap with other meetings that the person accepted and where the person’s status is set to Busy).</span></span> <span data-ttu-id="94ea5-142">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="94ea5-142">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="94ea5-143">long</span><span class="sxs-lookup"><span data-stu-id="94ea5-143">long</span></span>|<span data-ttu-id="94ea5-144">Длительность</span><span class="sxs-lookup"><span data-stu-id="94ea5-144">Duration</span></span>|<span data-ttu-id="94ea5-145">Время, затраченное на длительные собрания (более часа в течение длительного времени).</span><span class="sxs-lookup"><span data-stu-id="94ea5-145">Time spent in long meetings (more than an hour in duration).</span></span> <span data-ttu-id="94ea5-146">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="94ea5-146">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="94ea5-147">многозадачность</span><span class="sxs-lookup"><span data-stu-id="94ea5-147">multitasking</span></span>|<span data-ttu-id="94ea5-148">Длительность</span><span class="sxs-lookup"><span data-stu-id="94ea5-148">Duration</span></span>|<span data-ttu-id="94ea5-149">Время, затраченное на собрания, в которых пользователь выполнял многозадачность (чтение и отправка превышает минимальное количество сообщений электронной почты и/или отправляет больше минимального количества сообщений в Teams или Skype для бизнеса).</span><span class="sxs-lookup"><span data-stu-id="94ea5-149">Time spent in meetings where the person was multitasking (read/sent more than a minimum number of emails and/or sent more than a minimum number of messages in Teams or in Skype for Business).</span></span> <span data-ttu-id="94ea5-150">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="94ea5-150">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="94ea5-151">распределяют</span><span class="sxs-lookup"><span data-stu-id="94ea5-151">organized</span></span>|<span data-ttu-id="94ea5-152">Длительность</span><span class="sxs-lookup"><span data-stu-id="94ea5-152">Duration</span></span>|<span data-ttu-id="94ea5-153">Время, затраченное на собрания, организованные пользователем.</span><span class="sxs-lookup"><span data-stu-id="94ea5-153">Time spent in meetings organized by the user.</span></span> <span data-ttu-id="94ea5-154">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="94ea5-154">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="94ea5-155">повторяющихся</span><span class="sxs-lookup"><span data-stu-id="94ea5-155">recurring</span></span>|<span data-ttu-id="94ea5-156">Длительность</span><span class="sxs-lookup"><span data-stu-id="94ea5-156">Duration</span></span>|<span data-ttu-id="94ea5-157">Время, затраченное на повторяющиеся собрания.</span><span class="sxs-lookup"><span data-stu-id="94ea5-157">Time spent on recurring meetings.</span></span> <span data-ttu-id="94ea5-158">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="94ea5-158">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94ea5-159">Связи</span><span class="sxs-lookup"><span data-stu-id="94ea5-159">Relationships</span></span>

<span data-ttu-id="94ea5-160">Нет</span><span class="sxs-lookup"><span data-stu-id="94ea5-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94ea5-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94ea5-161">JSON representation</span></span>

<span data-ttu-id="94ea5-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94ea5-162">The following is a JSON representation of the resource.</span></span>

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