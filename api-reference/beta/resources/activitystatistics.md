---
title: Тип ресурса Активитистатистикс
description: Представляет время, затраченное на рабочие действия, включая электронную почту, собрания, фокусы, разговоры и звонки.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5cee94c1ff36bf30d977b7eb97d77f11d4d2ff5e
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450809"
---
# <a name="activitystatistics-resource-type"></a><span data-ttu-id="5842b-103">Тип ресурса Активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="5842b-103">activityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5842b-104">Представляет время, затраченное пользователем на выполнение различных действий в течение и за пределами рабочего времени, для указанного диапазона времени в запросе, в котором используется период агрегирования за один день.</span><span class="sxs-lookup"><span data-stu-id="5842b-104">Represents time spent by a user on various work activities during and outside of working hours, for the specified time range in the request, which uses an aggregation period of one day.</span></span>

<span data-ttu-id="5842b-105">Следующие типы статистики являются производными от **активитистатистикс**:</span><span class="sxs-lookup"><span data-stu-id="5842b-105">The following types of statistics are derived from **activityStatistics**:</span></span>

* [<span data-ttu-id="5842b-106">Call</span><span class="sxs-lookup"><span data-stu-id="5842b-106">Call</span></span>](callactivitystatistics.md)
* [<span data-ttu-id="5842b-107">Чат</span><span class="sxs-lookup"><span data-stu-id="5842b-107">Chat</span></span>](chatactivitystatistics.md)
* [<span data-ttu-id="5842b-108">Email</span><span class="sxs-lookup"><span data-stu-id="5842b-108">Email</span></span>](emailactivitystatistics.md)
* [<span data-ttu-id="5842b-109">Фокус</span><span class="sxs-lookup"><span data-stu-id="5842b-109">Focus</span></span>](focusactivitystatistics.md)
* [<span data-ttu-id="5842b-110">Назначить</span><span class="sxs-lookup"><span data-stu-id="5842b-110">Meeting</span></span>](meetingactivitystatistics.md)

### <a name="activity-id-property"></a><span data-ttu-id="5842b-111">Свойство идентификатора действия</span><span class="sxs-lookup"><span data-stu-id="5842b-111">Activity id property</span></span>

<span data-ttu-id="5842b-112">В HTTP-запросе для получения определенного типа статистики действий в диапазоне дат можно выразить эту информацию как идентификатор коллекции пользователей Активитистатистикс в следующем формате, где `{startdate}` и `{enddate}` в календаре ISO 8601. формат даты и `{activity}` может иметь следующий вид: "Call", "Chat", "Email", "Focus" или "Meeting".</span><span class="sxs-lookup"><span data-stu-id="5842b-112">In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":</span></span>

```
{activity}_{startdate}_{enddate}
```

<span data-ttu-id="5842b-113">Например, идентификатор "email_2019 – 08 -10 _2019 – 08 – 12" представляет Емаилактивитистатистикс для указанного пользователя между 10 августа 2019 и 12 августа 2019.</span><span class="sxs-lookup"><span data-stu-id="5842b-113">For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="5842b-114">Методы</span><span class="sxs-lookup"><span data-stu-id="5842b-114">Methods</span></span>

