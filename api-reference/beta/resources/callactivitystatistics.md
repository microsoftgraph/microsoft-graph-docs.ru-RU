---
title: Тип ресурса Каллактивитистатистикс
description: Представляет сведения о действиях звонка для пользователей.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 03625811beec7df8cd679455e9853ea49edf0ed6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507819"
---
# <a name="callactivitystatistics-resource-type"></a><span data-ttu-id="f4357-103">Тип ресурса Каллактивитистатистикс</span><span class="sxs-lookup"><span data-stu-id="f4357-103">callActivityStatistics resource type</span></span>

<span data-ttu-id="f4357-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f4357-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4357-105">Представляет данные о времени, затраченном пользователем на действия звонка в Microsoft Teams или Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f4357-105">Represents data about the user's time spent in call activities on Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="f4357-106">Это основано на [активитистатистикс](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="f4357-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f4357-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4357-107">Properties</span></span>

| <span data-ttu-id="f4357-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4357-108">Property</span></span>     | <span data-ttu-id="f4357-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f4357-109">Type</span></span>        | <span data-ttu-id="f4357-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f4357-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4357-111">activity</span><span class="sxs-lookup"><span data-stu-id="f4357-111">activity</span></span>|<span data-ttu-id="f4357-112">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="f4357-112">analyticsActivityType</span></span>| <span data-ttu-id="f4357-113">Действие Call, для которого возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="f4357-113">Call activity for which statistics are returned.</span></span>|
|<span data-ttu-id="f4357-114">duration</span><span class="sxs-lookup"><span data-stu-id="f4357-114">duration</span></span>|<span data-ttu-id="f4357-115">Длительность</span><span class="sxs-lookup"><span data-stu-id="f4357-115">Duration</span></span>|<span data-ttu-id="f4357-116">Общее количество часов, потраченных на звонки.</span><span class="sxs-lookup"><span data-stu-id="f4357-116">Total hours spent on calls.</span></span> <span data-ttu-id="f4357-117">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="f4357-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="f4357-118">endDate</span><span class="sxs-lookup"><span data-stu-id="f4357-118">endDate</span></span>|<span data-ttu-id="f4357-119">Date</span><span class="sxs-lookup"><span data-stu-id="f4357-119">Date</span></span>|<span data-ttu-id="f4357-120">Дата завершения действия звонка.</span><span class="sxs-lookup"><span data-stu-id="f4357-120">Date when the call activity ended.</span></span> <span data-ttu-id="f4357-121">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="f4357-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="f4357-122">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="f4357-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="f4357-123">id</span><span class="sxs-lookup"><span data-stu-id="f4357-123">id</span></span>|<span data-ttu-id="f4357-124">String</span><span class="sxs-lookup"><span data-stu-id="f4357-124">String</span></span>| <span data-ttu-id="f4357-125">Идентификатор, предназначенный только для чтения, для действия Call.</span><span class="sxs-lookup"><span data-stu-id="f4357-125">Read-only ID for the call activity.</span></span>|
|<span data-ttu-id="f4357-126">startDate</span><span class="sxs-lookup"><span data-stu-id="f4357-126">startDate</span></span>|<span data-ttu-id="f4357-127">Дата</span><span class="sxs-lookup"><span data-stu-id="f4357-127">Date</span></span>|<span data-ttu-id="f4357-128">Дата начала действия звонка.</span><span class="sxs-lookup"><span data-stu-id="f4357-128">Date when the call activity started.</span></span> <span data-ttu-id="f4357-129">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="f4357-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="f4357-130">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="f4357-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="f4357-131">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="f4357-131">timeZoneUsed</span></span>|<span data-ttu-id="f4357-132">String</span><span class="sxs-lookup"><span data-stu-id="f4357-132">String</span></span>|<span data-ttu-id="f4357-133">Для вычисления используется часовой пояс, который пользователь задает в календаре Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="f4357-133">The time zone that the user sets in Microsoft Outlook calendar is used for the computation.</span></span> <span data-ttu-id="f4357-134">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="f4357-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="f4357-135">афтерхаурс</span><span class="sxs-lookup"><span data-stu-id="f4357-135">afterHours</span></span>|<span data-ttu-id="f4357-136">Длительность</span><span class="sxs-lookup"><span data-stu-id="f4357-136">Duration</span></span>|<span data-ttu-id="f4357-137">Время, затраченное на вызовы в нерабочее время, которое основано на параметре календаря пользователя Outlook для рабочих часов.</span><span class="sxs-lookup"><span data-stu-id="f4357-137">Time spent on calls outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="f4357-138">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="f4357-138">The value is represented in ISO 8601 format for durations.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f4357-139">Связи</span><span class="sxs-lookup"><span data-stu-id="f4357-139">Relationships</span></span>

<span data-ttu-id="f4357-140">Нет</span><span class="sxs-lookup"><span data-stu-id="f4357-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4357-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4357-141">JSON representation</span></span>

<span data-ttu-id="f4357-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4357-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id", 
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.callActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->