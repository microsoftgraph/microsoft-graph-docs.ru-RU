---
title: Тип ресурса Емаилактивитистатистикс
description: Представляет дополнительные сведения о действиях электронной почты для пользователей
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ff75545b7f591a920ed4a1ffd65bff40cff8439b
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450813"
---
# <a name="emailactivitystatistics-resource-type"></a><span data-ttu-id="f628d-103">Тип ресурса Емаилактивитистатистикс</span><span class="sxs-lookup"><span data-stu-id="f628d-103">emailActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f628d-104">Представляет данные о времени, затраченном пользователем на действия с электронной почтой, в Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="f628d-104">Represents data about the user's time spent in email activities in Microsoft Outlook.</span></span> <span data-ttu-id="f628d-105">Это основано на [активитистатистикс](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="f628d-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f628d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f628d-106">Properties</span></span>

| <span data-ttu-id="f628d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f628d-107">Property</span></span>     | <span data-ttu-id="f628d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f628d-108">Type</span></span>        | <span data-ttu-id="f628d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f628d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f628d-110">activity</span><span class="sxs-lookup"><span data-stu-id="f628d-110">activity</span></span>|<span data-ttu-id="f628d-111">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="f628d-111">analyticsActivityType</span></span>| <span data-ttu-id="f628d-112">Действия электронной почты, для которых возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="f628d-112">Email activity for which statistics are returned.</span></span>|
|<span data-ttu-id="f628d-113">duration</span><span class="sxs-lookup"><span data-stu-id="f628d-113">duration</span></span>|<span data-ttu-id="f628d-114">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="f628d-114">Duration</span></span>|<span data-ttu-id="f628d-115">Общее количество часов, потраченных на электронную почту.</span><span class="sxs-lookup"><span data-stu-id="f628d-115">Total hours spent on emails.</span></span> <span data-ttu-id="f628d-116">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="f628d-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="f628d-117">endDate</span><span class="sxs-lookup"><span data-stu-id="f628d-117">endDate</span></span>|<span data-ttu-id="f628d-118">Date</span><span class="sxs-lookup"><span data-stu-id="f628d-118">Date</span></span>|<span data-ttu-id="f628d-119">Дата окончания действия электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f628d-119">Date when the email activity ended.</span></span> <span data-ttu-id="f628d-120">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="f628d-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="f628d-121">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="f628d-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="f628d-122">id</span><span class="sxs-lookup"><span data-stu-id="f628d-122">id</span></span>|<span data-ttu-id="f628d-123">String</span><span class="sxs-lookup"><span data-stu-id="f628d-123">String</span></span>| <span data-ttu-id="f628d-124">Идентификатор, предназначенный только для чтения, для действия электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f628d-124">Read-only ID for the email activity.</span></span>|
|<span data-ttu-id="f628d-125">startDate</span><span class="sxs-lookup"><span data-stu-id="f628d-125">startDate</span></span>|<span data-ttu-id="f628d-126">Дата</span><span class="sxs-lookup"><span data-stu-id="f628d-126">Date</span></span>|<span data-ttu-id="f628d-127">Дата начала действия электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f628d-127">Date when the email activity started.</span></span> <span data-ttu-id="f628d-128">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="f628d-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="f628d-129">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="f628d-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="f628d-130">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="f628d-130">timeZoneUsed</span></span>|<span data-ttu-id="f628d-131">String</span><span class="sxs-lookup"><span data-stu-id="f628d-131">String</span></span>|<span data-ttu-id="f628d-132">Часовой пояс, который пользователь задает в календаре Outlook для вычисления.</span><span class="sxs-lookup"><span data-stu-id="f628d-132">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="f628d-133">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="f628d-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="f628d-134">афтерхаурс</span><span class="sxs-lookup"><span data-stu-id="f628d-134">afterHours</span></span>|<span data-ttu-id="f628d-135">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="f628d-135">Duration</span></span>|<span data-ttu-id="f628d-136">Общее количество часов, потраченных на электронную почту за прев рабочее время, которая основана на параметре календаря пользователя Outlook для рабочих часов.</span><span class="sxs-lookup"><span data-stu-id="f628d-136">Total hours spent on email outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="f628d-137">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="f628d-137">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="f628d-138">реадемаил</span><span class="sxs-lookup"><span data-stu-id="f628d-138">readEmail</span></span>|<span data-ttu-id="f628d-139">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="f628d-139">Duration</span></span>|<span data-ttu-id="f628d-140">Общее количество часов, потраченных на чтение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f628d-140">Total hours spent reading email.</span></span> <span data-ttu-id="f628d-141">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="f628d-141">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="f628d-142">сентемаил</span><span class="sxs-lookup"><span data-stu-id="f628d-142">sentEmail</span></span>|<span data-ttu-id="f628d-143">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="f628d-143">Duration</span></span>|<span data-ttu-id="f628d-144">Общее количество часов, потраченных на запись и отправку электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f628d-144">Total hours spent writing and sending email.</span></span> <span data-ttu-id="f628d-145">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="f628d-145">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f628d-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="f628d-146">Relationships</span></span>

<span data-ttu-id="f628d-147">Нет</span><span class="sxs-lookup"><span data-stu-id="f628d-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f628d-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f628d-148">JSON representation</span></span>

<span data-ttu-id="f628d-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f628d-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailActivityStatistics"
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
  "readEmail": "String (ISO 8601 duration)",
  "sentEmail": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->