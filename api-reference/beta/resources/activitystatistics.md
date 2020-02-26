---
title: Тип ресурса Активитистатистикс
description: Представляет время, затраченное на рабочие действия, включая электронную почту, собрания, фокусы, разговоры и звонки.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3d2e626535d579b77c27125500d7247401f26915
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280619"
---
# <a name="activitystatistics-resource-type"></a><span data-ttu-id="da2ee-103">Тип ресурса Активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="da2ee-103">activityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da2ee-104">Представляет время, затраченное пользователем на выполнение различных действий в течение и за пределами рабочего времени, для указанного диапазона времени в запросе, в котором используется период агрегирования за один день.</span><span class="sxs-lookup"><span data-stu-id="da2ee-104">Represents time spent by a user on various work activities during and outside of working hours, for the specified time range in the request, which uses an aggregation period of one day.</span></span>

<span data-ttu-id="da2ee-105">Следующие типы статистики являются производными от **активитистатистикс**:</span><span class="sxs-lookup"><span data-stu-id="da2ee-105">The following types of statistics are derived from **activityStatistics**:</span></span>

* [<span data-ttu-id="da2ee-106">Call</span><span class="sxs-lookup"><span data-stu-id="da2ee-106">Call</span></span>](callactivitystatistics.md)
* [<span data-ttu-id="da2ee-107">Отображаются</span><span class="sxs-lookup"><span data-stu-id="da2ee-107">Chat</span></span>](chatactivitystatistics.md)
* [<span data-ttu-id="da2ee-108">Электронная почта</span><span class="sxs-lookup"><span data-stu-id="da2ee-108">Email</span></span>](emailactivitystatistics.md)
* [<span data-ttu-id="da2ee-109">Фокус</span><span class="sxs-lookup"><span data-stu-id="da2ee-109">Focus</span></span>](focusactivitystatistics.md)
* [<span data-ttu-id="da2ee-110">Назначить</span><span class="sxs-lookup"><span data-stu-id="da2ee-110">Meeting</span></span>](meetingactivitystatistics.md)

<!--  removing per Mathew 2/6/2020   ### Activity id property

In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":

```
{activity}_{startdate}_{enddate}
```

For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.
-->
## <a name="methods"></a><span data-ttu-id="da2ee-111">Методы</span><span class="sxs-lookup"><span data-stu-id="da2ee-111">Methods</span></span>

| <span data-ttu-id="da2ee-112">Метод</span><span class="sxs-lookup"><span data-stu-id="da2ee-112">Method</span></span>       | <span data-ttu-id="da2ee-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="da2ee-113">Return Type</span></span> | <span data-ttu-id="da2ee-114">Описание</span><span class="sxs-lookup"><span data-stu-id="da2ee-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="da2ee-115">Список Активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="da2ee-115">List activityStatistics</span></span>](../api/activitystatistics-list.md) | [<span data-ttu-id="da2ee-116">активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="da2ee-116">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="da2ee-117">Получение свойств для коллекции статистики действий пользователя за последнюю полную неделю.</span><span class="sxs-lookup"><span data-stu-id="da2ee-117">Retrieve the properties for the collection of activity statistics for a user, for the last complete week.</span></span> |

## <a name="properties"></a><span data-ttu-id="da2ee-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="da2ee-118">Properties</span></span>

| <span data-ttu-id="da2ee-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="da2ee-119">Property</span></span>     | <span data-ttu-id="da2ee-120">Тип</span><span class="sxs-lookup"><span data-stu-id="da2ee-120">Type</span></span>        | <span data-ttu-id="da2ee-121">Описание</span><span class="sxs-lookup"><span data-stu-id="da2ee-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da2ee-122">activity</span><span class="sxs-lookup"><span data-stu-id="da2ee-122">activity</span></span> |<span data-ttu-id="da2ee-123">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="da2ee-123">analyticsActivityType</span></span> |<span data-ttu-id="da2ee-124">Тип действия, для которого возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="da2ee-124">The type of activity for which statistics are returned.</span></span> <span data-ttu-id="da2ee-125">Возможные значения: `call`, `chat`, `email`, `focus`и. `meeting`</span><span class="sxs-lookup"><span data-stu-id="da2ee-125">The possible values are: `call`, `chat`, `email`, `focus`, and `meeting`.</span></span> |
|<span data-ttu-id="da2ee-126">duration</span><span class="sxs-lookup"><span data-stu-id="da2ee-126">duration</span></span> |<span data-ttu-id="da2ee-127">Длительность</span><span class="sxs-lookup"><span data-stu-id="da2ee-127">Duration</span></span> |<span data-ttu-id="da2ee-128">Общее количество часов, потраченных на действие.</span><span class="sxs-lookup"><span data-stu-id="da2ee-128">Total hours spent on the activity.</span></span> <span data-ttu-id="da2ee-129">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="da2ee-129">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="da2ee-130">endDate</span><span class="sxs-lookup"><span data-stu-id="da2ee-130">endDate</span></span> |<span data-ttu-id="da2ee-131">Date</span><span class="sxs-lookup"><span data-stu-id="da2ee-131">Date</span></span> |<span data-ttu-id="da2ee-132">Дата завершения действия, выраженная в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="da2ee-132">Date when the activity ended, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="da2ee-133">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="da2ee-133">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span> |
|<span data-ttu-id="da2ee-134">id</span><span class="sxs-lookup"><span data-stu-id="da2ee-134">id</span></span> |<span data-ttu-id="da2ee-135">String</span><span class="sxs-lookup"><span data-stu-id="da2ee-135">String</span></span> |<span data-ttu-id="da2ee-136">Идентификатор действия, предназначенный только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da2ee-136">Read-only ID for the activity.</span></span> <span data-ttu-id="da2ee-137">Не проанализируйте и не настраивайте значение для своих сценариев.</span><span class="sxs-lookup"><span data-stu-id="da2ee-137">Do not parse or customize the value for your scenarios.</span></span> |
|<span data-ttu-id="da2ee-138">startDate</span><span class="sxs-lookup"><span data-stu-id="da2ee-138">startDate</span></span> |<span data-ttu-id="da2ee-139">Дата</span><span class="sxs-lookup"><span data-stu-id="da2ee-139">Date</span></span> |<span data-ttu-id="da2ee-140">Дата начала действия, выраженная в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="da2ee-140">Date when the activity started, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="da2ee-141">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="da2ee-141">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span> |
|<span data-ttu-id="da2ee-142">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="da2ee-142">timeZoneUsed</span></span> |<span data-ttu-id="da2ee-143">String</span><span class="sxs-lookup"><span data-stu-id="da2ee-143">String</span></span> |<span data-ttu-id="da2ee-144">Часовой пояс, который пользователь задает в Microsoft Outlook для вычисления.</span><span class="sxs-lookup"><span data-stu-id="da2ee-144">The time zone that the user sets in Microsoft Outlook is used for the computation.</span></span> <span data-ttu-id="da2ee-145">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="da2ee-145">For example, the property value could be "Pacific Standard Time."</span></span> |

## <a name="relationships"></a><span data-ttu-id="da2ee-146">Связи</span><span class="sxs-lookup"><span data-stu-id="da2ee-146">Relationships</span></span>

<span data-ttu-id="da2ee-147">Нет</span><span class="sxs-lookup"><span data-stu-id="da2ee-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da2ee-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da2ee-148">JSON representation</span></span>

<span data-ttu-id="da2ee-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da2ee-149">The following is a JSON representation of the resource.</span></span>

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