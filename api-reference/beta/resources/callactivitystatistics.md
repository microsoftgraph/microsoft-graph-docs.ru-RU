---
title: Тип ресурса Каллактивитистатистикс
description: Представляет сведения о действиях звонка для пользователей.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 014cec3f8adab9f8d41b9f3062b38898b9956bb6
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450815"
---
# <a name="callactivitystatistics-resource-type"></a><span data-ttu-id="1e957-103">Тип ресурса Каллактивитистатистикс</span><span class="sxs-lookup"><span data-stu-id="1e957-103">callActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e957-104">Представляет данные о времени, затраченном пользователем на действия звонка в Microsoft Teams или Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1e957-104">Represents data about the user's time spent in call activities on Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="1e957-105">Это основано на [активитистатистикс](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="1e957-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1e957-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e957-106">Properties</span></span>

| <span data-ttu-id="1e957-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e957-107">Property</span></span>     | <span data-ttu-id="1e957-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1e957-108">Type</span></span>        | <span data-ttu-id="1e957-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1e957-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1e957-110">activity</span><span class="sxs-lookup"><span data-stu-id="1e957-110">activity</span></span>|<span data-ttu-id="1e957-111">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="1e957-111">analyticsActivityType</span></span>| <span data-ttu-id="1e957-112">Действие Call, для которого возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="1e957-112">Call activity for which statistics are returned.</span></span>|
|<span data-ttu-id="1e957-113">duration</span><span class="sxs-lookup"><span data-stu-id="1e957-113">duration</span></span>|<span data-ttu-id="1e957-114">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="1e957-114">Duration</span></span>|<span data-ttu-id="1e957-115">Общее количество часов, потраченных на звонки.</span><span class="sxs-lookup"><span data-stu-id="1e957-115">Total hours spent on calls.</span></span> <span data-ttu-id="1e957-116">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="1e957-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="1e957-117">endDate</span><span class="sxs-lookup"><span data-stu-id="1e957-117">endDate</span></span>|<span data-ttu-id="1e957-118">Date</span><span class="sxs-lookup"><span data-stu-id="1e957-118">Date</span></span>|<span data-ttu-id="1e957-119">Дата завершения действия звонка.</span><span class="sxs-lookup"><span data-stu-id="1e957-119">Date when the call activity ended.</span></span> <span data-ttu-id="1e957-120">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="1e957-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="1e957-121">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="1e957-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="1e957-122">id</span><span class="sxs-lookup"><span data-stu-id="1e957-122">id</span></span>|<span data-ttu-id="1e957-123">String</span><span class="sxs-lookup"><span data-stu-id="1e957-123">String</span></span>| <span data-ttu-id="1e957-124">Идентификатор, предназначенный только для чтения, для действия Call.</span><span class="sxs-lookup"><span data-stu-id="1e957-124">Read-only ID for the call activity.</span></span>|
|<span data-ttu-id="1e957-125">startDate</span><span class="sxs-lookup"><span data-stu-id="1e957-125">startDate</span></span>|<span data-ttu-id="1e957-126">Дата</span><span class="sxs-lookup"><span data-stu-id="1e957-126">Date</span></span>|<span data-ttu-id="1e957-127">Дата начала действия звонка.</span><span class="sxs-lookup"><span data-stu-id="1e957-127">Date when the call activity started.</span></span> <span data-ttu-id="1e957-128">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="1e957-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="1e957-129">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="1e957-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="1e957-130">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="1e957-130">timeZoneUsed</span></span>|<span data-ttu-id="1e957-131">String</span><span class="sxs-lookup"><span data-stu-id="1e957-131">String</span></span>|<span data-ttu-id="1e957-132">Для вычисления используется часовой пояс, который пользователь задает в календаре Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="1e957-132">The time zone that the user sets in Microsoft Outlook calendar is used for the computation.</span></span> <span data-ttu-id="1e957-133">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="1e957-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="1e957-134">афтерхаурс</span><span class="sxs-lookup"><span data-stu-id="1e957-134">afterHours</span></span>|<span data-ttu-id="1e957-135">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="1e957-135">Duration</span></span>|<span data-ttu-id="1e957-136">Время, затраченное на вызовы в нерабочее время, которое основано на параметре календаря пользователя Outlook для рабочих часов.</span><span class="sxs-lookup"><span data-stu-id="1e957-136">Time spent on calls outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="1e957-137">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="1e957-137">The value is represented in ISO 8601 format for durations.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1e957-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="1e957-138">Relationships</span></span>

<span data-ttu-id="1e957-139">Нет</span><span class="sxs-lookup"><span data-stu-id="1e957-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e957-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e957-140">JSON representation</span></span>

<span data-ttu-id="1e957-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e957-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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