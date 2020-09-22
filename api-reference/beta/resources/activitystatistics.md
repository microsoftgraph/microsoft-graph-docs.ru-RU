---
title: Тип ресурса Активитистатистикс
description: Представляет время, затраченное на рабочие действия, включая электронную почту, собрания, фокусы, разговоры и звонки.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: e94f9ad746c497e3b81eff6b919c50a59c6a0a11
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004284"
---
# <a name="activitystatistics-resource-type"></a><span data-ttu-id="b6d84-103">Тип ресурса Активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="b6d84-103">activityStatistics resource type</span></span>

<span data-ttu-id="b6d84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6d84-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6d84-105">Представляет время, затраченное пользователем на выполнение различных действий в течение и за пределами рабочего времени, для указанного диапазона времени в запросе, в котором используется период агрегирования за один день.</span><span class="sxs-lookup"><span data-stu-id="b6d84-105">Represents time spent by a user on various work activities during and outside of working hours, for the specified time range in the request, which uses an aggregation period of one day.</span></span>

<span data-ttu-id="b6d84-106">Следующие типы статистики являются производными от **активитистатистикс**:</span><span class="sxs-lookup"><span data-stu-id="b6d84-106">The following types of statistics are derived from **activityStatistics**:</span></span>

* [<span data-ttu-id="b6d84-107">Звонок</span><span class="sxs-lookup"><span data-stu-id="b6d84-107">Call</span></span>](callactivitystatistics.md)
* [<span data-ttu-id="b6d84-108">Отображаются</span><span class="sxs-lookup"><span data-stu-id="b6d84-108">Chat</span></span>](chatactivitystatistics.md)
* [<span data-ttu-id="b6d84-109">Электронная почта</span><span class="sxs-lookup"><span data-stu-id="b6d84-109">Email</span></span>](emailactivitystatistics.md)
* [<span data-ttu-id="b6d84-110">Фокус</span><span class="sxs-lookup"><span data-stu-id="b6d84-110">Focus</span></span>](focusactivitystatistics.md)
* [<span data-ttu-id="b6d84-111">Назначить</span><span class="sxs-lookup"><span data-stu-id="b6d84-111">Meeting</span></span>](meetingactivitystatistics.md)

<!--  removing per Mathew 2/6/2020   ### Activity id property

In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":

```
{activity}_{startdate}_{enddate}
```

For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.
-->
## <a name="methods"></a><span data-ttu-id="b6d84-112">Методы</span><span class="sxs-lookup"><span data-stu-id="b6d84-112">Methods</span></span>

| <span data-ttu-id="b6d84-113">Метод</span><span class="sxs-lookup"><span data-stu-id="b6d84-113">Method</span></span>       | <span data-ttu-id="b6d84-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b6d84-114">Return Type</span></span> | <span data-ttu-id="b6d84-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b6d84-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b6d84-116">Список Активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="b6d84-116">List activityStatistics</span></span>](../api/activitystatistics-list.md) | [<span data-ttu-id="b6d84-117">активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="b6d84-117">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="b6d84-118">Получение свойств для коллекции статистики действий пользователя за последнюю полную неделю.</span><span class="sxs-lookup"><span data-stu-id="b6d84-118">Retrieve the properties for the collection of activity statistics for a user, for the last complete week.</span></span> |

## <a name="properties"></a><span data-ttu-id="b6d84-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6d84-119">Properties</span></span>

| <span data-ttu-id="b6d84-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6d84-120">Property</span></span>     | <span data-ttu-id="b6d84-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b6d84-121">Type</span></span>        | <span data-ttu-id="b6d84-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b6d84-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b6d84-123">activity</span><span class="sxs-lookup"><span data-stu-id="b6d84-123">activity</span></span> |<span data-ttu-id="b6d84-124">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="b6d84-124">analyticsActivityType</span></span> |<span data-ttu-id="b6d84-125">Тип действия, для которого возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="b6d84-125">The type of activity for which statistics are returned.</span></span> <span data-ttu-id="b6d84-126">Возможные значения:,, `call` `chat` `email` , `focus` и `meeting` .</span><span class="sxs-lookup"><span data-stu-id="b6d84-126">The possible values are: `call`, `chat`, `email`, `focus`, and `meeting`.</span></span> |
|<span data-ttu-id="b6d84-127">duration</span><span class="sxs-lookup"><span data-stu-id="b6d84-127">duration</span></span> |<span data-ttu-id="b6d84-128">Длительность</span><span class="sxs-lookup"><span data-stu-id="b6d84-128">Duration</span></span> |<span data-ttu-id="b6d84-129">Общее количество часов, потраченных на действие.</span><span class="sxs-lookup"><span data-stu-id="b6d84-129">Total hours spent on the activity.</span></span> <span data-ttu-id="b6d84-130">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="b6d84-130">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="b6d84-131">endDate</span><span class="sxs-lookup"><span data-stu-id="b6d84-131">endDate</span></span> |<span data-ttu-id="b6d84-132">Date</span><span class="sxs-lookup"><span data-stu-id="b6d84-132">Date</span></span> |<span data-ttu-id="b6d84-133">Дата завершения действия, выраженная в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="b6d84-133">Date when the activity ended, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="b6d84-134">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="b6d84-134">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span> |
|<span data-ttu-id="b6d84-135">id</span><span class="sxs-lookup"><span data-stu-id="b6d84-135">id</span></span> |<span data-ttu-id="b6d84-136">String</span><span class="sxs-lookup"><span data-stu-id="b6d84-136">String</span></span> |<span data-ttu-id="b6d84-137">Идентификатор действия, предназначенный только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6d84-137">Read-only ID for the activity.</span></span> <span data-ttu-id="b6d84-138">Не проанализируйте и не настраивайте значение для своих сценариев.</span><span class="sxs-lookup"><span data-stu-id="b6d84-138">Do not parse or customize the value for your scenarios.</span></span> |
|<span data-ttu-id="b6d84-139">startDate</span><span class="sxs-lookup"><span data-stu-id="b6d84-139">startDate</span></span> |<span data-ttu-id="b6d84-140">Date</span><span class="sxs-lookup"><span data-stu-id="b6d84-140">Date</span></span> |<span data-ttu-id="b6d84-141">Дата начала действия, выраженная в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="b6d84-141">Date when the activity started, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="b6d84-142">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="b6d84-142">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span> |
|<span data-ttu-id="b6d84-143">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="b6d84-143">timeZoneUsed</span></span> |<span data-ttu-id="b6d84-144">String</span><span class="sxs-lookup"><span data-stu-id="b6d84-144">String</span></span> |<span data-ttu-id="b6d84-145">Часовой пояс, который пользователь задает в Microsoft Outlook для вычисления.</span><span class="sxs-lookup"><span data-stu-id="b6d84-145">The time zone that the user sets in Microsoft Outlook is used for the computation.</span></span> <span data-ttu-id="b6d84-146">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="b6d84-146">For example, the property value could be "Pacific Standard Time."</span></span> |

## <a name="relationships"></a><span data-ttu-id="b6d84-147">Связи</span><span class="sxs-lookup"><span data-stu-id="b6d84-147">Relationships</span></span>

<span data-ttu-id="b6d84-148">Нет</span><span class="sxs-lookup"><span data-stu-id="b6d84-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6d84-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6d84-149">JSON representation</span></span>

<span data-ttu-id="b6d84-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6d84-150">The following is a JSON representation of the resource.</span></span>

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

