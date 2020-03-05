---
title: Тип ресурса Емаилактивитистатистикс
description: Представляет дополнительные сведения о действиях электронной почты для пользователей
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: f2bd2d84d6f7dbc18fc5e37079eebc4289dd2ee2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499598"
---
# <a name="emailactivitystatistics-resource-type"></a><span data-ttu-id="5a31a-103">Тип ресурса Емаилактивитистатистикс</span><span class="sxs-lookup"><span data-stu-id="5a31a-103">emailActivityStatistics resource type</span></span>

<span data-ttu-id="5a31a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5a31a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a31a-105">Представляет данные о времени, затраченном пользователем на действия с электронной почтой, в Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="5a31a-105">Represents data about the user's time spent in email activities in Microsoft Outlook.</span></span> <span data-ttu-id="5a31a-106">Это основано на [активитистатистикс](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="5a31a-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5a31a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a31a-107">Properties</span></span>

| <span data-ttu-id="5a31a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a31a-108">Property</span></span>     | <span data-ttu-id="5a31a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5a31a-109">Type</span></span>        | <span data-ttu-id="5a31a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5a31a-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5a31a-111">activity</span><span class="sxs-lookup"><span data-stu-id="5a31a-111">activity</span></span>|<span data-ttu-id="5a31a-112">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="5a31a-112">analyticsActivityType</span></span>| <span data-ttu-id="5a31a-113">Действия электронной почты, для которых возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="5a31a-113">Email activity for which statistics are returned.</span></span>|
|<span data-ttu-id="5a31a-114">duration</span><span class="sxs-lookup"><span data-stu-id="5a31a-114">duration</span></span>|<span data-ttu-id="5a31a-115">Длительность</span><span class="sxs-lookup"><span data-stu-id="5a31a-115">Duration</span></span>|<span data-ttu-id="5a31a-116">Общее количество часов, потраченных на электронную почту.</span><span class="sxs-lookup"><span data-stu-id="5a31a-116">Total hours spent on emails.</span></span> <span data-ttu-id="5a31a-117">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="5a31a-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="5a31a-118">endDate</span><span class="sxs-lookup"><span data-stu-id="5a31a-118">endDate</span></span>|<span data-ttu-id="5a31a-119">Date</span><span class="sxs-lookup"><span data-stu-id="5a31a-119">Date</span></span>|<span data-ttu-id="5a31a-120">Дата окончания действия электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5a31a-120">Date when the email activity ended.</span></span> <span data-ttu-id="5a31a-121">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="5a31a-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="5a31a-122">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="5a31a-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="5a31a-123">id</span><span class="sxs-lookup"><span data-stu-id="5a31a-123">id</span></span>|<span data-ttu-id="5a31a-124">String</span><span class="sxs-lookup"><span data-stu-id="5a31a-124">String</span></span>| <span data-ttu-id="5a31a-125">Идентификатор, предназначенный только для чтения, для действия электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5a31a-125">Read-only ID for the email activity.</span></span>|
|<span data-ttu-id="5a31a-126">startDate</span><span class="sxs-lookup"><span data-stu-id="5a31a-126">startDate</span></span>|<span data-ttu-id="5a31a-127">Дата</span><span class="sxs-lookup"><span data-stu-id="5a31a-127">Date</span></span>|<span data-ttu-id="5a31a-128">Дата начала действия электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5a31a-128">Date when the email activity started.</span></span> <span data-ttu-id="5a31a-129">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="5a31a-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="5a31a-130">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="5a31a-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="5a31a-131">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="5a31a-131">timeZoneUsed</span></span>|<span data-ttu-id="5a31a-132">String</span><span class="sxs-lookup"><span data-stu-id="5a31a-132">String</span></span>|<span data-ttu-id="5a31a-133">Часовой пояс, который пользователь задает в календаре Outlook для вычисления.</span><span class="sxs-lookup"><span data-stu-id="5a31a-133">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="5a31a-134">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="5a31a-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="5a31a-135">афтерхаурс</span><span class="sxs-lookup"><span data-stu-id="5a31a-135">afterHours</span></span>|<span data-ttu-id="5a31a-136">Длительность</span><span class="sxs-lookup"><span data-stu-id="5a31a-136">Duration</span></span>|<span data-ttu-id="5a31a-137">Общее количество часов, потраченных на электронную почту за прев рабочее время, которая основана на параметре календаря пользователя Outlook для рабочих часов.</span><span class="sxs-lookup"><span data-stu-id="5a31a-137">Total hours spent on email outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="5a31a-138">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="5a31a-138">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="5a31a-139">реадемаил</span><span class="sxs-lookup"><span data-stu-id="5a31a-139">readEmail</span></span>|<span data-ttu-id="5a31a-140">Длительность</span><span class="sxs-lookup"><span data-stu-id="5a31a-140">Duration</span></span>|<span data-ttu-id="5a31a-141">Общее количество часов, потраченных на чтение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5a31a-141">Total hours spent reading email.</span></span> <span data-ttu-id="5a31a-142">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="5a31a-142">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="5a31a-143">сентемаил</span><span class="sxs-lookup"><span data-stu-id="5a31a-143">sentEmail</span></span>|<span data-ttu-id="5a31a-144">Длительность</span><span class="sxs-lookup"><span data-stu-id="5a31a-144">Duration</span></span>|<span data-ttu-id="5a31a-145">Общее количество часов, потраченных на запись и отправку электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5a31a-145">Total hours spent writing and sending email.</span></span> <span data-ttu-id="5a31a-146">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="5a31a-146">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a31a-147">Связи</span><span class="sxs-lookup"><span data-stu-id="5a31a-147">Relationships</span></span>

<span data-ttu-id="5a31a-148">Нет</span><span class="sxs-lookup"><span data-stu-id="5a31a-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a31a-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a31a-149">JSON representation</span></span>

<span data-ttu-id="5a31a-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a31a-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id", 
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