| <span data-ttu-id="5842b-115">Метод</span><span class="sxs-lookup"><span data-stu-id="5842b-115">Method</span></span>       | <span data-ttu-id="5842b-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5842b-116">Return Type</span></span> | <span data-ttu-id="5842b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="5842b-117">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5842b-118">Получение Активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="5842b-118">Get activityStatistics</span></span>](../api/activitystatistics-get.md) | [<span data-ttu-id="5842b-119">активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="5842b-119">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="5842b-120">Получение свойств для статистики указанного действия пользователя за указанный диапазон времени.</span><span class="sxs-lookup"><span data-stu-id="5842b-120">Get the properties for a specified activity's statistics for a user, for the specified time range.</span></span> |
| [<span data-ttu-id="5842b-121">Список Активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="5842b-121">List activityStatistics</span></span>](../api/activitystatistics-list.md) | [<span data-ttu-id="5842b-122">активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="5842b-122">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="5842b-123">Получение свойств для коллекции статистики действий пользователя за последнюю полную неделю.</span><span class="sxs-lookup"><span data-stu-id="5842b-123">Retrieve the properties for the collection of activity statistics for a user, for the last complete week.</span></span>|

## <a name="properties"></a><span data-ttu-id="5842b-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="5842b-124">Properties</span></span>

| <span data-ttu-id="5842b-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="5842b-125">Property</span></span>     | <span data-ttu-id="5842b-126">Тип</span><span class="sxs-lookup"><span data-stu-id="5842b-126">Type</span></span>        | <span data-ttu-id="5842b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="5842b-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5842b-128">activity</span><span class="sxs-lookup"><span data-stu-id="5842b-128">activity</span></span>|<span data-ttu-id="5842b-129">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="5842b-129">analyticsActivityType</span></span>| <span data-ttu-id="5842b-130">Тип действия, для которого возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="5842b-130">The type of activity for which statistics are returned.</span></span> <span data-ttu-id="5842b-131">Возможные значения: `call`, `chat`, `email`, `focus`и. `meeting`</span><span class="sxs-lookup"><span data-stu-id="5842b-131">The possible values are: `call`, `chat`, `email`, `focus`, and `meeting`.</span></span>|
|<span data-ttu-id="5842b-132">duration</span><span class="sxs-lookup"><span data-stu-id="5842b-132">duration</span></span>|<span data-ttu-id="5842b-133">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="5842b-133">Duration</span></span>|<span data-ttu-id="5842b-134">Общее количество часов, потраченных на действие.</span><span class="sxs-lookup"><span data-stu-id="5842b-134">Total hours spent on the activity.</span></span> <span data-ttu-id="5842b-135">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="5842b-135">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="5842b-136">endDate</span><span class="sxs-lookup"><span data-stu-id="5842b-136">endDate</span></span>|<span data-ttu-id="5842b-137">Date</span><span class="sxs-lookup"><span data-stu-id="5842b-137">Date</span></span>|<span data-ttu-id="5842b-138">Дата завершения действия, выраженная в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="5842b-138">Date when the activity ended, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="5842b-139">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="5842b-139">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="5842b-140">id</span><span class="sxs-lookup"><span data-stu-id="5842b-140">id</span></span>|<span data-ttu-id="5842b-141">String</span><span class="sxs-lookup"><span data-stu-id="5842b-141">String</span></span>| <span data-ttu-id="5842b-142">Идентификатор для операции, который представляется `{activity}_{startdate}_{enddate}`только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5842b-142">Read-only ID for the activity, which represents `{activity}_{startdate}_{enddate}`.</span></span>|
|<span data-ttu-id="5842b-143">startDate</span><span class="sxs-lookup"><span data-stu-id="5842b-143">startDate</span></span>|<span data-ttu-id="5842b-144">Дата</span><span class="sxs-lookup"><span data-stu-id="5842b-144">Date</span></span>|<span data-ttu-id="5842b-145">Дата начала действия, выраженная в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="5842b-145">Date when the activity started, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="5842b-146">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="5842b-146">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="5842b-147">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="5842b-147">timeZoneUsed</span></span>|<span data-ttu-id="5842b-148">String</span><span class="sxs-lookup"><span data-stu-id="5842b-148">String</span></span>|<span data-ttu-id="5842b-149">Часовой пояс, который пользователь задает в Microsoft Outlook для вычисления.</span><span class="sxs-lookup"><span data-stu-id="5842b-149">The time zone that the user sets in Microsoft Outlook is used for the computation.</span></span> <span data-ttu-id="5842b-150">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="5842b-150">For example, the property value could be "Pacific Standard Time."</span></span>|

## <a name="relationships"></a><span data-ttu-id="5842b-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="5842b-151">Relationships</span></span>

<span data-ttu-id="5842b-152">Нет</span><span class="sxs-lookup"><span data-stu-id="5842b-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5842b-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5842b-153">JSON representation</span></span>

<span data-ttu-id="5842b-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5842b-154">The following is a JSON representation of the resource.</span></span>

<!-- { 
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityStatistics",
  "keyProperty": "id"
}-->

```json
{
  "activity": "String",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601 format)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601 format)",
  "timeZoneUsed": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}--> 